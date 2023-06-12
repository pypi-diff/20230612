# Comparing `tmp/pybrick-0.2.3-py3-none-any.whl.zip` & `tmp/pybrick-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4421 bytes, number of entries: 6
+Zip file size: 4754 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-30 13:40 pybrick/__init__.py
--rw-rw-rw-  2.0 fat     8685 b- defN 22-Jul-06 18:45 pybrick/pybrick.py
--rw-rw-rw-  2.0 fat      321 b- defN 22-Jul-06 18:50 pybrick-0.2.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Jul-06 18:50 pybrick-0.2.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 22-Jul-06 18:50 pybrick-0.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      444 b- defN 22-Jul-06 18:50 pybrick-0.2.3.dist-info/RECORD
-6 files, 9550 bytes uncompressed, 3613 bytes compressed:  62.2%
+-rw-rw-rw-  2.0 fat    10069 b- defN 23-Jun-12 20:01 pybrick/pybrick.py
+-rw-rw-rw-  2.0 fat      321 b- defN 23-Jun-12 20:07 pybrick-0.2.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 20:07 pybrick-0.2.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-12 20:07 pybrick-0.2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      445 b- defN 23-Jun-12 20:07 pybrick-0.2.4.dist-info/RECORD
+6 files, 10935 bytes uncompressed, 3946 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pybrick/__init__.py
 Comment: 
 
 Filename: pybrick/pybrick.py
 Comment: 
 
-Filename: pybrick-0.2.3.dist-info/METADATA
+Filename: pybrick-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: pybrick-0.2.3.dist-info/WHEEL
+Filename: pybrick-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: pybrick-0.2.3.dist-info/top_level.txt
+Filename: pybrick-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pybrick-0.2.3.dist-info/RECORD
+Filename: pybrick-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pybrick/pybrick.py

