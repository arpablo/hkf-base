# hkf-base — stillgelegt

Dieses Repository lieferte das Vokabular von HKF als Bundle: Person,
Körperschaft, Ort, Ereignis, Quelle, Begriff und die übrigen. **Seit HKF
Config 1.0 wird davon nichts mehr geliefert.**

Alle Typdefinitionen und Property-Typen gehören jetzt zur **Grundausstattung**
einer Wissensbasis. Sie entstehen mit ihr, statt zugeladen zu werden, und
stehen darum in der Vorlage:

| | |
|---|---|
| Spezifikation | [`HKF-Config-V1.0.md`](https://github.com/arpablo/hkf-spec/blob/main/HKF-Config-V1.0.md) |
| Vorlage | [`hkf-kb-template`](https://github.com/arpablo/hkf-kb-template) |
| Werkzeuge | [`hkf-harness`](https://github.com/arpablo/hkf-harness) — `hk-init` legt die Grundausstattung an |

## Warum

Der Grund steht in Config §1. Für die drei Kern-Typen `typedef`, `proptype`
und `bundle` war es immer so: Ein Import muss Typdefinitionen ablegen und die
Lieferung verbuchen können, bevor er irgendetwas anderes tut — ein Bundle, das
sie mitbrächte, müsste sich selbst schon kennen.

Für die übrigen gilt derselbe Schluss aus einem einfacheren Grund: Was jede
Wissensbasis ohnehin bekommt, muss niemand ausliefern. Ein Bundle bringt
Inhalte mit und, wenn es einen Typ braucht, den Config nicht kennt, dessen
Typdefinition dazu — nie eine von hier.

Die Kennung `hkf-base` bleibt vergeben. Sie benannte eine Lieferreihe, und
eine Kennung wird nach Core §4.1 nicht neu vergeben.
