# Auswertung Ombudscom-Statistiken 2014-2018

## Vorbemerkungen

Dieses Dokument beschreibt die Vorprozessierung und explorative Analyse des Datensatzes, der Grundlage des auf srf.ch veröffentlichten Artikel [Diese Telekom-Anbieter sorgen für den meisten Unmut](https://www.srf.ch/news/schweiz/nun-herrscht-klarheit-diese-telekom-anbieter-sorgen-fuer-den-meisten-unmut) ist.

SRF Data legt Wert darauf, dass die Datenvorprozessierung und -Analyse nachvollzogen und überprüft werden kann. SRF Data glaubt an das Prinzip offener Daten, aber auch offener und nachvollziehbarer Methoden. Zum anderen soll es Dritten ermöglicht werden, auf dieser Vorarbeit aufzubauen und damit weitere Auswertungen oder Applikationen zu generieren.  


Die Endprodukte des vorliegenden Scripts, neben der vorliegenden explorativen Analyse, sind (Datenbeschreibung siehe unten):

* `reasons_top_four_providers.csv`
* `cases_per_type.csv`
* `cases_top_4_with_exit.csv`

### R-Script & Daten

Die Vorprozessierung und Analyse wurde im Statistikprogramm R vorgenommen. Das zugrunde liegende Script sowie die prozessierten Daten können unter [diesem Link](https://srfdata.github.io/2019-11-ombudscom/rscript.zip) heruntergeladen werden. Durch Ausführen von `main.Rmd` kann der hier beschriebene Prozess nachvollzogen und der für den Artikel verwendete Datensatz generiert werden. Dabei werden Daten aus dem Ordner `input` eingelesen und Ergebnisse in den Ordner `output` geschrieben. 

SRF Data verwendet das [rddj-template](https://github.com/grssnbchr/rddj-template) von Timo Grossenbacher als Grundlage für seine R-Scripts.  Entstehen bei der Ausführung dieses Scripts Probleme, kann es helfen, die Anleitung von [rddj-template](https://github.com/grssnbchr/rddj-template) zu studieren. 

Debug-Informationen: *This report was generated on `r Sys.time()`. R version: `r paste0(version$major, ".", version$minor)` on `r version$platform`. For this report, CRAN packages as of `r package_date` were used.*

### GitHub

Der Code für die vorliegende Datenprozessierung ist auf [https://github.com/srfdata/2019-11-ombudscom](https://github.com/srfdata/2019-11-ombudscom) zur freien Verwendung verfügbar. 


### Lizenz

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons Lizenzvertrag" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Dataset" property="dct:title" rel="dct:type">2019-11-ombudscom</span> von <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/srfdata/2019-11-ombudscom" property="cc:attributionName" rel="cc:attributionURL">SRF Data</a> ist lizenziert unter einer <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Namensnennung - Weitergabe unter gleichen Bedingungen 4.0 International Lizenz</a>.

### Weitere Projekte

Code & Daten von [SRF Data](https://srf.ch/data) sind unter [https://srfdata.github.io](https://srfdata.github.io) verfügbar.

### Haftungsausschluss

Die veröffentlichten Informationen sind sorgfältig zusammengestellt, erheben aber keinen Anspruch auf Aktualität, Vollständigkeit oder Richtigkeit. Es wird keine Haftung übernommen für Schäden, die  durch die Verwendung dieses Scripts oder der daraus gezogenen Informationen entstehen. Dies gilt ebenfalls für Inhalte Dritter, die über dieses Angebot zugänglich sind.

