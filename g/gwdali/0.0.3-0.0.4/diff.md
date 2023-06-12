# Comparing `tmp/gwdali-0.0.3.tar.gz` & `tmp/gwdali-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdali-0.0.3.tar", last modified: Fri Jun  9 21:05:24 2023, max compression
+gzip compressed data, was "gwdali-0.0.4.tar", last modified: Mon Jun 12 02:22:07 2023, max compression
```

## Comparing `gwdali-0.0.3.tar` & `gwdali-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-09 21:05:24.523400 gwdali-0.0.3/
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-09 21:05:24.515400 gwdali-0.0.3/GWDALI/
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-09 21:05:24.519400 gwdali-0.0.3/GWDALI/Detectors_Sensitivity/
--rw-r--r--   0 josiel    (1000) josiel    (1000)       14 2022-11-09 20:10:14.000000 gwdali-0.0.3/GWDALI/Detectors_Sensitivity/__init__.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)      921 2023-02-28 14:51:14.000000 gwdali-0.0.3/GWDALI/Detectors_Sensitivity/plot_Sn.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     8949 2023-05-16 02:06:35.000000 gwdali-0.0.3/GWDALI/GWDALI.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)      143 2023-01-12 01:48:50.000000 gwdali-0.0.3/GWDALI/__init__.py
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-09 21:05:24.519400 gwdali-0.0.3/GWDALI/lib/
--rw-r--r--   0 josiel    (1000) josiel    (1000)     2945 2022-08-02 22:07:40.000000 gwdali-0.0.3/GWDALI/lib/Angles_lib.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     8601 2023-05-16 02:02:47.000000 gwdali-0.0.3/GWDALI/lib/Compute_Tensors.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     5858 2023-02-16 19:29:30.000000 gwdali-0.0.3/GWDALI/lib/Corner_Plots.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     5579 2023-05-16 01:58:53.000000 gwdali-0.0.3/GWDALI/lib/Derivatives_Tensors.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     3172 2023-05-16 01:56:05.000000 gwdali-0.0.3/GWDALI/lib/Dictionaries.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     7896 2023-04-13 14:39:02.000000 gwdali-0.0.3/GWDALI/lib/Likelihood.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     3274 2023-01-20 00:22:18.000000 gwdali-0.0.3/GWDALI/lib/Symmetric_Indexies.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     4479 2023-05-16 02:00:22.000000 gwdali-0.0.3/GWDALI/lib/Waveforms.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)      145 2023-01-12 19:30:22.000000 gwdali-0.0.3/GWDALI/lib/__init__.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     1089 2023-03-21 13:34:46.000000 gwdali-0.0.3/LICENSE
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     5058 2023-06-09 21:05:24.523400 gwdali-0.0.3/PKG-INFO
--rw-r--r--   0 josiel    (1000) josiel    (1000)     4709 2023-04-14 13:50:04.000000 gwdali-0.0.3/README.md
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-09 21:05:24.523400 gwdali-0.0.3/gwdali.egg-info/
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     5058 2023-06-09 21:05:24.000000 gwdali-0.0.3/gwdali.egg-info/PKG-INFO
--rw-rw-r--   0 josiel    (1000) josiel    (1000)      511 2023-06-09 21:05:24.000000 gwdali-0.0.3/gwdali.egg-info/SOURCES.txt
--rw-rw-r--   0 josiel    (1000) josiel    (1000)        1 2023-06-09 21:05:24.000000 gwdali-0.0.3/gwdali.egg-info/dependency_links.txt
--rw-rw-r--   0 josiel    (1000) josiel    (1000)        7 2023-06-09 21:05:24.000000 gwdali-0.0.3/gwdali.egg-info/top_level.txt
--rw-rw-r--   0 josiel    (1000) josiel    (1000)       38 2023-06-09 21:05:24.523400 gwdali-0.0.3/setup.cfg
--rw-r--r--   0 josiel    (1000) josiel    (1000)      658 2023-06-09 21:04:36.000000 gwdali-0.0.3/setup.py
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-12 02:22:07.238126 gwdali-0.0.4/
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-12 02:22:07.234126 gwdali-0.0.4/GWDALI/
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-12 02:22:07.234126 gwdali-0.0.4/GWDALI/Detectors_Sensitivity/
+-rw-r--r--   0 josiel    (1000) josiel    (1000)       14 2022-11-09 20:10:14.000000 gwdali-0.0.4/GWDALI/Detectors_Sensitivity/__init__.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      921 2023-02-28 14:51:14.000000 gwdali-0.0.4/GWDALI/Detectors_Sensitivity/plot_Sn.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     9246 2023-06-12 01:59:52.000000 gwdali-0.0.4/GWDALI/GWDALI.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      143 2023-01-12 01:48:50.000000 gwdali-0.0.4/GWDALI/__init__.py
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-12 02:22:07.234126 gwdali-0.0.4/GWDALI/lib/
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     2945 2022-08-02 22:07:40.000000 gwdali-0.0.4/GWDALI/lib/Angles_lib.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     8601 2023-05-16 02:02:47.000000 gwdali-0.0.4/GWDALI/lib/Compute_Tensors.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     5858 2023-02-16 19:29:30.000000 gwdali-0.0.4/GWDALI/lib/Corner_Plots.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     5713 2023-06-12 02:03:46.000000 gwdali-0.0.4/GWDALI/lib/Derivatives_Tensors.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     3172 2023-05-16 01:56:05.000000 gwdali-0.0.4/GWDALI/lib/Dictionaries.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     8121 2023-06-09 16:38:20.000000 gwdali-0.0.4/GWDALI/lib/Likelihood.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     3274 2023-01-20 00:22:18.000000 gwdali-0.0.4/GWDALI/lib/Symmetric_Indexies.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     4479 2023-05-16 02:00:22.000000 gwdali-0.0.4/GWDALI/lib/Waveforms.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      145 2023-01-12 19:30:22.000000 gwdali-0.0.4/GWDALI/lib/__init__.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     1089 2023-03-21 13:34:46.000000 gwdali-0.0.4/LICENSE
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     5058 2023-06-12 02:22:07.238126 gwdali-0.0.4/PKG-INFO
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     4709 2023-04-14 13:50:04.000000 gwdali-0.0.4/README.md
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2023-06-12 02:22:07.238126 gwdali-0.0.4/gwdali.egg-info/
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     5058 2023-06-12 02:22:07.000000 gwdali-0.0.4/gwdali.egg-info/PKG-INFO
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)      511 2023-06-12 02:22:07.000000 gwdali-0.0.4/gwdali.egg-info/SOURCES.txt
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)        1 2023-06-12 02:22:07.000000 gwdali-0.0.4/gwdali.egg-info/dependency_links.txt
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)        7 2023-06-12 02:22:07.000000 gwdali-0.0.4/gwdali.egg-info/top_level.txt
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)       38 2023-06-12 02:22:07.238126 gwdali-0.0.4/setup.cfg
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      658 2023-06-12 02:20:47.000000 gwdali-0.0.4/setup.py
```

### Comparing `gwdali-0.0.3/GWDALI/Detectors_Sensitivity/plot_Sn.py` & `gwdali-0.0.4/GWDALI/Detectors_Sensitivity/plot_Sn.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.3/GWDALI/GWDALI.py` & `gwdali-0.0.4/GWDALI/GWDALI.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,62 +28,67 @@
 
 #-------------------------------------------------
 # From Dictionaries.py
 Waveforms, PSD, labels_tex = gwdict.Load_Dictionaries()
 #-------------------------------------------------
 freq0 = 10**np.linspace(0,4,4000)
 
