---
type: typedef
title: Notiz
description: Eine Notiz ohne spezifischeren Typ.
created: 2026-08-27
modified: 2026-08-27T12:40:50
modified_by: claude-opus-5
---

# Properties

| Property | Typ | Pflicht | Beschreibung |
|---|---|---|---|
| about | hkf-link-list | nein | Worauf sich die Notiz bezieht |
| sources | hkf-link-list:source | nein | Verwendete Quellen |

# Konventionen

Auffangtyp. Er wird verwendet, wenn kein anderer Typ passt — nicht, um die
Wahl eines Typs zu vermeiden. `about` nimmt Verweise beliebigen Typs auf.
