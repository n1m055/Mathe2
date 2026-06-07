---
themenpool: 16
titel: "Beschreibende Statistik und Grundlagen der Wahrscheinlichkeitsrechnung"
gebiet: Stochastik
tags: [themenpool, stochastik, statistik, wahrscheinlichkeit, kennzahlen]
quelle: ["Themenpool 16", "Notizbuch 6B (2023/24)", "Notizbuch 8B (2025/26)"]
verwandt: ["[[TP17 Diskrete Verteilungen]]", "[[Kennzahlen der Statistik]]", "[[Bedingte Wahrscheinlichkeit]]"]
---

# TP16 — Beschreibende Statistik & Grundlagen der Wahrscheinlichkeit

> [!info] Leitidee
> **Beschreibende Statistik** verdichtet Daten zu **Kennzahlen** und Grafiken. Die **Wahrscheinlichkeitsrechnung** quantifiziert den Zufall — von der Laplace-Formel über Baumdiagramme bis zur bedingten Wahrscheinlichkeit. Beides ist Grundlage der [[TP17 Diskrete Verteilungen|Verteilungen]].
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 16]] · Notizbuch **6B/8B**

## 1. Beschreibende Statistik

> [!definition] Lagemaße #definition #formel
> Für Daten $x_1,\dots,x_n$:
> - **Arithmetisches Mittel** $\bar x=\frac{1}{n}\sum_{i=1}^{n}x_i$ (nutzt alle Werte, ausreißerempfindlich).
> - **Median** $\tilde x$ = mittlerer Wert der **geordneten** Liste (robust gegen Ausreißer).
> - **Modus** = häufigster Wert.

> [!definition] Streumaße #definition #formel
> - **Spannweite** $R=x_{\max}-x_{\min}$.
> - **Varianz** $s^2=\frac{1}{n}\sum(x_i-\bar x)^2$, **Standardabweichung** $s=\sqrt{s^2}$ (mittlere Abweichung vom Mittel).
> - **Quartile** $Q_1,Q_2{=}\tilde x,Q_3$; **Interquartilsabstand** $Q_3-Q_1$ → Boxplot. Übersicht: [[Kennzahlen der Statistik]].

![[boxplot.svg|520]]
*Abbildung: Ein Boxplot zeigt Minimum, $Q_1$, Median ($Q_2$), $Q_3$ und Maximum; die Box umfasst die mittleren 50 % der Daten.*

> [!merke] Mittelwerte vergleichen #merke
> $\bar x>\tilde x$ deutet auf eine **rechtsschiefe** Verteilung (wenige große Werte). Der Median ist robuster, weil er Ausreißer ignoriert.

> [!beispiel] Kennzahlen #beispiel
> Daten $2,3,3,5,12$: $\bar x=5$, Median $=3$, Modus $=3$, $R=10$. $\bar x>\tilde x$, weil $12$ ein Ausreißer ist.

## 2. Grundlagen der Wahrscheinlichkeit

> [!definition] Zufallsexperiment, Ereignis, Wahrscheinlichkeit #definition #formel
> Ein **Zufallsexperiment** hat die Ergebnismenge $\Omega$ (alle möglichen Ausgänge). Ein **Ereignis** ist eine Teilmenge $A\subseteq\Omega$. Bei **Laplace-Experimenten** (alle Ergebnisse gleich wahrscheinlich):
> $$P(A)=\frac{|A|}{|\Omega|}=\frac{\text{günstige}}{\text{mögliche}},\qquad 0\le P(A)\le1,\ P(\Omega)=1.$$

> [!satz] Rechenregeln #satz #formel
> - **Gegenereignis:** $P(\bar A)=1-P(A)$.
> - **Additionssatz:** $P(A\cup B)=P(A)+P(B)-P(A\cap B)$.
> - **Unvereinbar** ($A\cap B=\varnothing$): $P(A\cup B)=P(A)+P(B)$.
> - **Unabhängig:** $P(A\cap B)=P(A)\cdot P(B)$.

> [!satz] Baumdiagramme & Pfadregeln #satz #merke
> - **Produktregel:** Wahrscheinlichkeiten **entlang** eines Pfades multiplizieren.
> - **Summenregel:** Wahrscheinlichkeiten **mehrerer** günstiger Pfade addieren.

> [!definition] Bedingte Wahrscheinlichkeit #definition #formel
> $$P(A\mid B)=\frac{P(A\cap B)}{P(B)}\qquad(P(B)>0).$$
> „Wahrscheinlichkeit von $A$, gegeben dass $B$ eingetreten ist." Bayes & Vierfeldertafel: [[Bedingte Wahrscheinlichkeit]].

> [!beispiel] Baumdiagramm #beispiel
> Urne: 3 rote, 2 blaue Kugeln, ohne Zurücklegen zwei ziehen. $P(\text{beide rot})=\frac{3}{5}\cdot\frac{2}{4}=0{,}3$.

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. **Definieren Sie** arithmetisches Mittel, Median und Standardabweichung. Wann ist der Median aussagekräftiger?
> 2. Wie liest man einen Boxplot? Welche Kennzahlen stecken darin?
> 3. Formulieren Sie die Laplace-Definition und die wichtigsten Rechenregeln.
> 4. Erklären Sie Produkt- und Summenregel am Baumdiagramm.
> 5. Was ist eine bedingte Wahrscheinlichkeit? Rechnen Sie ein Beispiel mit Vierfeldertafel.

## Verwandte Themen
[[TP17 Diskrete Verteilungen]] · [[TP18 Stetige Verteilungen]] · [[Kennzahlen der Statistik]] · [[Bedingte Wahrscheinlichkeit]] · [[TP01 Zahlenbereiche & Mengen]]
