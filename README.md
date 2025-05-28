# FORSTINGER Dropshipper Import Vorgaben

Um einen möglichst reibungslosen Import von Dropshiper Daten zu gewährleisten, bitten wir darum die Daten im vorgegebenen Format anzuliefern:

## Spaltenübersicht - Basisdaten
| Spalte | Typ | Beschreibung | Pflichtfeld |
|--------|-----|--------------|-------------|
| sku | text(9) | Forstinger SKU (wenn bekannt) | |
| ean | int(13) | EAN Nummer | * |
| name | text(255) | Artikelname | * |
| description | textarea | Artikel Beschreibung (HTML Tags "p", "ul", "li", "ul", "ol", "b" und "i" werden akzeptiert) | * |
| metaTitle | text(255) | SEO Metatitel | * |
| metaDescription | text(255) | SEO Metabeschreibung | * |
| metaKeywords | text | SEO Metaschlüsselwörter (getrennt durch ",") | * |
| searchKeywords | text | Schlüsselwörter für Suche (getrennt durch Pipe "\|") | * |
| categories | text | Kategorien laut ... (getrennt durch Pipe "\|") | * |
| manufacturerItemNumber | text(255) | Hersteller Teilenummer | * |
| imageGallery | text | URL's zu Bildern (getrennt durch Pipe "\|") | * |
| imageGallery | text | URL's zu Bildern (getrennt durch Pipe "\|") | * |
| attachments | text | URL's zu PDF Dokumenten (getrennt durch Pipe "\|") |  |
| video | text | YouTube Codes für Videos (getrennt durch Pipe "\|") |  |

## Spaltenübersicht - Artikeleigenschaften

Diese Spalten sind optional, sollten aber für eine bessere Darstellung der Artikel im Shop nach Möglichkeit angegeben werden. Die Werte müssen den Vorgaben der jeweiligen Spalte entsprechen.

| Spalte | Typ | Beschreibung |
|--------|-----|--------------|
| propertiesStore~NetContent~capacity | int | Füllmenge in Milliliter [ml] |
| propertiesStore~Capacity~capacity | int | Volumen / Fassungsvermögen in Liter [l] |
| propertiesStore~Color~color | select | Farbe laut [FORSTINGER Farben](https://pim-forstinger.dynaflow.at/dropship/csv/tmpl/Color.csv) |
| propertiesStore~Size~size | select | Größe laut [FORSTINGER Größen](https://pim-forstinger.dynaflow.at/dropship/csv/tmpl/Size.csv) |
| propertiesStore~TargetGroup~targetGroup | multiselect | Zielgruppe(n) laut [FORSTINGER Zielgruppen](https://pim-forstinger.dynaflow.at/dropship/csv/tmpl/TargetGroup.csv), getrennt durch Pipe "\|") |
| propertiesStore~Material~material | select | Material laut [FORSTINGER Material](https://pim-forstinger.dynaflow.at/dropship/csv/tmpl/Material.csv) |
| ... | ... | ... |