```diff
@@ -27,14 +27,24 @@
         if hasattr(self,"connection"):
             try:
                 self.disconnect()
             except:
                 pass
         return
     
+    def __repr__(self):
+        """ """
+        stat="CONNECTED"
+        try:
+            self.connection.execute("select 1")
+        except:
+            stat="DISCONNECTED"
+            
+        return(f"Yellowbrick connector for user {self.user} on host {self.host}.\n{stat}")
+    
     def _checkConnection(self,reconnect=False):
         """ When using psycopg2 interactively, it's not unusual for the db
             connection to become invalid due to idle timeout.  Before issuing
             a query, check the connection and optionally reconnect if needed.
         """
         try:
             self.connection.execute("select 1")
@@ -62,28 +72,36 @@
             password=self.pw,
             host=self.host,
             database=self.db,
         )
         
         try:
             self.engine=sa.create_engine(connection_url,pool_pre_ping=True)
-            conn=self.engine.connect()
+            conn=self.engine.connect().execution_options(isolation_level="AUTOCOMMIT")
             return conn
         except Exception as details:
             print("Error connecting using:",(self.host,self.db,self.user,self.pw))
             print(">>> ",details)
             sys.exit()
     
     def disconnect(self):
         """ """
         if self.connection:
             self.connection.close()
         return
     
-    def query(self,query_to_run,withResults=False,withData=False,dryRun=False,dumpTo=None,dumpAppend=False,printQuery=False):
+    def query(self,query_to_run,dryRun=False,dumpTo=None,dumpAppend=False,printQuery=False):
+        """ Query implies fetch data. """
+        return self._query(query_to_run,withData=True,dryRun=dryRun,dumpTo=dumpTo,dumpAppend=dumpAppend,printQuery=printQuery)
+        
+    def execute(self,query_to_run,dryRun=False,dumpTo=None,dumpAppend=False,printQuery=False):
+        """ Execute implies don't fetch data. """
+        return self._query(query_to_run,withData=False,dryRun=dryRun,dumpTo=dumpTo,dumpAppend=dumpAppend,printQuery=printQuery)
+    
+    def _query(self,query_to_run,withResults=False,withData=False,dryRun=False,dumpTo=None,dumpAppend=False,printQuery=False):
         """ Query Yellowbrick, optionally returning a dataframe of results. """
         self._checkConnection(reconnect=True)
         
         df=None
         if dumpTo:
             mode="a+" if dumpAppend else "w+"
             open(os.path.join(".",dumpTo),mode).write(query_to_run)
@@ -118,102 +136,117 @@
         (db,tbl)=table.split(".")
         q=f"""
             select count(*) as rc
             from information_schema.tables
             where upper(table_schema)=upper('{db}')
               and upper(table_name)=upper('{tbl}')
         """
-        d=self.query(q,withData=True)
+        d=self.query(q)
         return d.rc[0]>0
     
     def tableRowCount(self,table):
         """ """
         q=f"""
             select count(*) as rc
             from {table}
         """
-        d=self.query(q,withData=True)
+        d=self.query(q)
         return d.rc[0]
     
+    def sample(self,table,fields=None,limit=10,orderby=None):
+       """ """
+       h="Sample of "+table
+       print(h+"\n"+("-"*len(h)))
+       return self.query(f"select {fields if fields else '*'} from {table} order by {orderby if orderby else 'random()'} limit {limit}")
+    
     
     def getDfDDL(self,src,ybTypes=None):
         """ """
         if not ybTypes:
             #If were weren't supplied types, guess them ourselves.
             ybTypes=self.getYbTypesFromDf(src)
             
         ddl = ""
         for i in range(len(src.columns)):
             #New DDL line for each element.  Trickiness to handle no-comma for last element.
-            ddl+="    %s %s%s\n"%(src.columns[i],ybTypes[i],(i<len(src.columns)-1)*",")
+            ddl+='    "%s" %s%s\n'%(src.columns[i],ybTypes[i],(i<len(src.columns)-1)*",")
             
         return ddl
 
     def dfToYb(self,src,target,distribute_on="random",clobber=False,ybTypes=None,verbose=False,ignoreLoadErrors=False):
         """ Given a pandas df, push that table to yellowbrick, optionally replace the existing table in yellowbrick.
             If ybTypes immutable is provided, use those types and to hell with the consequences.
             Otherwise, infer the types.
         """
         
-        print("Loading %d rows and %d columns into %s."%(src.shape[0],src.shape[1],target))
-        print("Here is a sample of the source data:\n%s\n"%src.head(5))
+        def vprint(s):
+            if verbose:
+                print(s)
+        
+        print(f"Loading {src.shape[0]} rows and {src.shape[1]} columns into {target}.")
+        vprint(f"Here is a sample of the source data:\n{src.head(5)}")
         
         if not ybTypes:
             #If were weren't supplied types, guess them ourselves.
             ybTypes=self.getYbTypesFromDf(src)
         
         if clobber:
-            print("Dropping %s." %target)
-            self.query("drop table if exists %s;"%target)
+            vprint(f"Dropping {target}.")
+            self.execute(f"drop table if exists {target};")
         
         maxbad="0"
         if ignoreLoadErrors:
             maxbad="-1"
         
         ddl = self.getDfDDL(src,ybTypes)
         
         dump=tempfile.mkstemp(".csv")[1]
-        print("Dumping local data to %s." %dump)
-        src.to_csv(dump,index=False,header=True,line_terminator="\n")
-        print("Dumped %0.2fMB."%(os.path.getsize(dump)/1024/1024),verbose)
-        
-        self.query(f"""
-            create table {target} (
-                {ddl}
-            )
-            ;
-        """,printQuery=True)
+        vprint(f"Dumping local data to {dump}")
+        src.to_csv(dump,index=False,header=True,lineterminator="\n")
+        vprint(f"Dumped {os.path.getsize(dump)/1024/1024:0.2f}MB.")
+        
+        if not self.tableExists(target):
+            self.execute(f"""
+                create table {target} (
+                    {ddl}
+                )
+                ;
+            """,printQuery=verbose)
         
         os.environ["YBPASSWORD"]=self.pw
         cmd=rf'"C:\Program Files\Yellowbrick Data\Client Tools\bin\ybload.exe" --host {self.host} --username {self.user} --dbname {self.db} --max-bad-rows {maxbad} --csv-skip-header-line true --table {target} {dump}'
-        print("Running this now ===>",cmd)
+        vprint(f"Running this now ===> {cmd}")
         
         try:
-            print(subprocess.call(cmd))
+            _=subprocess.call(cmd)
         except Exception as details:
             print(f"There was a problem running ybload.  Make sure it's installed, is on your PATH, and that Java is installed:\n{details}\n")
             sys.exit(1)
         
         lrows = self.tableRowCount(target)
-        if len(src)==lrows:
-            print(f"Looks good: We dumped {len(src)} rows, and then loaded {lrows} rows.")
+        if len(src)==lrows or clobber==False:
+            print("YBload successful")
+            vprint(f"Dumped {len(src)} rows, and then loaded {lrows} rows.")
         else:
             print("THERE MIGHT HAVE BEEN A PROBLEM LOADING!  The number of rows loaded doesn't match the input length.  Check the output.")
         
         return
     
+    #Alias
+    df2Yb=dfToYb
+    
     def getYbTypesFromDf(self,df):
         """ Try to map.  This is almost vulgar.
             Return a tuple the same size as dftypes."""
         default_yb = "varchar(255)"
         df2yb = {'int64':'bigint',
                  'int32':'bigint',
                  'float64':'float',
                  'float32':'float',
-                 'object':'varchar(255)'}
+                 'object':'varchar(1024)'}
         ybtypes = []
         for t in df.dtypes:
             ybtypes.append(df2yb.get(t.name,default_yb))
         return(tuple(ybtypes))
```

