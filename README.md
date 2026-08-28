# HKF Base — das Standardvokabular

Dieses Repository ist ein **HKF-Bundle**. Es liefert das Vokabular von
[**HKF Base 1.0**](https://github.com/arpablo/hkf-spec/blob/main/HKF-Base-V1.0.md): neun Typdefinitionen und zwei Aufzählungen.
Wurzeldatei ist `hbundle.md`.

| | |
|---|---|
| Kennung | `hkf-base` |
| Fassung | `1.0` |
| Spezifikation | [`HKF-Base-V1.0.md`](https://github.com/arpablo/hkf-spec/blob/main/HKF-Base-V1.0.md) |
| setzt voraus | [HKF Core 1.0](https://github.com/arpablo/hkf-spec/blob/main/HKF-Core-V1.0.md) |

Die verbindliche Fassung steht in der Spezifikation, nicht hier: Was dieses
Bundle ausliefert, ist die maschinenlesbare Form von [§3 in
HKF-Base-V1.0.md](https://github.com/arpablo/hkf-spec/blob/main/HKF-Base-V1.0.md#3-typdefinitionen). Weichen beide voneinander ab, gilt
die Spezifikation — `tools/check-base.py` im Repository
[`hkf-spec`](https://github.com/arpablo/hkf-spec) prüft das.

## Was geliefert wird

| Typ | Verzeichnis | Zweck |
|---|---|---|
| `person` | `persons` | Ein Mensch. |
| `organisation` | `organisations` | Eine Körperschaft: Unternehmen, Institut, Verein, Behörde. |
| `place` | `places` | Ein geographischer Ort. |
| `event` | `events` | Ein Geschehen zu einer bestimmten Zeit. |
| `source` | `sources` | Eine zitierbare Quelle: Buch, Aufsatz, Webseite, Vortrag. |
| `term` | `terms` | Ein definierter Begriff. |
| `topic` | `topics` | Ein Themengebiet als Einstiegspunkt. |
| `note` | `notes` | Eine Notiz ohne spezifischeren Typ. |
| `specification` | `specifications` | Ein normatives Dokument, an das sich die Wissensbasis hält. |

Dazu die beiden Property-Typen `hkf-person-category` und
`hkf-organisation-category`, die nur mit `person` und `organisation` Sinn
ergeben.

**Keine Notizen, keine Mediendateien, keine Grundausstattung.** Die
Property-Typen und die Kern-Typen `typedef`, `proptype` und `bundle` legt eine
Wissensbasis beim Anlegen selbst an; ein Bundle liefert sie nicht.

## Verwenden

Das Bundle wird mit `hk-import` in eine bestehende Wissensbasis geladen — etwa
in eine, die aus der Vorlage [`hkf-kb-template`](https://github.com/arpablo/hkf-kb-template) entstanden
ist.
Danach steht dort in `bundles/hkf-base.md` eine Notiz mit dem Importnachweis, und
jede übernommene Typdefinition trägt die Zugehörigkeit in ihrer
`bundles`-Property.

Der Import ist **freiwillig**. Eine Wissensbasis, die andere Gegenstände
verwaltet, definiert stattdessen eigene Typen. Wer aber einen Typ dieses
Namens führt, führt ihn in dieser Fassung — nur so bleiben Bundles zwischen
fremden Wissensbasen austauschbar.

## Fortschreibung

Die Regeln dafür stehen in [§5 von HKF-Base-V1.0.md](https://github.com/arpablo/hkf-spec/blob/main/HKF-Base-V1.0.md#5-versionierung).
Eine neue Fassung darf Typen ergänzen, Properties ergänzen und die `values`
der beiden Aufzählungen erweitern. Sie darf nichts entfernen und keine
Bedeutung ändern, weil das vorhandene Notizen ungültig machte.

Fortschreibung in einer Wissensbasis ist ein erneuter Import: geänderte
Notizen werden übernommen, unveränderte übersprungen.
