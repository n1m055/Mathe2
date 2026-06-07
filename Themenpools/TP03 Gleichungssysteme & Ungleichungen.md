---
themenpool: 3
titel: "Lineare Gleichungssysteme und Ungleichungen bzw. Ungleichungssysteme"
gebiet: Algebra
tags: [themenpool, algebra, lgs, ungleichungen]
quelle: ["Themenpool 3", "Notizbuch 5B (2022/23)"]
verwandt: ["[[TP04 Vektoren in R2]]", "[[TP05 Vektoren in R3]]", "[[TP02 Lineare & quadratische Modelle]]"]
---

# TP03 — Lineare Gleichungssysteme & Ungleichungen

> [!info] Leitidee
> Ein lineares Gleichungssystem sucht die **gemeinsamen** Lösungen mehrerer linearer Gleichungen — geometrisch der Schnitt von Geraden (2D) bzw. Ebenen (3D). Ungleichungen beschreiben **Bereiche** statt einzelner Punkte; entscheidend sind Vorzeichen und Fallunterscheidungen.
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 3]] · Notizbuch **5B**

## 1. Lineare Gleichungssysteme (LGS)

> [!definition] Lineares Gleichungssystem, Lösung, Lösungsmenge #definition
> Ein **LGS** aus $m$ Gleichungen mit $n$ Unbekannten ist eine Menge linearer Gleichungen, die **gleichzeitig** erfüllt sein sollen, z. B.
> $$\begin{cases} a_1x+b_1y=c_1\\ a_2x+b_2y=c_2\end{cases}$$
> Eine **Lösung** ist ein Tupel $(x\mid y)$, das **jede** Gleichung erfüllt. Die **Lösungsmenge** $\mathbb{L}$ ist die Menge aller Lösungen.

> [!merke] Lösungsmethoden #merke
> - **Einsetzverfahren** — eine Gleichung nach einer Variablen auflösen, einsetzen.
> - **Gleichsetzungsverfahren** — beide nach derselben Variablen auflösen, gleichsetzen.
> - **Additions-/Eliminationsverfahren** — Gleichungen so kombinieren, dass eine Variable wegfällt.
> - **Gauß-Verfahren** — durch erlaubte Umformungen (Zeilen tauschen, mit $\lambda\neq0$ multiplizieren, Vielfaches addieren) auf **Stufenform** bringen; besonders bei 3 Unbekannten systematisch.

![[lgs-faelle.svg|640]]
*Abbildung: Zwei Geraden in der Ebene können sich schneiden (genau eine Lösung), parallel sein (keine Lösung) oder identisch sein (unendlich viele Lösungen).*

> [!satz] Lösbarkeit und geometrische Deutung #satz
> | Fall | algebraisch | 2D (Geraden) | 3D (Ebenen) |
> |---|---|---|---|
> | **eindeutig** | genau eine Lösung | Schnittpunkt | ein Schnittpunkt |
> | **keine Lösung** | Widerspruch (z. B. $0=5$) | parallel | parallel / kein gem. Punkt |
> | **unendlich viele** | allgemeingültig ($0=0$), freier Parameter | identisch | gemeinsame Gerade/Ebene |
>
> Geometrische Vertiefung: [[TP04 Vektoren in R2]], [[TP05 Vektoren in R3]].

> [!beispiel] LGS mit Eliminationsverfahren #beispiel
> $\begin{cases}2x+3y=12\\ x-y=1\end{cases}$ — zweite Gleichung $\times3$: $3x-3y=3$, addieren $\Rightarrow 5x=15\Rightarrow x=3$, dann $y=2$. Probe: $2\cdot3+3\cdot2=12$ ✓. Lösung $(3\mid2)$ = Schnittpunkt.

> [!beispiel] $3\times3$ in Stufenform #beispiel
> $\begin{cases}x+y+z=6\\ 2x-y+z=3\\ x+2y-z=2\end{cases}\Rightarrow x=1,\ y=2,\ z=3.$ Geometrisch: drei Ebenen schneiden sich in **einem Punkt** $(1\mid2\mid3)$.

## 2. Ungleichungen

> [!definition] Ungleichung, Lösungsmenge #definition
> Eine **Ungleichung** verbindet zwei Terme mit $<,\le,>,\ge$. Ihre **Lösungsmenge** ist die Menge aller $x$, die sie erfüllen — meist ein **Intervall** oder eine Vereinigung von Intervallen.

> [!satz] Grundregel — Vorzeichenwechsel #satz #merke
> Multipliziert/dividiert man eine Ungleichung mit einer **negativen** Zahl, **dreht sich das Relationszeichen um**:
> $$-2x<6 \iff x>-3.$$
> Häufigste Fehlerquelle!

### Bruchungleichungen
> [!merke] Methode #merke
> Bei $\frac{A}{B}\lessgtr c$ darf man nicht einfach mit $B$ multiplizieren (Vorzeichen von $B$ unbekannt). Zwei Wege: **Fallunterscheidung** $B>0$ / $B<0$ (mit Definitionslücke $B=0$) oder **Vorzeichentabelle** (alles auf eine Seite, Zähler- und Nennernullstellen markieren, Vorzeichen je Abschnitt prüfen).

> [!beispiel] Bruchungleichung #beispiel
> $\frac{x-1}{x+2}\ge0$. Nullstellen: Zähler $x=1$, Nenner $x=-2$ (ausgeschlossen). Vorzeichen auf $(-\infty,-2),(-2,1),(1,\infty)$: $+,-,+$.
> $\mathbb{L}=(-\infty;-2)\cup[1;\infty)$ ($x=1$ erlaubt, $x=-2$ verboten).

### Betragsungleichungen
> [!formel] Beträge auflösen #formel #merke
> $$|x|<a \iff -a<x<a \qquad |x|>a \iff x<-a \ \text{oder}\ x>a$$
> Deutung: $|x-m|<r$ = „Abstand von $m$ kleiner als $r$" = Intervall $(m-r,\,m+r)$.

> [!beispiel] Betrag #beispiel
> $|2x-4|\le6 \Rightarrow -6\le2x-4\le6 \Rightarrow -1\le x\le5$. $\mathbb{L}=[-1;5]$.

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. Definieren Sie ein LGS und seine Lösungsmenge. Nennen Sie die Lösungsmethoden.
> 2. Erklären Sie die drei Lösbarkeitsfälle eines $2\times2$-Systems geometrisch (Abbildung).
> 3. Wann hat ein $3\times3$-LGS keine / genau eine / unendlich viele Lösungen? Veranschaulichen Sie mit Ebenen.
> 4. **Warum** dreht sich bei Multiplikation mit einer negativen Zahl das Ungleichungszeichen um?
> 5. Lösen Sie $\frac{x-1}{x+2}\ge0$ und $|2x-4|\le6$, jeweils mit Begründung.

## Verwandte Themen
[[TP02 Lineare & quadratische Modelle]] · [[TP04 Vektoren in R2]] · [[TP05 Vektoren in R3]]
