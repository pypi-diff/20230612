# Comparing `tmp/captif_cpx_db-0.6.tar.gz` & `tmp/captif_cpx_db-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_db-0.6.tar", max compression
+gzip compressed data, was "captif_cpx_db-0.7.tar", max compression
```

## Comparing `captif_cpx_db-0.6.tar` & `captif_cpx_db-0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-06-07 04:06:38.965736 captif_cpx_db-0.6/LICENSE
--rw-r--r--   0        0        0       16 2023-06-07 04:06:38.965736 captif_cpx_db-0.6/README.md
--rw-r--r--   0        0        0       20 2023-06-07 04:06:38.965736 captif_cpx_db-0.6/captif_cpx_db/__init__.py
--rw-r--r--   0        0        0    28571 2023-06-07 04:06:38.965736 captif_cpx_db-0.6/captif_cpx_db/models.py
--rw-r--r--   0        0        0      504 2023-06-07 04:06:38.965736 captif_cpx_db-0.6/pyproject.toml
--rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 captif_cpx_db-0.6/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-12 00:05:09.043789 captif_cpx_db-0.7/LICENSE
+-rw-r--r--   0        0        0       16 2023-06-12 00:05:09.043789 captif_cpx_db-0.7/README.md
+-rw-r--r--   0        0        0       20 2023-06-12 00:05:09.043789 captif_cpx_db-0.7/captif_cpx_db/__init__.py
+-rw-r--r--   0        0        0    26968 2023-06-12 00:05:09.043789 captif_cpx_db-0.7/captif_cpx_db/models.py
+-rw-r--r--   0        0        0      504 2023-06-12 00:05:09.043789 captif_cpx_db-0.7/pyproject.toml
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 captif_cpx_db-0.7/PKG-INFO
```

### Comparing `captif_cpx_db-0.6/LICENSE` & `captif_cpx_db-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_db-0.6/captif_cpx_db/models.py` & `captif_cpx_db-0.7/captif_cpx_db/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         nullable=False,
         description="tyre type (e.g., P1, H1, etc.)",
     )
     tyre_purchase_date: date_ = Field(
         nullable=False,
         description="purchase date of the tyre",
     )
-    hardness: condecimal(max_digits=3, decimal_places=1) = Field(
+    hardness: condecimal(decimal_places=1) = Field(
         nullable=False,
         description="tyre hardness in Shore A",
     )
     hardness_date: date_ = Field(
         nullable=False,
         description="date of hardness measurement",
     )
@@ -154,18 +154,15 @@
         primary_key=True,
         description="microphone position (1-6) as per ISO 11819-2:2017",
     )
     microphone_serial_number: str = Field(
         nullable=False,
         description="microphone serial number",
     )
-    microphone_sensitivity_mv_pa: condecimal(
-        max_digits=4,
-        decimal_places=2,
-    ) = Field(
+    microphone_sensitivity_mv_pa: condecimal(decimal_places=2) = Field(
         nullable=False,
         description="microphone sensitivity in mV/Pa",
     )
     microphone_calibration_date: date_ = Field(
         nullable=False,
         description="microphone calibration date",
     )
@@ -201,18 +198,15 @@
         primary_key=True,
         description="accelerometer position ('chassis' or 'axle')",
     )
     accelerometer_serial_number: str = Field(
         nullable=False,
         description="accelerometer serial number",
     )
