# Week 3 Data Preparation Note

## Study Area

This week's data preparation focused on preparing the Ogun State study area boundary for analysis in QGIS.

## Coordinate Reference System

The final dataset was reprojected to **WGS 84 / UTM Zone 31N (EPSG:32631)**.

This projected coordinate reference system was selected because Ogun State falls within UTM Zone 31N. It uses metres as the coordinate unit and is suitable for spatial analysis within the study area.

## Reprojection and Clipping

The Ogun State boundary was reprojected from its original coordinate reference system to **EPSG:32631**.

The boundary was clipped/prepared to represent the Ogun State study area.

The final analysis-ready dataset is stored in:

`data/Ogun_Boundary_UTM31N.gpkg`

The GeoPackage contains the layer:

`ogun`

## Quality Checks

### 1. CRS Check

The final dataset was checked and confirmed to use **WGS 84 / UTM Zone 31N (EPSG:32631)**.

**Result:** Passed. No CRS issue was found.

### 2. Geometry Validity Check

The final dataset was checked for geometry validity.

**Result:**

* Valid features: 1
* Invalid features: 0
* Geometry errors: 0

No geometry repair was required.

### 3. Duplicate Geometry Check

The dataset was checked for duplicate geometries.

**Result:** No duplicate geometries were identified. No features were removed.

### 4. Missing Attribute Check

The attribute table was reviewed for NULL or empty values.

Some optional metadata fields contained NULL values, including administrative name, validity and language fields. However, no important field required for the analysis contained missing values.

**Decision:** The optional NULL values were flagged but did not require correction because they do not affect the intended analysis.

### 5. Spatial Extent Check

The final dataset was checked against the Ogun State study area boundary.

**Result:** The dataset is contained within the Ogun State study area, with no features extending outside the required boundary.

No correction was required.

## Analysis-Ready File

**File:** `data/Ogun_Boundary_UTM31N.gpkg`

**Layer:** `ogun`

**CRS:** EPSG:32631 — WGS 84 / UTM Zone 31N