-'''
-#-------------------------------------------------------
-# CAUTION! From GWFISH 
-#-------------------------------------------------------
-def invertSVD(matrix): 
-    thresh = 1e-10
-
-    dm = np.sqrt(np.diag(matrix))
-    normalizer = np.outer(dm, dm)
-    matrix_norm = matrix / normalizer
-
-    [U, S, Vh] = np.linalg.svd(matrix_norm)
-
-    kVal = sum(S > thresh)
-    matrix_inverse_norm = U[:, 0:kVal] @ np.diag(1. / S[0:kVal]) @ Vh[0:kVal, :]
-
-    # print(matrix @ (matrix_inverse_norm / normalizer))
-
-    return matrix_inverse_norm / normalizer
-#-------------------------------------------------------
-'''
-
-#-------------------------------------------------------
-# Numpy routine: 
+#-------------------------------------------------------------------------------
 #	"Compute the (Moore-Penrose) pseudo-inverse of a matrix"
-#-------------------------------------------------------
+#-------------------------------------------------------------------------------
 def invert_matrix(matrix, rcond): 
 
     dm = np.sqrt(np.diag(matrix))
     norm = np.outer(dm, dm)
     M_norm = matrix / norm
 
     M_inv = np.linalg.pinv(M_norm,rcond=rcond)
 
     return M_inv / norm
 #-------------------------------------------------------
