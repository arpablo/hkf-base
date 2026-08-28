---
type: typedef
title: Begriff
description: Ein definierter Begriff.
created: 2026-08-27
modified: 2026-08-27T15:31:41
modified_by: claude-opus-5
---

# Properties

| Property | Typ | Pflicht | Beschreibung |
|---|---|---|---|
| lang | hkf-lang | nein | Sprache des Begriffs |
| broader | hkf-link:term | nein | Übergeordneter Begriff |
| related | hkf-link-list:term | nein | Verwandte Begriffe |
| sources | hkf-link-list:source | nein | Belege der Definition |
| wikidata_id | hkf-wikidata | nein | Kennung des Gegenstands in Wikidata |

# Konventionen

Der Body beginnt mit einer Definition in einem Satz. Synonyme werden als
Obsidian-`aliases` geführt, nicht als eigene Property.
