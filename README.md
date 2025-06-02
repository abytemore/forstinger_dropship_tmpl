# FORSTINGER Dropshipper Import Vorgaben

Um einen möglichst reibungslosen Import von Dropshiper Daten zu gewährleisten, bitten wir darum die Daten im vorgegebenen Format anzuliefern:

## Spaltenübersicht - Basisdaten
| Spalte | Typ | Beschreibung | Pflichtfeld |
|--------|-----|--------------|-------------|
| sku | text(9) | Forstinger SKU (wenn bekannt) | |
| ean | int(13) | EAN Nummer | * |
| name | text | Artikelname | * |
| description | textarea | Artikel Beschreibung (HTML Tags "p", "ul", "li", "ul", "ol", "b" und "i" werden akzeptiert) | * |
| metaTitle | text | SEO Metatitel | * |
| metaDescription | text | SEO Metabeschreibung | * |
| metaKeywords | text | SEO Metaschlüsselwörter (getrennt durch ",") | * |
| searchKeywords | text | Schlüsselwörter für Suche (getrennt durch Pipe "\|") | * |
| categories | text | Kategorien laut ... (getrennt durch Pipe "\|") | * |
| manufacturerItemNumber | text | Hersteller Teilenummer | * |
| imageGallery | text | URL's zu Bildern (getrennt durch Pipe "\|") | * |
| attachments | text | URL's zu PDF Dokumenten (getrennt durch Pipe "\|") |  |
| video | text | YouTube Codes für Videos (getrennt durch Pipe "\|") |  |

## Spaltenübersicht - Artikeleigenschaften

Diese Spalten sind optional, sollten aber, für eine bessere Darstellung der Artikel im Shop soweit sinnvoll, angegeben werden. Die Werte müssen den Vorgaben der jeweiligen Spalte entsprechen.
Bei Feldern vom Typ "select" bzw. "multiselect" ist der Wert aus der Spalte "value" verwenden (siehe Link in der jeweiligen Feldbeschreibung).
Bei Feldern vom Typ "bool" ist der Wert 0 für "nein" und 1 für "ja" zu verwenden.

| Spalte | Typ | Beschreibung |
|--------|-----|--------------|
| propertiesStore~NetContent~capacity | int | Füllmenge in Milliliter [ml] |
| propertiesStore~Capacity~capacity | int | Volumen / Fassungsvermögen in Liter [l] |
| propertiesStore~Power~power | int | Leistung in Watt [W] |
| propertiesStore~Voltage~voltage | int | Spannung in Volt [V] |
| propertiesStore~Color~color | select | Farbe laut [FORSTINGER Farben](https://pim-forstinger.dynaflow.at/dropship/csv/tmpl/Color.csv) |
| propertiesStore~Size~size | select | Größe laut [FORSTINGER Größen](https://pim-forstinger.dynaflow.at/dropship/csv/tmpl/Size.csv) |
| propertiesStore~TargetGroup~targetGroup | multiselect | Zielgruppe(n) laut [FORSTINGER Zielgruppen](https://pim-forstinger.dynaflow.at/dropship/csv/tmpl/TargetGroup.csv), getrennt durch Pipe "\|") |
| propertiesStore~Material~material | select | Material laut [FORSTINGER Material](https://pim-forstinger.dynaflow.at/dropship/csv/tmpl/Material.csv) |
| propertiesStore~ISize~iSize | select | iSize für Kindersizte [FORSTINGER iSize](https://pim-forstinger.dynaflow.at/dropship/csv/tmpl/ISize.csv) |
| propertiesStore~Isofix~isofix | bool | ISOFIX Kindersitze |
| propertiesStore~normChildSeat~NormChildCarSeat | select | Norm für Kindersitze [FORSTINGER Normen Kindersitze](https://pim-forstinger.dynaflow.at/dropship/csv/tmpl/NormChildCarSeat.csv) |
| propertiesStore~Dimensions~length | int | Artikellänge in Millimeter [mm] |
| propertiesStore~Dimensions~width | int | Artikelbreite in Millimeter [mm] |
| propertiesStore~Dimensions~height | int | Artikelhöhe in Millimeter [mm] |