+# Get Waveforms and SNR
+#-------------------------------------------------------
+def get_strain_snr(gw_prms,detectors,approximant='TaylorF2',fmin=1.,fmax=1.e4,fsize=3.e3):
+	Strains, SNR = [], []
+	rho2 = 0
 
+	freq = 10**np.linspace(np.log10(fmin), np.log10(fmax), int(fsize))
+	for idx in range(len(detectors)):
+		det = detectors[idx]
+		name = det['name']
+		Sn0 = PSD[name]
+		func_Sn = interp1d(freq0, Sn0, fill_value=np.inf, bounds_error=False)
+		detectors[idx]['freq'] = freq
+		detectors[idx]['Sn']   = func_Sn(freq)
+
+		h 	  = gwfunc.Signal(gw_prms, det, approximant)
+		SNR2  = gwfunc.ScalarProduct(det['freq'], det['Sn'],h,h)
+		rho2 += SNR2
+
+		Strains.append(h)
+		SNR.append(np.sqrt(SNR2))
+
+	hp, hx = gwfunc.GW_Polarizations(gw_prms,freq, approximant)
+
+	return [hp,hx,freq], Strains, SNR, np.sqrt(rho2)
+#-------------------------------------------------------
+# Main Function
+#-------------------------------------------------------
 def GWDALI( Detection_Dict, 
 			FreeParams, 
 			detectors, 
 			approximant = 'TaylorF2',
 			fmin  = 1., 
 			fmax  = 1.e4, 
 			fsize = 3000, 
 			dali_method    = 'Doublet',
 			sampler_method = 'nestle', 
 			npoints      = 100,
 			rcond		 = 1.e-4,
+			new_priors   = None,
 			save_samples = False, 
 			save_cov     = False, 
 			save_fisher  = False,
 			plot_corner  = False,
 			hide_info    = False,
 			index		 = 1):
 
@@ -96,51 +101,51 @@
 		print(" >> approximant: %s" % approximant)
 		print(" >> sampler_method: %s\n" % sampler_method)
 
 	T1 = now()
 	
 	cond_out = any([save_cov, save_samples, save_fisher, plot_corner])
 	#-----------------------------------------------------------------------------------
-	# Cria uma pasta para armazenar os resultados
+	# Make a directory to store the results
 	if(cond_out):
 		path = 'output_%s/' % dali_method
 		if(not os.path.isdir(path)): os.mkdir(path)
 	#-----------------------------------------------------------------------------------
 
 	Np   = len(FreeParams)
 	keys = Detection_Dict.keys()
 	freq = 10**np.linspace(np.log10(fmin), np.log10(fmax), fsize)
 
 	#-------------------------------------------------
-	# Atribuir ao detector seu respectivo Sn(f)
+	# Setting Sn(f) by interpolation
 	for idx in range(len(detectors)):
 		det = detectors[idx]
 		name = det['name']
 		Sn0 = PSD[name]
 		func_Sn = interp1d(freq0, Sn0, fill_value=np.inf, bounds_error=False)
 		detectors[idx]['freq'] = freq
 		detectors[idx]['Sn']   = func_Sn(freq)
 
 	t_init = now()
 	#-----------------------------------------------------------------------------------
 	
 	Result = {}
 