-    accelerometer_sensitivity_mv_g: condecimal(
-        max_digits=5,
-        decimal_places=2,
-    ) = Field(
+    accelerometer_sensitivity_mv_g: condecimal(decimal_places=2) = Field(
         nullable=False,
         description="accelerometer sensitivity in mV/g",
     )
     wav_file_channel_number: int = Field(
         nullable=False,
         description=(
             "channel number in the wav file corresponding to the accelerometer"
@@ -242,19 +236,19 @@
         default=None,
         primary_key=True,
     )
     wheel_bay_name: Optional[str] = Field(
         default=None,
         primary_key=True,
     )
-    frequency_hz: condecimal(max_digits=6, decimal_places=1) = Field(
+    frequency_hz: condecimal(decimal_places=1) = Field(
         primary_key=True,
         description="one-third octave band centre frequency in Hz",
     )
-    correction_db: condecimal(decimal_places=2) = Field(
+    correction_db: float = Field(
         nullable=False,
         description="device correction in dB",
     )
 
 
 """
 Session-level (results set) models
@@ -381,24 +375,20 @@
     hardness_coefficient: condecimal(decimal_places=3) = Field(
         nullable=False,
         description=(
             "hardness coefficient in dB/Shore A used to calculate the "
             "hardness correction"
         ),
     )
-    hardness_correction_db: condecimal(decimal_places=2) = Field(
+    hardness_correction_db: float = Field(
         nullable=False,
         description="hardness correction value in dB",
     )
     microphone_details: List["ResultsSetMicrophoneDetails"] = Relationship()
 
-    @validator("hardness_correction_db", pre=True)
-    def round_2(cls, v):
-        return round(v, 2) if v is not None else None
-
 
 class ResultsSetMicrophoneDetails(SQLModel, table=True):
     """
     Results set (session) level microphone details.
     """
 
     __tablename__ = "results_set_microphone_details"
@@ -536,27 +526,27 @@
         nullable=False,
         description=(
             "wav sample number corresponding to the end of the road "
             "segment. This is the same side of the road segment as 'end_m', "
             "meaning that 'end_sample' may be lower than 'start_sample'."
         ),
     )
-    speed_kph: condecimal(decimal_places=2) = Field(
+    speed_kph: float = Field(
         nullable=False,
         description="average speed across the road segment in km/h",
     )
-    air_temperature: condecimal(decimal_places=2) = Field(
+    air_temperature: float = Field(
         nullable=False,
         description="average air temperature across the road segment in deg C",
     )
-    speed_correction_db: condecimal(decimal_places=2) = Field(
+    speed_correction_db: float = Field(
         nullable=False,
         description="speed correction in dB",
     )
-    temperature_correction_db: condecimal(decimal_places=2) = Field(
+    temperature_correction_db: float = Field(
         nullable=False,
         description="temperature correction in dB",
     )
     start_latitude: float = Field(
         nullable=False,
         description="latitude of segment start point",
     )
@@ -590,24 +580,14 @@
 
     wheel_bay_details: List["SegmentWheelBayDetails"] = Relationship()
 
     @validator("start_m", "end_m", "length_m", pre=True)
     def round_1(cls, v):
         return round(v, 1) if v is not None else None
 
-    @validator(
-        "speed_kph",
-        "air_temperature",
-        "speed_correction_db",
-        "temperature_correction_db",
-        pre=True,
-    )
-    def round_2(cls, v):
-        return round(v, 2) if v is not None else None
-
 
 class SegmentWheelBayDetails(SQLModel, table=True):
     """
     Segment-level (results set) wheel bay details.
     """
 
     __tablename__ = "segment_wheel_bay_details"
@@ -635,45 +615,35 @@
         primary_key=True,
     )
     wheel_bay_name: Optional[str] = Field(
         default=None,
         primary_key=True,
         description="wheel bay name ('left' or 'right')",
     )
-    road_temperature: Optional[condecimal(decimal_places=2)] = Field(
+    road_temperature: Optional[float] = Field(
         default=None,
         description="Mean road surface temperature for the segment in °C)",
     )
-    tyre_temperature: Optional[condecimal(decimal_places=2)] = Field(
+    tyre_temperature: Optional[float] = Field(
         default=None,
         description="Mean tyre temperature for the segment in °C",
     )
-    laeq_db: Optional[condecimal(decimal_places=2)] = Field(
+    laeq_db: Optional[float] = Field(
         default=None,
         description="LAeq for the wheel bay in dB (no CPX corrections applied)",
     )
-    lcpx_db: Optional[condecimal(decimal_places=2)] = Field(
+    lcpx_db: Optional[float] = Field(
         default=None,
         description="LCPX for the wheel bay in dB",
     )
 
     microphone_details: List["SegmentMicrophoneDetails"] = Relationship()
     wheel_bay_third_octave_levels: List["WheelBayThirdOctaveLevels"] = Relationship()
     wheel_bay_texture_results: Optional[List["WheelBayTextureResults"]] = Relationship()
 
-    @validator(
-        "road_temperature",
-        "tyre_temperature",
-        "laeq_db",
-        "lcpx_db",
-        pre=True,
-    )
-    def round_2(cls, v):
-        return round(v, 2) if v is not None else None
-
 
 class SegmentMicrophoneDetails(SQLModel, table=True):
     """
     Segment-level (results set) microphone details.
     """
 
     __tablename__ = "segment_microphone_details"
@@ -710,25 +680,21 @@
         default=None,
         primary_key=True,
     )
     microphone_position: int = Field(
         primary_key=True,
         description="microphone position (1-6) as per ISO 11819-2:2017)",
     )
-    laeq_db: condecimal(decimal_places=2) = Field(
+    laeq_db: float = Field(
         nullable=False,
         description="LAeq for the microphone position in dB (no CPX corrections applied)",
     )
 
     microphone_third_octave_levels: List["MicrophoneThirdOctaveLevels"] = Relationship()
 
-    @validator("laeq_db", pre=True)
-    def round_2(cls, v):
-        return round(v, 2) if v is not None else None
-
 
 class MicrophoneThirdOctaveLevels(SQLModel, table=True):
     """
     One-third octave band sound pressure levels for each microphone position
     in the wheel bay, measured across one road segment.
     """
 
@@ -771,27 +737,23 @@
     microphone_position: int = Field(
         primary_key=True,
     )
     frequency_hz: condecimal(decimal_places=1) = Field(
         primary_key=True,
         description="one-third octave band centre frequency in Hz",
     )
-    leq_db: condecimal(decimal_places=2) = Field(
+    leq_db: float = Field(
         nullable=False,
         description="microphone Leq in dB across the road segment",
     )
-    laeq_db: condecimal(decimal_places=2) = Field(
+    laeq_db: float = Field(
         nullable=False,
         description="microphone LAeq in dB across the road segment",
     )
 
-    @validator("leq_db", "laeq_db", pre=True)
-    def round_2(cls, v):
-        return round(v, 2) if v is not None else None
-
 
 class WheelBayThirdOctaveLevels(SQLModel, table=True):
     __tablename__ = "wheel_bay_third_octave_levels"
     __table_args__ = (
         ForeignKeyConstraint(
             [
                 "measurement_id",
@@ -824,44 +786,40 @@
         default=None,
         primary_key=True,
     )
     frequency_hz: condecimal(decimal_places=1) = Field(
         primary_key=True,
         description="one-third octave band centre frequency in Hz",
     )
-    leq_db: condecimal(decimal_places=2) = Field(
+    leq_db: float = Field(
         nullable=False,
         description=(
             "energy-based average of the one-third octave Leq of all "
             "microphone positions within the enclosure in dB. Calculated by "
             "subtracting the A weighting from the one-third octave LAeq (see "
             "'laeq_db' field) for the wheel bay."
         ),
     )
-    laeq_db: condecimal(decimal_places=2) = Field(
+    laeq_db: float = Field(
         nullable=False,
         description=(
             "energy-based average of the one-third octave LAeq of all "
             "microphone positions within the enclosure in dB (refer ISO "
             "11819-2:2017 Formula C.1 / C.7)"
         ),
     )
-    lcpx_db: condecimal(decimal_places=2) = Field(
+    lcpx_db: float = Field(
         nullable=False,
         description=(
             "one-third octave LCPX with all corrections applied (including "
             "the device-related correction) in dB (refer ISO 11819-2:2017 "
             "Formula C.8 and C.9)"
         ),
     )
 
-    @validator("leq_db", "laeq_db", "lcpx_db", pre=True)
-    def round_2(cls, v):
-        return round(v, 2) if v is not None else None
-
 
 class WheelBayTextureResults(SQLModel, table=True):
 
     """
     Wheel bay texture results for each wheel bay in the enclosure.
     """
 
@@ -913,29 +871,25 @@
         description=(
             "laser sample number corresponding to the end of the road "
             "segment. This is the same side of the road segment as 'end_m', "
             "meaning that 'laser_end_sample' may be lower than "
             "'laser_start_sample'."
         ),
     )
-    mpd_mm: condecimal(decimal_places=3) = Field(
+    mpd_mm: float = Field(
         nullable=False,
         description=(
             "mean profile depth for road segment in mm, calculated from all "
             "valid mean segment depth results within the road segment"
         ),
     )
-    stdev_mm: condecimal(decimal_places=3) = Field(
+    stdev_mm: float = Field(
         nullable=False,
         description=(
             "standard deviation in mm of all valid mean segment depths within "
             "the road segment"
         ),
     )
     valid: bool = Field(
         nullable=False,
         description="validity of the mean profile depth result for the segment",
     )
-
-    @validator("mpd_mm", "stdev_mm", pre=True)
-    def round_3(cls, v):
-        return round(v, 3) if v is not None else None
```

