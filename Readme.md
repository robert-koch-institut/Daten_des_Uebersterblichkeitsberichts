

<!-- HEADER_START: {"lang": "de"} -->


Dokumentation  

# Daten des Übersterblichkeitsberichts

<br> 
<br> 
<br> 

[**Robert Koch-Institut**](https://www.rki.de/)&sup1;

<br> 

**Beitragende**   
[Benedikt Zacher](https://orcid.org/0000-0002-6107-6389)&sup2;, [Andreas Hicketier](https://orcid.org/0009-0000-5882-852X)&sup2;, [Alexander Ullrich](https://orcid.org/0000-0002-4894-6124)&sup2;, [Michaela Diercke](https://orcid.org/0000-0002-4678-1813)&sup2;, & [Matthias an der Heiden](https://orcid.org/0000-0001-5863-4549)&sup3;

&emsp;&emsp;&sup1; [Bundesministerium für Gesundheit (BMG)](https://www.bundesgesundheitsministerium.de/)  
&emsp;&emsp;&sup2; [Robert Koch-Institut](https://www.rki.de/) | [Fachgebiet 32](https://www.rki.de/fg32)  
&emsp;&emsp;&sup3; [Robert Koch-Institut](https://www.rki.de/) | [Fachgebiet 34](https://www.rki.de/fg34)

<br> 

**Zitieren**  
Robert Koch-Institut. (2026). Daten des Übersterblichkeitsberichts [Data set]. Zenodo. [https://doi.org/10.5281/zenodo.18607445](https://doi.org/10.5281/zenodo.18607445)

<br>


**Zusammenfassung**    
Im Datensatz "Daten des Übersterblichkeitsberichts" des Robert Koch-Instituts werden wöchentliche Daten zur Übersterblichkeit in Deutschland bereitgestellt. Der Datensatz enthält Angaben zum Wochendatum und zur jeweiligen Gruppe (z. B. Altersgruppen, Geschlecht oder Region). Für jede Gruppe wird die beobachtete Sterbefallzahl den modellbasiert erwarteten Sterbefallzahlen gegenübergestellt.Zur Bewertung von Abweichungen zwischen beobachteter und erwarteter Sterbefallzahl wird der z-Score berechnet, der zur Einordnung einer etwaigen Übersterblichkeit genutzt wird. Der Datensatz dient der kontinuierlichen Überwachung von Sterbefallzahlen in Deutschland und ermöglicht die frühzeitige Erkennung von ungewöhnlich hohen Sterbefallzahlen in den betrachteten Gruppen.

<br>

**Inhaltsverzeichnis**  

<!-- TOC_START: {"heading_depth": 2} -->
  - [Informationen zum Datensatz und Entstehungskontext](#informationen-zum-datensatz-und-entstehungskontext)  
  - [Aufbau und Inhalt des publizierten Datensatzes](#aufbau-und-inhalt-des-publizierten-datensatzes)  
  - [Hinweise zur Nachnutzung der Daten](#hinweise-zur-nachnutzung-der-daten)  
<!-- TOC_END -->

<br>

<!-- HEADER_END -->

## Informationen zum Datensatz und Entstehungskontext  

Ereignisse wie Infektionswellen oder Hitzeperioden führen regelmäßig zu kurzfristigen Anstiegen der Sterbefallzahlen in Deutschland. Wenn die Zahl der Sterbefälle im Vergleich zur erwarteten Sterbefallzahl deutlich erhöht ist, wird von Übersterblichkeit gesprochen.

Im Rahmen der Mortalitätssurveillance werden nach § 5b BevStatG dieser Datensatz sowie ein Bericht zur Einordnung veröffentlicht. Wie ermöglichen eine zeitnahe Einschätzung der aktuellen Sterbefallzahlen in Deutschland. Der Datensatz wird wöchentlich aktualisiert, um fortlaufend über die aktuelle Lage zur Sterbefallzahlen und Übersterblichkeit zu informieren. 

Der Bericht zur Übersterblichkeit in Deutschland ist verfügbar unter:    

> Robert Koch-Institut. (2025). Bericht zur Übersterblichkeit in Deutschland. Zenodo. [https://doi.org/10.5281/zenodo.17608501](https://doi.org/10.5281/zenodo.17608501)


### Administrative und organisatorische Angaben  

Die zugrundeliegenden Daten für die Mortalitätssurveillance gemäß § 5b Bevölkerungsstatistikgesetz (BevStatG) werden vom [Statistischen Bundesamt (Destatis)](https://www.destatis.de) an das [Robert Koch-Institut (RKI)](https://www.rki.de) übermittelt. Die Konzeption und Durchführung der Analysen erfolgen im [Fachgebiet 32 | Surveillance und elektronisches Melde- und Informationssystem (DEMIS) | ÖGD-Kontaktstelle](https://www.rki.de/fg32) des RKI.

Die Veröffentlichung der aufbereiteten und validierten Daten, die Kuration der Datensätze sowie das Qualitätsmanagement der Metadaten werden durch das Fachgebiet [MF 4 | Fach- und Forschungsdatenmanagement](https://www.rki.de/mf4) des RKI verantwortet. Fragen zum Datenmanagement oder zu den offenen Datensätzen können an das Open-Data-Team des Fachgebiets MF 4 unter [OpenData@rki.de](mailto:OpenData@rki.de) gerichtet werden.



### Datenerhebung und Datenauswertung

Gemäß § 5b des BevStatG übermittelt Destatis dem RKI für epidemiologische Analysen einer überdurchschnittlichen Sterblichkeit Einzelangaben zu jedem registrierten Sterbefall. Diese Angaben umfassen das Geschlecht, Jahr und Monat der Geburt, den Sterbetag, die Anschrift des Sterbeortes, den Landkreis bzw. die kreisfreie Stadt der letzten Meldung sowie das zuständige Standesamt, das den Sterbefall registriert hat. Die Datengrundlage dieses Übersterblichkeitsberichts entspricht derjenigen des Sterbefallmonitorings des Statistischen Bundesamts.

Es werden zwei statistische Verfahren für die Analyse angewendet: die Hochrechnung der Fallzahlen (Nowcasting) und die Übersterblichkeitsanalyse.

Da Sterbefallmeldungen zeitverzögert eingehen, wird ein Schätzverfahren eingesetzt, um die endgültigen Fallzahlen einer Sterbewoche frühzeitig zu prognostizieren. Hierzu wird ein generalisiertes lineares quasi-Poisson-Modell verwendet, das den Zusammenhang zwischen bereits gemeldeten und endgültigen Fallzahlen beschreibt. Das Modell berücksichtigt Zeittrends im Meldeverhalten sowie Feiertagseffekte und wird auf historischen Daten trainiert. 

Zur Identifikation von Phasen erhöhter Sterblichkeit werden Hidden Markov Modelle eingesetzt, die zwischen einem normalen Sterblichkeitsniveau und verschiedenen Zuständen erhöhter Sterblichkeit unterscheiden. Das Modell beinhaltet ein generalisiertes linearen Modell, das die erwartete Sterbefallzahl unter Berücksichtigung von Saisonalität und Zeittrends schätzt. Anschließend ein z-Score berechnet, analog zur Methodik von [EuroMOMO](https://www.euromomo.eu/), wodurch internationale Vergleichbarkeit gewährleistet ist.

Die zugrundeliegende Methodik ist als Open Source R-Paket [excode auf github](https://github.com/robert-koch-institut/excode) und Zenodo verfügbar.

> Zacher, B., & Vietor, A. (2025). excode: Excess Count Detection in Epidemiological Time Series. Zenodo. [https://doi.org/10.5281/zenodo.17417083](https://doi.org/10.5281/zenodo.17417083)



## Aufbau und Inhalt des publizierten Datensatzes

Der Datensatz enthält wöchentliche Informationen zur Sterblichkeit in Deutschland. Jede Zeile beschreibt eine Kombination aus Wochendatum und Gruppe (z. B. Altersgruppe, Geschlecht oder Region). Es werden die beobachtete Sterbefallzahl, die erwartete Sterbefallzahl sowie der daraus abgeleitete z-Score angegeben. Ergänzend wird angegeben, ob es sich um hochgerechnete Werte handelt.


#### Variablen und Variablenausprägungen

<!-- DATA_SCHEMA_SPECIFICATION_START: {"id": "daten_uebersterblichkeitsbericht", "lang": "de"} -->

Die Datei [daten_uebersterblichkeitsbericht.tsv](https://github.com/robert-koch-institut/Daten_des_Uebersterblichkeitsberichts/blob/main/daten_uebersterblichkeitsbericht.tsv) enthält die in der folgenden Tabelle abgebildeten Variablen und deren Ausprägungen. Ein maschinenlesbares Datenschema ist im [Data Package Standard](https://datapackage.org/) in [tableschema_daten_uebersterblichkeitsbericht.json](https://github.com/robert-koch-institut/Daten_des_Uebersterblichkeitsberichts/blob/main/Metadaten/schemas/tableschema_daten_uebersterblichkeitsbericht.json) hinterlegt:
> [tableschema_daten_uebersterblichkeitsbericht.json](https://github.com/robert-koch-institut/Daten_des_Uebersterblichkeitsberichts/blob/main/Metadaten/schemas/tableschema_daten_uebersterblichkeitsbericht.json)

<!-- DATA_SCHEMA_TABLE_START -->
| Variable                  | Typ     | Ausprägungen                                                                                                                                                                       | Beschreibung                                                                                                                                     |
|:--------------------------|:--------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------|
| Wochendatum               | date    | Format: `YYYY-MM-DD`<br>Fehlende Werte:<br>`NA`                                                                                                                                    | Datum (Sonntag) der Sterbewoche                                                                                                                  |
| Gruppe                    | string  | Werte:<br>`0-14 Jahre`, `15-44 Jahre`, `45-64 Jahre`, `65-74 Jahre`, `75-84 Jahre`, `85+ Jahre`, `Alten- und Pflegeheime`, …<br>Beispiel: `45-64 Jahre`<br>Fehlende Werte:<br>`NA` | Stratifizierung nach Region (Deutschland, Bundesländer), Altersgruppen und Sterbeort (Krankenhäuser, Alten- und Pfelgeheime und andere Adressen) |
| Sterbefallzahl            | integer | Werte: `≥0`<br>Beispiel: `2032`<br>Fehlende Werte:<br>`NA`                                                                                                                         | Anzahl der Verstorbenen in der jeweiligen Woche und Gruppe                                                                                       |
| Erwartete_Sterbefahllzahl | number  | Werte: `≥0`<br>Beispiel: `2109.17949033554`<br>Fehlende Werte:<br>`NA`                                                                                                             | Erwartete Anzahl der Verstorbenen in der jeweiligen Woche und Gruppe                                                                             |
| zscore                    | number  | Beispiel: `-1.23644832483487`<br>Fehlende Werte:<br>`NA`                                                                                                                           | Der z-score gibt an, wie weit ein Wert vom Durchschnitt entfernt ist, gemessen in Standardabweichungen.                                          |
| Hochrechnung              | string  | Werte:<br>`ja`, `nein`<br>Beispiel: `nein`<br>Fehlende Werte:<br>`NA`                                                                                                              | "ja" falls die Sterbefallzahl hochgerechnet, also für den Meldeverzug korrigiert, wurde. "nein" andernfalls.                                     |

<!-- DATA_SCHEMA_TABLE_END -->

<!-- DATA_SCHEMA_SPECIFICATION_END -->

### Formatierung
Die Daten sind im Datensatz als Tab-separierte .tsv-Datei enthalten. Der verwendete Zeichensatz ist UTF-8.  

* Zeichensatz: UTF-8  
* .tsv-Trennzeichen: Tab \"\\t\"  


<!-- FOOTER_START: {"lang": "de"} -->



### Metadaten  

Zur Erhöhung der Auffindbarkeit sind die bereitgestellten Daten mit Metadaten beschrieben. Über GitHub Actions werden Metadaten an die entsprechenden Plattformen verteilt. Für jede Plattform existiert eine spezifische Metadatendatei, diese sind im Metadatenordner hinterlegt:  

> [Metadaten/](https://github.com/robert-koch-institut/Daten_des_Uebersterblichkeitsberichts/tree/main/Metadaten/) 

Versionierung und DOI-Vergabe erfolgt über [Zenodo.org](https://zenodo.org). Die für den Import in Zenodo bereitgestellten Metadaten sind in der [zenodo.json](https://github.com/robert-koch-institut/Daten_des_Uebersterblichkeitsberichts/blob/main/Metadaten/zenodo.json) hinterlegt. Die Dokumentation der einzelnen Metadatenvariablen ist unter https://developers.zenodo.org/#representation nachlesbar.
 
> [Metadaten/zenodo.json](https://github.com/robert-koch-institut/Daten_des_Uebersterblichkeitsberichts/blob/main/Metadaten/zenodo.json)  

In der zenodo.json ist neben dem Publikationsdatum (`"publication_date"`) auch der Datenstand in folgendem Format enthalten (Beispiel):  

```
  "dates": [
    {
      "start": "2023-09-11T15:00:21+02:00",
      "end": "2023-09-11T15:00:21+02:00",
      "type": "Created",
      "description": "Date when the published data was created"
    }
  ],
```    


Zusätzlich beschreiben wir tabellarische Daten mithilfe des [Data Package Standards](https://datapackage.org/).
Ein Data Package ist eine strukturierte Sammlung von Daten und zugehörigen Metadaten, die den Austausch und die Wiederverwendung von Daten erleichtert. Es besteht aus einer datapackage.json-Datei, die zentrale Informationen wie die enthaltenen Ressourcen, ihre Formate und Schema-Definitionen beschreibt.

Der Data Package Standard wird von der [Open Knowledge Foundation](https://okfn.org/) bereitgestellt und ist ein offenes Format, das eine einfache, maschinenlesbare Beschreibung von Datensätzen ermöglicht.

Die Liste der in diesem Repository enthaltenen Daten ist in folgender Datei hinterlegt:

> [datapackage.json](https://github.com/robert-koch-institut/Daten_des_Uebersterblichkeitsberichts/tree/main/datapackage.json)

Für tabellarische Daten definieren wir zusätzlich ein [Table Schema](https://datapackage.org/standard/table-schema/), das die Struktur der Tabellen beschreibt, einschließlich Spaltennamen, Datentypen und Validierungsregeln. Diese Schema-Dateien finden sich unter:

> [Metadaten/schemas/](https://github.com/robert-koch-institut/Daten_des_Uebersterblichkeitsberichts/tree/main/Metadaten/schemas) 



## Hinweise zur Nachnutzung der Daten  

Offene Forschungsdaten des RKI werden auf [Zenodo.org](http://Zenodo.org/), [GitHub.com](http://GitHub.com/), [OpenCoDE](https://gitlab.opencode.de) und [Edoc.rki.de](http://Edoc.rki.de/) bereitgestellt:  

- https://zenodo.org/communities/robertkochinstitut  
- https://github.com/robert-koch-institut  
- https://gitlab.opencode.de/robert-koch-institut  
- https://edoc.rki.de/  


 
### Lizenz  

Der Datensatz "Daten des Übersterblichkeitsberichts" ist lizenziert unter der [Creative Commons Namensnennung 4.0 International Public License | CC-BY 4.0 International](https://creativecommons.org/licenses/by/4.0/deed.de).  

Die im Datensatz bereitgestellten Daten sind, unter Bedingung der Namensnennung des Robert Koch-Instituts als Quelle, frei verfügbar. Das bedeutet, jede Person hat das Recht die Daten zu verarbeiten und zu verändern, Derivate des Datensatzes zu erstellen und sie für kommerzielle und nicht kommerzielle Zwecke zu nutzen. Weitere Informationen zur Lizenz finden sich in der [LICENSE](https://github.com/robert-koch-institut/Daten_des_Uebersterblichkeitsberichts/blob/main/LICENSE) bzw. [LIZENZ](https://github.com/robert-koch-institut/Daten_des_Uebersterblichkeitsberichts/blob/main/LIZENZ) Datei des Datensatzes.  
<!-- FOOTER_END -->
