# Extinct Species in Berlin 

Extracting Berlin red list data from different published sources. 

[IUCN Red List](https://en.wikipedia.org/wiki/IUCN_Red_List) is an inventory of the global conservation status and extinction risk of species. As conservation status can vary between locations, extinction can be defined relative to the location in addition to the global red list, there are other red lists for geo-political areas. In the case of Germany, the [overall red list for Germany](https://www.rote-liste-zentrum.de/en/index.html) as well as the red lists for each state are available. While the country red lists are compiled in a singular format and available digitally, the lists for Berlin state are of varying structure and are only available as their initial research publication format (largely as pdf or in print). 

This project is an effort to extract specific information from a multitude of sources to form a singular list that reflects extinct species in Berlin. The data extraction process is made available so the final research outcomes can be reproducible.  

## Data Source

Main Source: 

[Species Lists – Red Lists of Endangered Plants, Animals and Fungi from Berlin](https://www.berlin.de/sen/uvk/natur-und-gruen/naturschutz/artenschutz/artenlisten-rote-listen/) / Artenlisten – Rote Listen der gefährdeten Pflanzen, Tiere und Pilze von Berlin

| #  | List Name   | Author/s    | Primary Link |  Secondary Link |
| -- | ----------- | ----------- | -----------  | --------------- |
| 01 |        |  |||
| 02 |         |  |||
| 03 |        |  |||
| 04 |         |  |||
| 05 |        |  |||
| 06 |         |  |||
| 07 |        |  |||
| 08 |         |  |||
| 09 |        |  |||
| 10 |         |  |||
| 11 |        |  |||
| 12 |         |  |||
| 13 |        |  |||
| 14 |         |  |||
| 15 |        |  |||
| 16 |         |  |||

## Development steps:

1. EDA -  **DONE**
2. Data Extraction - **DONE**
3. Raw data transformation - Transformation step 1  - **DONE**
4. Adding taxonomy backbone - Transformation step 2 - **DONE**
5. ~~Addng metadata table - Transformation step 3~~
6. Extinct species concatenated data list - Transformation step 4 - **DONE**
7. Basic README - **DONE**
8. Publishing the transformation process - **HERE**
9. Publishing references
10. How to reproduce the process - documentation v1
11. Moving transformation to Databricks
12. How to reproduce the process - documentation v2

## Tools and libraries

* Python
* Pandas
* NumPy
* Camelot
* PyGBIF
* Xmind
* Potentially: Databricks, Google Drive

## How to setup