-	#=====================================================
-	# Armazena os valores das injeções (Dict)
+	#-------------------------------------------------------
+	# Store the injection values (Dict)
 	truths = {}
 	for key in Detection_Dict.keys():
 		truths[key] = Detection_Dict[key]
-	#=====================================================
-	# Armazena os valores das injeções (List)
+	#-------------------------------------------------------
+	# Store the injection values (List)
 	Theta0 = []
 	for fp in FreeParams:
 		Theta0.append(Detection_Dict[fp])
 	Theta0 = np.array(Theta0)
-	#=====================================================
+	#-------------------------------------------------------
 	
 	t1 = now()
 	#-----------------------------------------------------------------------------------
 	# From Compute_Tensors.py (looping in detectors)
 	#-----------------------------------------------------------------------------------
 	SNR , GwData, Fisher , Doublet , Triplet = Get_Tensors(FreeParams, Detection_Dict, detectors, dali_method, approximant,hide_info)
 	Tensors = [Fisher , Doublet , Triplet]
@@ -165,16 +170,15 @@
 
 	if(not hide_info):
 		print("\n Fisher = \n", np.matrix(Fisher),'\n')
 		print("\n Covariance = \n", np.matrix(Cov),'\n')
 		print("-----"*10+'\n')
 
 	#------------------------------------------------------
-	#------------------------------------------------------
-	# Salvar as injeções nas headers de cada file:
+	# Save the injection in each file headers:
 	#------------------------------------------------------
 	header01 = 'FullInjections:\n'
 	header02 = ''
 	for key in keys:
 		header01 += "%s\t" % key
 		header02 += "%e\t" % Detection_Dict[key]
 	header1 = 'Injections: ' ; header2 = '' ; line = '---'*10
@@ -194,15 +198,15 @@
 	#------------------------------------------------------
 	# From Likelihood.py
 	#------------------------------------------------------
 	if(dali_method != 'Fisher'):
 		# allowed only for Fisher_Sampling and Doublet
 		if(not hide_info): print("Running Sampler ...\n")
 		#------------------------------------------------------#------------------------------------------------------
-		M = get_posterior(FreeParams, Theta0, Detection_Dict, GwData, approximant, detectors, Tensors, dali_method, sampler_method, npoints)
+		M = get_posterior(FreeParams, Theta0, Detection_Dict, GwData, approximant, detectors, Tensors, dali_method, sampler_method, npoints, new_priors)
 		#------------------------------------------------------#------------------------------------------------------
 		Cov2 = np.matrix( np.cov(np.transpose(M)) )
 		header3 = header + '\n' + line + '\nRecovery:\n'
 		for i in range(len(FreeParams)): header3 += '%e\t' % np.average(M[:,i])
 		header3 += '\n' + line
 		if(save_cov): np.savetxt(path+'Covariance_Matrix_%d.txt'%(index),Cov2,fmt='%e',delimiter='\t',header=header3)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gwdali-0.0.3/GWDALI/lib/Angles_lib.py` & `gwdali-0.0.4/GWDALI/lib/Angles_lib.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.3/GWDALI/lib/Compute_Tensors.py` & `gwdali-0.0.4/GWDALI/lib/Compute_Tensors.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.3/GWDALI/lib/Corner_Plots.py` & `gwdali-0.0.4/GWDALI/lib/Corner_Plots.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.3/GWDALI/lib/Derivatives_Tensors.py` & `gwdali-0.0.4/GWDALI/lib/Derivatives_Tensors.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #-------------------------------------------------
 def Integral(x,y):
 	return np.sum( np.array( [0.5*(y[i]+y[i-1])*(x[i]-x[i-1]) for i in range(1,len(x)) ] ) )
 
 def ScalarProduct(freq,Sn,A,B):
 	return 4*np.real( Integral(freq, A*np.conj(B)/Sn) )
 
