# Extinct Species in Berlin 

Extracting Berlin red list data from different published sources. 

[IUCN Red List](https://en.wikipedia.org/wiki/IUCN_Red_List) is an inventory of the global conservation status and extinction risk of species. As conservation status can vary between locations, extinction can be defined relative to the location in addition to the global red list, there are other red lists for geo-political areas. In the case of Germany, the [overall red list for Germany](https://www.rote-liste-zentrum.de/en/index.html) as well as the red lists for each state are available. While the country red lists are compiled in a singular format and available digitally, the lists for Berlin state are of varying structure and are only available as their initial research publication format (largely as pdf or in print). 

This project is an effort to extract specific information from a multitude of sources to form a singular list that reflects extinct species in Berlin. The data extraction process is made available so the final research outcomes can be reproducible.  

## Data Source

Main Source: 

[Species Lists – Red Lists of Endangered Plants, Animals and Fungi from Berlin](https://www.berlin.de/sen/uvk/natur-und-gruen/naturschutz/artenschutz/artenlisten-rote-listen/) / Artenlisten – Rote Listen der gefährdeten Pflanzen, Tiere und Pilze von Berlin

| #  | List Name   | Author/s    | Primary Link |  Secondary Link |
| -- | ----------- | ----------- | -----------  | --------------- |
| 01 | Rote Liste und Gesamtartenliste der Großschmetterlinge (Lepidoptera: Makrolepidoptera) von Berlin|             |              |                 |
| 02 | Rote Liste und Gesamtartenliste der Sackträger (Lepidoptera: Psychidae) von Berlin|  |||
| 03 |Rote Liste und Gesamtartenliste
der Libellen (Odonata) von Berlin |  |||
| 04 |Rote Liste und Gesamtartenliste der Heuschrecken und Grillen (Saltatoria: Ensifera et Caelifera) von Berlin|  |||
| 05 |Rote Liste und Gesamtartenliste
der Zikaden (Hemiptera: Fulgoromorpha
und Cicadomorpha) von Berlin|  |||
| 06 |Rote Liste und Gesamtartenliste der Kamelhalsfliegen, Schlammfliegen und Netzflügler (Raphidioptera, Megaloptera, Neuroptera) von Berlin|  |||
| 07 |Rote Liste und Gesamtartenliste der Bienen und Wespen (Hymenoptera part.) von Berlin mit Angaben zu den Ameisen|  |||
| 08 |Rote Liste und Gesamtartenliste der Köcherfliegen (Trichoptera) von Berlin|  |||
| 09 |Rote Liste und Gesamtartenliste der Schnabelfliegen (Mecoptera) von Berlin|  |||
| 10 | Rote Liste und Gesamtartenliste der Raubfliegen (Diptera: Asilidae) von Berlin|  |||
| 11 |Rote Liste und Gesamtartenliste der Eintagsfliegen (Ephemeroptera) von Berlin|  |||
| 12 |Rote Liste und Gesamtartenliste der Schwebfliegen (Diptera: Syrphidae) von Berlin|  |||
| 13 |Rote Liste und Gesamtartenliste der Wanzen (Heteroptera) von Berlin|  |||
| 14 |Rote Liste und Gesamtartenliste der Wasserkäfer (Coleoptera: Hydradephaga, Hydrophiloidea part., Hydraenidae, Elmidae und Dryopidae) von Berlin|  |||
| 15 |Rote Liste und Gesamtartenliste der Laufkäfer (Coleoptera: Carabidae) von Berlin|  |||
| 16 |Rote Liste und Gesamtartenliste der Prachtkäfer (Coleoptera: Buprestidae) von Berlin|  |||
| 17 |Rote Liste und Gesamtartenliste der Blattkäfer (Chrysomelidae und Megalopodidae) von Berlin|  |||
| 18 |Rote Liste und Gesamtartenliste der Blatthornkäfer (Coleoptera: Scarabaeoidea) von Berlin|  |||
| 19 |Rote Liste und Gesamtartenliste der Kurzflügelkäferartigen und Stutzkäfer (Coleoptera: Staphylinoidea und Histeridae) von Berlin|  |||
| 20 |Rote Liste und Gesamtartenliste der Kapuzinerkäferartigen (Bostrichoidea), Buntkäferartigen (Cleroidea), Plattkäferartigen (Cucujoidea), Schnellkäferartigen (Elateroidea), Werftkäferartigen (Lymexyloidea) und Schwarzkäferartigen (Tenebrioidea) von Berlin (Coleoptera)|  |||
| 21 |Rote Liste und Gesamtartenliste der Bockkäfer (Coleoptera: Cerambycidae) von Berlin|  |||
| 22 |Rote Liste und Gesamtartenliste der Rüsselkäfer (Curculionoidea) von Berlin|  |||
| 23 |Rote Liste und Gesamtartenliste der Spinnen (Araneae) und Gesamtartenliste der Weberknechte (Opiliones) von Berlin|  |||
| 24 |Rote Liste und Gesamtartenliste der Weichtiere (Mollusca: Gastropoda und Bivalvia) von Berlin|  |||
| 25 |Gesamtartenliste und Rote Liste der Fische und Neunaugen (Pisces et Cyclostomata) von Berlin|  |||
| 26 |Rote Liste und Gesamtartenliste der Kriechtiere (Reptilia) von Berlin|  |||
| 27 |Rote Liste und Gesamtartenliste der Lurche (Amphibia) von Berlin|  |||
| 28 |Rote Liste und Liste der Brutvögel (Aves) von Berlin|  |||
| 29 |Rote Liste und Gesamtartenliste der Säugetiere (Mammalia) von Berlin|  |||
| 30 |Rote Liste und Gesamtartenliste der etablierten Farn- und Blütenpflanzen von Berlin|  |||
| 31 |Rote Liste und Gesamtartenliste der Moose (Bryophyta) von Berlin|  |||
| 32 |Rote Liste und Gesamtartenliste der Flechten (Lichenes) von Berlin|  |||
| 33 |Rote Liste und Gesamtartenliste der Röhrlinge s. l. (Boletales) von Berlin|  |||
| 34 |Rote Liste und Gesamtartenliste der flechtenbewohnenden (lichenicolen) Pilze von Berlin|  |||
| 35 |Rote Liste und Gesamtartenliste der Brandpilze (Ustilaginales) von Berlin|  |||
| 36 |Rote Liste und Gesamtartenliste der Armleuchteralgen (Characeae) von Berlin|  |||
| 37 |Rote Liste und Gesamtartenliste der limnischen Rotalgen (Rhodophyta) und Braunalgen (Phaeophyceae) von Berlin|  |||

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
