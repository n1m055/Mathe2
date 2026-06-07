---
themenpool: 1
titel: "Zahlenbereiche, Mengen, Algebraische Gleichungen"
gebiet: Algebra
tags: [themenpool, algebra, zahlenbereiche, mengen, gleichungen]
quelle: ["Themenpool 1", "Notizbuch 5B (2022/23)", "Notizbuch 7B (2024/25) – komplexe Zahlen"]
verwandt: ["[[TP02 Lineare & quadratische Modelle]]", "[[TP08 Funktionen & Polynomfunktionen]]"]
---

# TP01 — Zahlenbereiche, Mengen, Algebraische Gleichungen

> [!info] Leitidee
> Jede Erweiterung des Zahlenbereichs entsteht, weil eine Gleichung im alten Bereich keine Lösung hat. Mengen sind die Sprache, in der wir diese Bereiche und ihre Lösungen beschreiben. Der **Fundamentalsatz der Algebra** schließt den Kreis: in $\mathbb{C}$ hat jede algebraische Gleichung genügend Lösungen.
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 1]] · Notizbuch **5B** (Grundlagen), **7B** (komplexe Zahlen)

## 1. Mengen — Grundbegriffe

> [!definition] Menge (nach Georg Cantor) #definition
> Eine **Menge** ist eine Zusammenfassung bestimmter, wohlunterschiedener Objekte unserer Anschauung oder unseres Denkens zu einem Ganzen. Die Objekte heißen **Elemente**. Man schreibt $x\in A$ („$x$ ist Element von $A$") bzw. $x\notin A$.
> Eine Menge ist durch ihre Elemente **eindeutig bestimmt** (Extensionalität); Reihenfolge und Wiederholung spielen keine Rolle.

> [!definition] Darstellung und Beziehungen #definition
> - **Aufzählend:** $A=\{1,2,3,4\}$ — **beschreibend:** $A=\{x\in\mathbb{N}\mid 1\le x\le 4\}$.
> - **Teilmenge:** $A\subseteq B \;:\!\iff\; (\forall x:\ x\in A \Rightarrow x\in B)$.
> - **Gleichheit:** $A=B \iff A\subseteq B \ \text{und}\ B\subseteq A$.
> - **Leere Menge:** $\varnothing$ (enthält kein Element), ist Teilmenge jeder Menge.

> [!formel] Verknüpfungen #formel
> $$A\cup B=\{x\mid x\in A \ \text{oder}\ x\in B\}\qquad A\cap B=\{x\mid x\in A \ \text{und}\ x\in B\}$$
> $$A\setminus B=\{x\mid x\in A \ \text{und}\ x\notin B\}\qquad |A\cup B|=|A|+|B|-|A\cap B|$$

![[venn.svg|460]]
*Abbildung: Zwei Mengen $A,B$. Der Überlappungsbereich ist $A\cap B$, beide Kreise zusammen sind $A\cup B$. „oder" ist hier das nicht-ausschließende Oder.*

## 2. Die Zahlenbereiche und ihre Erweiterung

![[zahlenbereiche.svg|470]]
*Abbildung: Die Zahlenbereiche sind ineinander geschachtelt. Jeder äußere Ring enthält Zahlen, die der innere nicht „lösen" kann.*

> [!definition] Die fünf Zahlenbereiche #definition #formel
> $$\mathbb{N}\subset\mathbb{Z}\subset\mathbb{Q}\subset\mathbb{R}\subset\mathbb{C}$$
> - $\mathbb{N}=\{0,1,2,3,\dots\}$ — natürliche Zahlen (Zählen).
> - $\mathbb{Z}=\{\dots,-2,-1,0,1,2,\dots\}$ — ganze Zahlen; Abschluss unter **Subtraktion**.
> - $\mathbb{Q}=\left\{\dfrac{p}{q}\;\middle|\; p\in\mathbb{Z},\ q\in\mathbb{Z}\setminus\{0\}\right\}$ — rationale Zahlen; Abschluss unter **Division**.
> - $\mathbb{R}$ — reelle Zahlen; **vollständig**: es gibt keine „Lücken" (jede nach oben beschränkte Teilmenge hat eine kleinste obere Schranke). Enthält die irrationalen Zahlen wie $\sqrt2,\pi,e$.
> - $\mathbb{C}=\{a+bi\mid a,b\in\mathbb{R}\}$ mit $i^2=-1$; Abschluss unter **Wurzelziehen** / Lösen aller Polynomgleichungen.

**Treibende Idee** (zentrale Transferfrage): Ein Bereich wird erweitert, sobald eine Rechenoperation **aus ihm hinausführt** — $\mathbb{N}$ ist nicht abgeschlossen unter Subtraktion ($2-5\notin\mathbb{N}$), $\mathbb{Z}$ nicht unter Division, $\mathbb{Q}$ nicht unter dem Grenzwert/Wurzel, $\mathbb{R}$ nicht unter Wurzeln aus negativen Zahlen.

> [!satz] Eigenschaften zum Argumentieren #satz #merke
> - **Rational $\iff$ endliche oder periodische** Dezimaldarstellung. Irrational $\iff$ unendlich, nicht-periodisch.
> - $\mathbb{Q}$ ist **abzählbar** (gleichmächtig zu $\mathbb{N}$, Cantors Diagonalverfahren), $\mathbb{R}$ ist **überabzählbar** — es gibt „mehr" irrationale als rationale Zahlen.
> - $\mathbb{Q}$ liegt **dicht** in $\mathbb{R}$: zwischen je zwei reellen Zahlen liegt eine rationale.

> [!beispiel] Beweis: $\sqrt{2}$ ist irrational #herleitung #beispiel
> Annahme (Widerspruch): $\sqrt2=\frac{p}{q}$ vollständig gekürzt. Dann $2q^2=p^2$, also ist $p^2$ gerade $\Rightarrow p$ gerade $\Rightarrow p=2k \Rightarrow 2q^2=4k^2 \Rightarrow q^2=2k^2 \Rightarrow q$ gerade. Also sind $p,q$ beide gerade — Widerspruch zur vollständigen Kürzung. $\blacksquare$

## 3. Algebraische Gleichungen

> [!definition] Polynomgleichung, Nullstelle, Vielfachheit #definition
> Eine **Polynomgleichung $n$-ten Grades** hat die Form
> $$a_n x^n+a_{n-1}x^{n-1}+\dots+a_1x+a_0=0,\qquad a_n\neq0.$$
> Eine Zahl $x_1$ mit $p(x_1)=0$ heißt **Nullstelle** (Lösung). $x_1$ hat die **Vielfachheit** $k$, wenn $(x-x_1)^k$ das Polynom teilt, $(x-x_1)^{k+1}$ aber nicht.

> [!satz] Faktorsatz & Satz vom Nullprodukt #satz #merke
> $x_1$ ist genau dann Nullstelle von $p$, wenn sich $(x-x_1)$ als **Linearfaktor** abspalten lässt: $p(x)=(x-x_1)\cdot q(x)$. Ein Produkt ist null $\iff$ mindestens ein Faktor ist null — daher liest man aus der faktorisierten Form $a_n(x-x_1)\cdots(x-x_n)=0$ alle Lösungen direkt ab.

> [!satz] Fundamentalsatz der Algebra #satz
> Jedes Polynom vom Grad $n\ge1$ hat in $\mathbb{C}$ **genau $n$ Nullstellen** (mit Vielfachheit gezählt). Reelle Polynome ungeraden Grades haben mindestens eine reelle Nullstelle; komplexe Nullstellen treten als **konjugierte Paare** auf. → [[Fundamentalsatz der Algebra]]

**Lösungsstrategie** (typischer Prüfungsablauf): (1) eine Nullstelle $x_1$ **raten** (Teiler von $a_0$ testen), (2) mit [[Polynomdivision]] den Faktor $(x-x_1)$ abspalten, (3) Restpolynom weiter zerlegen (quadratischer Rest mit [[Mitternachtsformel]]).

> [!beispiel] Kubische Gleichung lösen #beispiel
> $x^3-2x^2-5x+6=0$.
> (1) Raten: $x=1$: $1-2-5+6=0$ ✓.
> (2) [[Polynomdivision]]: $(x^3-2x^2-5x+6):(x-1)=x^2-x-6$.
> (3) $x^2-x-6=0\Rightarrow x=\frac{1\pm\sqrt{25}}{2}\Rightarrow x_2=3,\ x_3=-2$.
> Lösungsmenge $\mathbb{L}=\{-2,1,3\}$, Faktorisierung $(x+2)(x-1)(x-3)$.

## 4. Komplexe Zahlen — Grundlagen

> [!definition] Imaginäre Einheit und komplexe Zahl #definition #formel
> Die **imaginäre Einheit** $i$ ist durch $i^2=-1$ definiert. Eine **komplexe Zahl** ist $z=a+bi$ mit $a=\operatorname{Re}(z)\in\mathbb{R}$ (Realteil) und $b=\operatorname{Im}(z)\in\mathbb{R}$ (Imaginärteil).
> - **Konjugiert:** $\bar z=a-bi$ — **Betrag:** $|z|=\sqrt{a^2+b^2}$ — und $z\bar z=a^2+b^2=|z|^2$.

Rechenregeln, Polarform, geometrische Deutung: [[Komplexe Zahlen]].

> [!beispiel] Rechnen in $\mathbb{C}$ #beispiel
> $(2+3i)(1-5i)=2-10i+3i-15i^2=2-7i+15=17-7i$. $\quad\dfrac{1}{2+3i}=\dfrac{2-3i}{13}$ (mit $\bar z$ erweitern).

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. Geben Sie eine präzise Definition einer Menge an und erklären Sie $\subseteq$, $\cup$, $\cap$, $\setminus$ am Venn-Diagramm.
> 2. **Warum** erweitert man die Zahlenbereiche schrittweise? Geben Sie zu jedem Übergang eine Gleichung an, die erst danach lösbar wird.
> 3. Was bedeutet „$\mathbb{Q}$ abzählbar, $\mathbb{R}$ überabzählbar"? Wie unterscheiden sich rationale und irrationale Zahlen in der Dezimaldarstellung?
> 4. Formulieren Sie den Fundamentalsatz der Algebra. Wie viele Lösungen hat $x^4+1=0$ in $\mathbb{R}$ bzw. $\mathbb{C}$?
> 5. Beschreiben Sie das Verfahren zur Bestimmung der Nullstellen eines Polynoms 3. Grades.

## Verwandte Themen
[[TP02 Lineare & quadratische Modelle]] · [[TP08 Funktionen & Polynomfunktionen]] · [[Mitternachtsformel]] · [[Satz von Vieta]] · [[Komplexe Zahlen]] · [[Fundamentalsatz der Algebra]] · [[Polynomdivision]]