-def Signal(params, detector, approximant):
+def GW_Polarizations(params, freq, approximant):
 	keys = list(params.keys())
 	
 	#-------------------------------------------------
 	# Convert Masses
 	#-------------------------------------------------
 	if(all( p in  keys for p in ['m1','m2'])):
 		m1 = params['m1'] ; m2 = params['m2']
@@ -43,51 +43,58 @@
 	elif(all( p in keys for p in ['Mc','q'] )):
 		Mc = params['Mc'] ; q = params['q'] # q = m2/m1
 		m2 = ( q*q*(1.+q) )**0.2 * Mc
 		m1 = m2/q 
 	else: print("\n\n# Invalid options to mass! \n\t >> Available: [m1,m2] or [Mc,eta] or [Mc,q]\n\n")
 	#-------------------------------------------------
 
-	alpha    = params['RA']*rad       # rad
-	beta     = (90-params['Dec'])*rad # rad
 	DL       = params['DL']*1.e3      # Gpc --> Mpc
 	iota     = params['iota']         # rad
 	psi      = params['psi']          # rad
-	t_coal   = params['t_coal']       # sec
-	phi_coal = params['phi_coal']     # rad
 
 	sx1 = params['sx1']
 	sy1 = params['sy1']
 	sz1 = params['sz1']
 	sx2 = params['sx2']
 	sy2 = params['sy2']
 	sz2 = params['sz2']
 
 	s1 = [sx1, sy1, sz1]
 	s2 = [sx2, sy2, sz2]
 
+	hp, hx, _ = Waveforms[approximant](m1,m2,iota,DL,s1,s2,freq)
+
+	return hp, hx
+
+def Signal(params, detector, approximant):
+	alpha    = params['RA']*rad       # rad
+	beta     = (90-params['Dec'])*rad # rad
+	iota     = params['iota']         # rad
+	psi      = params['psi']          # rad
+	t_coal   = params['t_coal']       # sec
+	phi_coal = params['phi_coal']     # rad
+	
 	name  = detector['name']
 	freq  = detector['freq'].copy()
 	lon   = detector['lon'] # deg
 	lat   = detector['lat'] # deg
 	rot   = detector['rot']*rad # rad
 
 	phi   = lon*rad
 	theta = (90-lat)*rad
 
 	alpha_obs, beta_obs = geo.AngTransf(alpha,beta,theta,phi,rot)
 	psi_obs             = geo.poll_ang(alpha,beta,iota,psi,theta,phi,rot)
 
 	t_delay = -np.cos(beta_obs)*R_earth/c
 
-	Fp, Fx    = Pattern_Func(alpha_obs,beta_obs,psi_obs,detector['shape'])
-	hp, hx, _ = Waveforms[approximant](m1,m2,iota,DL,s1,s2,freq)
+	Fp, Fx = Pattern_Func(alpha_obs,beta_obs,psi_obs,detector['shape']*rad)
+	hp, hx = GW_Polarizations(params, freq, approximant)
 
-	exp2 = np.exp(-1.j*phi_coal) #
-	#exp2 = np.exp( 1.j*( 2*np.pi*freq*(t_coal+t_delay) - phi_coal )  )
+	exp2 = np.exp(-1.j*phi_coal)
 
 	h = Fp*hp + Fx*hx
 	
 	return h * exp2	
 
 #-------------------------------------------------
