# Week 2 Data Note

## Dataset 1: Nigeria Administrative Boundaries

**Source:** DIVA GIS

**Source link:** https://geodata.ucdavis.edu/diva/adm/NGA_adm.zip

**Number of features:** 37

**Geometry type:** Polygon

**Key columns:** `ID_0`, `ISO`, `NAME_0`, `ID_1`, `NAME_1`, `TYPE_1`, `ENGTYPE_1`

**Gaps or missing values:** `NL_NAME_1` and `VARNAME_1` contain some missing (`NULL`) values.

**Purpose:** This dataset contains Nigeria's administrative boundaries at the state level, including the 36 states and the Federal Capital Territory. It is used to identify and define Ogun State as the study area and support the spatial analysis for the project.

---

## Dataset 2: Waterways

**Source:** OpenStreetMap (OSM), downloaded using the QuickOSM plugin in QGIS.

**Source link:** https://www.openstreetmap.org/

**Number of features:** 144

**Geometry type:** LineString

**Key columns:** `osm_id`, `osm_type`, `waterway`, `name_yo`, `width`, `seasonal`, `tidal`, `name`

**Gaps or missing values:** Some attribute fields contain missing values, particularly `name`, `width`, `seasonal`, and `tidal`. This is because not all mapped waterways have complete attribute information in OpenStreetMap.

**Purpose:** This dataset contains mapped waterways within the study area. It will be used to identify and represent water features and support the spatial interpretation of land use and land cover patterns in Ogun State.
