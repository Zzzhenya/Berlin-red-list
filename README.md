# Extinct Species in Berlin 

Extracting Berlin red list data from different published sources. 

[IUCN Red List](https://en.wikipedia.org/wiki/IUCN_Red_List) is an inventory of the global conservation status and extinction risk of species. As conservation status can vary between locations, extinction can be defined relative to the locality as well. Because of this, there are other red lists for geo-political areas. In the case of Germany, the [overall red list for Germany](https://www.rote-liste-zentrum.de/en/index.html) as well as the red lists for each state are available. While the country red lists are compiled in a singular format and available digitally, the lists for Berlin state are of varying structure and are only available as their initial research publication format (either as pdf or in print). 

This project is an effort to extract species data from multiple sources to form a singular list that reflects extinct species in Berlin. The data extraction process is made available so the final research outcomes are reproducible.  

## Data Transformation Process

![](https://github.com/Zzzhenya/Berlin-red-list/blob/main/Data_transformation_process.jpg)

## Tools and libraries

* Python
* Pandas
* NumPy
* Camelot
* PyGBIF
* Xmind
* Potentially: Databricks, Google Drive

## How to setup

Setting up dependencies with uv and pyproject.toml

1. Clone the repository and move to folder

```
git clone https://github.com/Zzzhenya/Berlin-red-list.git
cd Berln-red-list
```

![2. Install uv](https://docs.astral.sh/uv/getting-started/installation/)

`pip install uv`

3. Install dependencies and open Jupyter notebooks

`uv run Jupyter lab`


## Development steps:

1. EDA -  **DONE**
2. Data Extraction - **DONE**
3. Raw data transformation - Transformation step 1  - **DONE**
4. Adding taxonomy backbone - Transformation step 2 - **DONE**
5. ~~Addng metadata table - Transformation step 3~~
6. Extinct species concatenated data list - Transformation step 4 - **DONE**
7. Basic README - **DONE**
8. Updating the transformation process for Makrolepidoptera - **HERE**
9. Publishing the transformation process - **DONE**
10. Publishing references **DONE**
11. How to reproduce the process - documentation v1 **DONE**
12. Moving transformation to Databricks
13. How to reproduce the process - documentation v2

## Data Source

Main Source: 

[Species Lists – Red Lists of Endangered Plants, Animals and Fungi from Berlin](https://www.berlin.de/sen/uvk/natur-und-gruen/naturschutz/artenschutz/artenlisten-rote-listen/) / Artenlisten – Rote Listen der gefährdeten Pflanzen, Tiere und Pilze von Berlin



| #  | List Name   | Author/s    | Link |
| -- | ----------- | ----------- | -----------  |
| 01 |Rote Liste und Gesamtartenliste der Großschmetterlinge (Lepidoptera: Makrolepidoptera) von Berlin |Jörg Gelbrecht, Alessandro Kormannshaus, Bernd Krüger, Fred Ockruck, Bernd Schulze, Franz Theimer, Peter Weisbach, Hubert Woelky, Otfried Woelky & Michael Woelky|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote-liste-und-gesamtartenliste-der-grossschmetterlinge-berlins.pdf)|
| 02 |Rote Liste und Gesamtartenliste der Sackträger (Lepidoptera: Psychidae) von Berlin|Michael Weidlich|[Link](https://www.zobodat.at/pdf/Maerkische-Ent-Nachr_SH_7_0109-0122.pdf)|
| 03 |Rote Liste und Gesamtartenliste der Libellen (Odonata) von Berlin|Falk Petzold unter Mitarbeit von Peter Jahn|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_libellen_petzold.pdf)|
| 04 |Rote Liste und Gesamtartenliste der Heuschrecken und Grillen (Saltatoria: Ensifera et Caelifera) von Berlin|Bernd Machatzi, Andreas Ratsch, Rüdiger Prasse & Michael Ristow|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/16_heuschreck_print.pdf)|
| 05 |Rote Liste und Gesamtartenliste der Zikaden (Hemiptera: Fulgoromorpha und Cicadomorpha) von Berlin|Herbert Nickel & Roland Mühlethaler|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_zikaden_nickel_muehletaler.pdf)|
| 06 |Rote Liste und Gesamtartenliste der Kamelhalsfliegen, Schlammfliegen und Netzflügler (Raphidioptera, Megaloptera, Neuroptera) von Berlin|Christoph Saure|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/18_netzfl_print.pdf)|
| 07 |Rote Liste und Gesamtartenliste der Bienen und Wespen (Hymenoptera part.) von Berlin mit Angaben zu den Ameisen|Christoph Saure unter Mitarbeit von Thomas Ziska|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/24_bienen_print.pdf)|
| 08 |Rote Liste und Gesamtartenliste der Köcherfliegen (Trichoptera) von Berlin|Reinhard Müller & Wolfram Mey|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_koecherfliegen_mueller_mey.pdf)|
| 09 |Rote Liste und Gesamtartenliste der Schnabelfliegen (Mecoptera) von Berlin|Christoph Saure|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/26_schnabelfl_print.pdf?ts=1657265339)|
| 10 | Rote Liste und Gesamtartenliste der Raubfliegen (Diptera: Asilidae) von Berlin|Günter Degen|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_raubfliegen_degen.pdf?ts=1657265396)|
| 11 |Rote Liste und Gesamtartenliste der Eintagsfliegen (Ephemeroptera) von Berlin|Reinhard Muller|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_eintagsfliegen_mueller.pdf?ts=1657265418)|
| 12 |Rote Liste und Gesamtartenliste der Schwebfliegen (Diptera: Syrphidae) von Berlin|Christoph Saure|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_schwebfliegen_saure.pdf?ts=1657265397)|
| 13 |Rote Liste und Gesamtartenliste der Wanzen (Heteroptera) von Berlin|Jürgen Deckert & Gerhard Burghardt|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/17_wanzen_print.pdf?ts=1657265362)|
| 14 |Rote Liste und Gesamtartenliste der Wasserkäfer (Coleoptera: Hydradephaga, Hydrophiloidea part., Hydraenidae, Elmidae und Dryopidae) von Berlin|Lars Hendrich & Reinhard Müller|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_wasserkaefer_hendrich_mueller.pdf?ts=1657265366)|
| 15 |Rote Liste und Gesamtartenliste der Laufkäfer (Coleoptera: Carabidae) von Berlin|Karl-Hinrich Kielhorn|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/19_laufkaefer_print.pdf?ts=1657265406)|
| 16 |Rote Liste und Gesamtartenliste der Prachtkäfer (Coleoptera: Buprestidae) von Berlin|Stephan Gottwald|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_prachtkaefer_gottwald.pdf?ts=1657265374)|
| 17 |Rote Liste und Gesamtartenliste der Blattkäfer (Chrysomelidae und Megalopodidae) von Berlin|Uwe Heinig & Matthias Schöller unter Mitarbeit von Ulf Arnold, Jens Esser, Lars Hendrich, Hella Wendt und Herbert Winkelmann|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_blattkaefer_heinig_schoeller.pdf?ts=1657265376)|
| 18 |Rote Liste und Gesamtartenliste der Blatthornkäfer (Coleoptera: Scarabaeoidea) von Berlin|Jens Esser|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_blatthornkaefer_esser.pdf?ts=1657265365)|
| 19 |Rote Liste und Gesamtartenliste der Kurzflügelkäferartigen und Stutzkäfer (Coleoptera: Staphylinoidea und Histeridae) von Berlin|Jens Esser|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_kurzflueglerartige_esser.pdf?ts=1657265399)|
| 20 |Rote Liste und Gesamtartenliste der Kapuzinerkäferartigen (Bostrichoidea), Buntkäferartigen (Cleroidea), Plattkäferartigen (Cucujoidea), Schnellkäferartigen (Elateroidea), Werftkäferartigen (Lymexyloidea) und Schwarzkäferartigen (Tenebrioidea) von Berlin (Coleoptera)|Jens Esser|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_kurzflueglerartige_esser.pdf?ts=1657265399)|
| 21 |Rote Liste und Gesamtartenliste der Bockkäfer (Coleoptera: Cerambycidae) von Berlin|Jens Esser|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_bockkaefer_esser.pdf?ts=1657265364)|
| 22 |Rote Liste und Gesamtartenliste der Rüsselkäfer (Curculionoidea) von Berlin|Christoph Bayer & Herbert Winkelmann|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/23_ruesselk_print.pdf?ts=1657265359)|
| 23 |Rote Liste und Gesamtartenliste der Spinnen (Araneae) und Gesamtartenliste der Weberknechte (Opiliones) von Berlin|Ulrike Kielhorn|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_spinnen_kielhorn.pdf?ts=1649931234)|
| 24 |Rote Liste und Gesamtartenliste der Weichtiere (Mollusca: Gastropoda und Bivalvia) von Berlin|Eva Hackenberg & Reinhard Müller|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_mollusken_hackenberg_mueller.pdf?ts=1674578488)|
| 25 |Gesamtartenliste und Rote Liste der Fische und Neunaugen (Pisces et Cyclostomata) von Berlin||[Link](https://www.berlin.de/fischereiamt/_assets/service/pdf/flyer_richtiges_fischen_text.pdf?ts=1673255017)|
| 26 |Rote Liste und Gesamtartenliste der Kriechtiere (Reptilia) von Berlin|Klaus-Detlef Kühnel, Jens Scharon, Beate Kitzmann & Beate Schonert unter Mitarbeit von Daniel Bohle|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_reptilien_kuehnel_et_al.pdf?ts=1649931234)|
| 27 |Rote Liste und Gesamtartenliste der Lurche (Amphibia) von Berlin|Klaus-Detlef Kühnel, Jens Scharon, Beate Kitzmann & Beate Schonert unter Mitarbeit von Angele Schonert (†)|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_amphibien_kuehnel_et_al.pdf?ts=1649931234)|
| 28 |Rote Liste und Liste der Brutvögel (Aves) von Berlin|Klaus Witt & Klemens Steiof|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_brutvoegel_witt_steiof.pdf?ts=1649931234)|
| 29 |Rote Liste und Gesamtartenliste der Säugetiere (Mammalia) von Berlin|Jürgen Klawitter, Rainer Altenkamp, Carsten Kallasch, Dieter Köhler, Manfred Krauß, Susanne Rosenau & Tobias Teige|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/10_saeuge_print.pdf?ts=1649931234)|
| 30 |Rote Liste und Gesamtartenliste der etablierten Farn- und Blütenpflanzen von Berlin|Birgit Seitz, Michael Ristow, Justus Meißner, Bernd Machatzi, Herbert Sukopp|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/09_gefaesspflanzen.pdf?ts=1649931234)|
| 31 |Rote Liste und Gesamtartenliste der Moose (Bryophyta) von Berlin|Jürgen Klawitter & Hanna Köstler|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_moose_klawitter_koestler.pdf?ts=1649931234)|
| 32 |Rote Liste und Gesamtartenliste der Flechten (Lichenes) von Berlin|Josephin Krause, Hans-Georg Wagner & Volker Otte|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_flechten_krause_et_al.pdf?ts=1649931234)|
| 33 |Rote Liste und Gesamtartenliste der Röhrlinge s. l. (Boletales) von Berlin|Martin Schmidt unter Mitarbeit von Mitgliedern der Pilzkundlichen Arbeitsgemeinschaft Berlin-Brandenburg e.V. (PABB) und der Interessengemeinschaft Märkischer Mykologen (IMM)|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_roehrlinge_schmidt.pdf?ts=1649931234)|
| 34 |Rote Liste und Gesamtartenliste der flechtenbewohnenden (lichenicolen) Pilze von Berlin|Hans-Georg Wagner, Josephin Krause & Volker Otte|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_flechtenpilze_wagner_et_al.pdf?ts=1649931234)|
| 35 |Rote Liste und Gesamtartenliste der Brandpilze (Ustilaginales) von Berlin|Hildemar Scholz & Ilse Scholz|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/06_brandpilze_print.pdf?ts=1649931234)|
| 36 |Rote Liste und Gesamtartenliste der Armleuchteralgen (Characeae) von Berlin|Wolf-Henning Kusber, Regine Jahn & Heiko Korsch|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_armleuchteralgen_kusber_et_al.pdf?ts=1649931234)|
| 37 |Rote Liste und Gesamtartenliste der limnischen Rotalgen (Rhodophyta) und Braunalgen (Phaeophyceae) von Berlin|Klaus Rudolph, Regine Jahn & Wolf-Henning Kusber|[Link](https://www.berlin.de/sen/uvk/_assets/natur-gruen/naturschutz/artenschutz/rote-listen/rote_liste_rotalgen_rudolph_et_al.pdf?ts=1649931234)|
