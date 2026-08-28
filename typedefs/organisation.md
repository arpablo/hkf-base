---
type: typedef
title: Organisation
description: 'Eine Körperschaft: Unternehmen, Institut, Verein, Behörde.'
created: 2026-08-27
modified: 2026-08-27T15:41:37
modified_by: claude-opus-5
---

# Properties

| Property | Typ | Pflicht | Beschreibung |
|---|---|---|---|
| founded | date | nein | Gründungsdatum |
| founded_year | hkf-year | nein | Gründungsjahr, wenn kein Datum bekannt ist |
| dissolved | date | nein | Auflösungsdatum |
| dissolved_year | hkf-year | nein | Auflösungsjahr, wenn kein Datum bekannt ist |
| o_categories | hkf-organisation-category-list | nein | Art der Körperschaft |
| seat | hkf-link:place | nein | Sitz |
| parent | hkf-link:organisation | nein | Übergeordnete Körperschaft |
| homepage | hkf-url | nein | Webseite |
| email | hkf-email | nein | Kontaktadresse |
| phone | hkf-phone | nein | Telefonnummer |
| logo | hkf-file:image / hkf-url | nein | Bildmarke, als Datei in der Ablage oder als Adresse im Netz |
| wikidata_id | hkf-wikidata | nein | Kennung des Gegenstands in Wikidata |

# Konventionen

Rechtsform und Untergliederungen gehören in den Body, nicht in den Namen.
