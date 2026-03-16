# Georgievi Brothers Trade Correspondence (1847–1863)

## Project Overview

This repository contains a **TEI XML–encoded corpus of 680 commercial letters** from the archive of the Bulgarian merchant house of **Hristo Georgiev** and **Evlogi Georgiev**.

The correspondence spans **17 January 1847 – 20 April 1863** and documents the commercial activities of the Georgievi trading network across the **Danubian Principalities, the Ottoman Empire, and Western Europe**.

The letters record:

* commodity trade
* financial transfers and credit relations
* transportation logistics
* merchant partnerships and agents
* commercial risk and market information

The corpus offers valuable material for studying **nineteenth-century Balkan merchant networks and transnational trade**.

---

# Interactive Visualization

The TEI XML corpus can be explored through an interactive web interface:

**Streamlit application**

[https://georgievi-network-7yeau6d6whkwazqwe5zjmv.streamlit.app/](https://georgievi-network-7yeau6d6whkwazqwe5zjmv.streamlit.app/)

The application allows users to:

* browse the letters
* explore metadata fields
* inspect geographic references
* visualize merchant networks

---

# Related Repository

The code used for network analysis and the visualization environment is available here:

[https://github.com/Bestroi150/georgievi-network/tree/main](https://github.com/Bestroi150/georgievi-network/tree/main)

This repository contains:

* data processing scripts
* network construction workflows
* Streamlit visualization code

---

# Geographic Scope

The correspondence connects merchants across multiple commercial centers including:

* Bucharest
* Brăila
* Galați
* Giurgiu
* Ruse
* Veliko Tarnovo
* Svishtov
* Manchester
* Constantinople
* Marseille

This geographic distribution reflects the **international commercial infrastructure of Balkan merchants in the mid-nineteenth century**.

---

# Dataset

## Main Files

### `georgievi_correspondence_1847-1863_bg.xml`

Primary TEI XML dataset.

Metadata fields are encoded in **Bulgarian**, reflecting the language of the original archival summaries.

---

### `georgievi_correspondence_1847-1863_en.xml`

*(currently distributed as `data_english.xml`)*

English-language version of the corpus.

All metadata fields have been translated to support **international research use and digital humanities projects**.

---

# TEI Encoding Structure

Each letter is encoded as:

```xml
<object type="letter">
```

within a `<listObject>` container.

## Core Metadata

| Element                   | Description                        |
| ------------------------- | ---------------------------------- |
| `<idno type="shelfmark">` | Archival shelfmark                 |
| `<desc type="sender">`    | Sender name, place, date           |
| `<desc type="addressee">` | Addressee name and place           |
| `<textLang>`              | Language(s) of the original letter |

---

## Thematic Annotation

Each letter includes structured thematic lists:

```
<list type="main_topics">
<list type="keywords">
<list type="other_info">
```

These record:

* commercial themes
* commodities and financial instruments
* notable remarks or observations

---

## Geographic References

Places mentioned in the letters are encoded with **GeoNames identifiers and geographic coordinates**.

Example:

```xml
<placeName ref="[GeoNames URL]">Place Name</placeName>
<location>
  <geo>latitude longitude</geo>
</location>
```

This enables **geospatial analysis and network visualization**.

---

## Persons Mentioned

Individuals referenced in the letters are encoded in:

```
<desc type="mentioned_persons">
```

These references allow reconstruction of **merchant and intermediary networks**.

---

# Repository Structure

```
georgievi-correspondence/
│
├── data/
│   ├── georgievi_correspondence_1847-1863_bg.xml
│   └── georgievi_correspondence_1847-1863_en.xml
││
└── README.md
```

---

# Encoding History

| Date        | Encoder | Action                                               |
| ----------- | ------- | ---------------------------------------------------- |
| 20 Nov 2022 | K.S.    | Initial TEI encoding from CSV dataset                |
| 2024        | K.S.    | Added geographic coordinates and GeoNames references |
| 2025        | K.S.    | Added ISO-8601 date encoding (`when` attributes)     |
| 2026        | K.S.    | Created English-language metadata version            |

---

# TEI Schema

The XML files validate against the **TEI All schema**:

```
http://www.tei-c.org/release/xml/tei/custom/schema/relaxng/tei_all.rng
```

---

# Archival Source

**Archive:** Georgievi Brothers Collection

The letters derive primarily from archival bundles covering **1856–1863**.

---

# License

This dataset is released under the **Creative Commons Attribution 4.0 International License (CC-BY 4.0)**.

This allows reuse, distribution, and adaptation provided that **appropriate credit is given**.

---

# Citation

If you use this dataset in research, please cite:

```

```

---