```

### Comparing `gwdali-0.0.3/GWDALI/lib/Dictionaries.py` & `gwdali-0.0.4/GWDALI/lib/Dictionaries.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.3/GWDALI/lib/Likelihood.py` & `gwdali-0.0.4/GWDALI/lib/Likelihood.py`

 * *Files 8% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 H = cosmo.H(x).value
 Rc = d/(1+x)
 priorD = 4*np.pi*Rc**2/H
 xx = d/1.e3
 yy = priorD/sum(priorD)
 #----------------------------------------
 
-def get_posterior(FreeParams, Theta0, Detection_Dict, GwData, approximant, Detectors, Tensors, dali_method, sampler_method, npoints):
+def get_posterior(FreeParams, Theta0, Detection_Dict, GwData, approximant, Detectors, Tensors, dali_method, sampler_method, npoints,new_priors):
 	Dict = {}
 	DL0 = Detection_Dict['DL']
 	d1 = cosmo.luminosity_distance(0.001).value / 1.e3 # Gpc
 	d2 = cosmo.luminosity_distance(5.0).value / 1.e3   # Gpc
 	#----------------------------#----------------------------#----------------------------
 	Dict['DL']    = bilby.core.prior.Interped(name='DL',xx=xx,yy=yy,minimum=d1, maximum=d2)
 	Dict['iota']  = bilby.core.prior.Sine(name='iota', minimum=0, maximum=np.pi)
@@ -168,22 +168,26 @@
 	#----------------------------#----------------------------#----------------------------
 	Dict['phi_coal']  = bilby.core.prior.Uniform(name='phi_coal',minimum=0, maximum=2*np.pi)
 	Dict['t_coal']    = bilby.core.prior.Uniform(name='t_coal',minimum=0, maximum=3600) # 1 hour
 	#----------------------------#----------------------------#----------------------------
 
 	Priors = {}
 	for fp in FreeParams:
-		Priors[fp] = Dict[fp]
-
-	'''
-	self.FreeParams = args[0]
-	self.Data       = args[1]
-	self.GWparams   = args[2]
-	self.DetAp		= args[3]
-	'''
+		if(new_priors == None):
+			Priors[fp] = Dict[fp]
+		elif(not (fp in new_priors.keys()) ):
+			Priors[fp] = Dict[fp]
+		else:
+			try:
+				x, y = new_priors[fp]
+				y /= sum(y)
+				Priors[fp] = bilby.core.prior.Interped(name=fp,xx=x,yy=y,minimum=min(x),maximum=max(x))
+			except:
+				print('\n>> Invalid key/argment in new_priors dictionay!\n')
+				quit()
 
 	if(dali_method=='Standard'):
 		likelihood = GW_likelihood([FreeParams, GwData, Detection_Dict, [Detectors,approximant] ])
 	else:
 		likelihood = DALI_likelihood([FreeParams, Theta0, Tensors, dali_method])
 
 	outdir = 'outdir_%s_%d/' % (dali_method, int(np.random.uniform(0,300))  )
```

### Comparing `gwdali-0.0.3/GWDALI/lib/Symmetric_Indexies.py` & `gwdali-0.0.4/GWDALI/lib/Symmetric_Indexies.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.3/GWDALI/lib/Waveforms.py` & `gwdali-0.0.4/GWDALI/lib/Waveforms.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.3/LICENSE` & `gwdali-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.3/PKG-INFO` & `gwdali-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdali
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Fisher-Based Software for Parameter Estimation from Gravitational Waves
 Author: Josiel Mendonça Soares de Souza
 Author-email: jmsdsouza.phd@gmail.com
 License: MIT License
 Keywords: fisher matrix,gravitational waves,gw,dali
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gwdali-0.0.3/README.md` & `gwdali-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gwdali-0.0.3/gwdali.egg-info/PKG-INFO` & `gwdali-0.0.4/gwdali.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdali
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Fisher-Based Software for Parameter Estimation from Gravitational Waves
 Author: Josiel Mendonça Soares de Souza
 Author-email: jmsdsouza.phd@gmail.com
 License: MIT License
 Keywords: fisher matrix,gravitational waves,gw,dali
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gwdali-0.0.3/setup.py` & `gwdali-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md",'r') as arq:
 	readme = arq.read()
 
 setup(
 	name = 'gwdali',
-	version = '0.0.3',
+	version = '0.0.4',
 	license = 'MIT License',
 	author  = 'Josiel Mendonça Soares de Souza',
 	long_description = readme,
 	long_description_content_type = "text/markdown",
 	author_email = 'jmsdsouza.phd@gmail.com',
 	keywords = 'fisher matrix, gravitational waves, gw, dali',
 	description = 'A Fisher-Based Software for Parameter Estimation from Gravitational Waves',
```

