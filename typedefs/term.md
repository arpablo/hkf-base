---
type: typedef
title: Begriff
description: Ein definierter Begriff.
created: 2026-08-27
modified: 2026-08-29T07:23:15
modified_by: claude-opus-5
---

# Properties

| Property | Typ | Pflicht | Beschreibung |
|---|---|---|---|
| lang | hkf-lang | nein | Sprache des Begriffs |
| broader | hkf-link:term | nein | Übergeordneter Begriff |
| sources | hkf-link-list:source | nein | Belege der Definition |
| wikidata_id | hkf-wikidata | nein | Kennung des Gegenstands in Wikidata |
| related | hkf-link-or-url-list | nein | Verwandtes: Notizen oder Adressen; nimmt auf, was unter „Siehe auch" steht |

# Konventionen

Der Body beginnt mit einer Definition in einem Satz. Synonyme werden als
Obsidian-`aliases` geführt, nicht als eigene Property.
