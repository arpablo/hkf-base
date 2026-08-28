---
type: typedef
title: Veranstaltung
description: Ein Geschehen zu einer bestimmten Zeit.
created: 2026-08-27
modified: 2026-08-27T12:40:50
modified_by: claude-opus-5
---

# Properties

| Property | Typ | Pflicht | Beschreibung |
|---|---|---|---|
| date | date | nein | Tag, wenn keine Uhrzeit bekannt ist |
| starts_at | datetime | nein | Beginn |
| ends_at | datetime | nein | Ende |
| location | hkf-link:place | nein | Veranstaltungsort |
| organizer | hkf-link:person,organisation | nein | Ausrichter |
| participants | hkf-link-list:person,organisation | nein | Beteiligte |
| cancelled | checkbox | nein | Abgesagt |
| homepage | hkf-url | nein | Ankündigung |

# Konventionen

Eine Veranstaltung trägt entweder `starts_at` oder `date`, nicht beides.
Zeiten gelten in der `timezone` der Ablage (Core §3.4).
