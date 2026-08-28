---
type: typedef
title: Ort
description: Ein geographischer Ort.
created: 2026-08-27
modified: 2026-08-27T15:41:37
modified_by: claude-opus-5
---

# Properties

| Property | Typ | Pflicht | Beschreibung |
|---|---|---|---|
| latitude | hkf-latitude | nein | Geographische Breite |
| longitude | hkf-longitude | nein | Geographische Länge |
| country | hkf-country | nein | Staat |
| address | text | nein | Anschrift in einer Zeile |
| part_of | hkf-link:place | nein | Übergeordneter Ort |
| image | hkf-file:image / hkf-url | nein | Ansicht, als Datei in der Ablage oder als Adresse im Netz |
| wikidata_id | hkf-wikidata | nein | Kennung des Gegenstands in Wikidata |

# Konventionen

`latitude` und `longitude` werden nur gemeinsam gesetzt. `part_of` bildet die
räumliche Schachtelung ab — Gebäude in Stadt, Stadt in Region.
