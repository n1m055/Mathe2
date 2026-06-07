---
themenpool: 17
titel: "Diskrete Wahrscheinlichkeitsverteilungen"
gebiet: Stochastik
tags: [themenpool, stochastik, zufallsvariable, erwartungswert, binomialverteilung]
quelle: ["Themenpool 17", "Notizbuch 8B (2025/26)"]
verwandt: ["[[TP16 Statistik & Wahrscheinlichkeit]]", "[[TP18 Stetige Verteilungen]]", "[[Binomialverteilung]]"]
---

# TP17 — Diskrete Wahrscheinlichkeitsverteilungen

> [!info] Leitidee
> Eine **Zufallsvariable** ordnet jedem Ausgang eine Zahl zu; ihre **Verteilung** sagt, mit welcher Wahrscheinlichkeit jeder Wert auftritt. **Erwartungswert** und **Standardabweichung** verdichten die Verteilung zu „Mittelwert" und „Streuung". Wichtigster Fall: die **Binomialverteilung**.
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 17]] · Notizbuch **8B**

## 1. Zufallsvariable und Kennzahlen

> [!definition] Zufallsvariable, Wahrscheinlichkeitsverteilung #definition
> Eine **Zufallsvariable** $X$ ist eine Funktion, die jedem Ergebnis eines Zufallsexperiments eine reelle Zahl zuordnet. **Diskret** heißt sie, wenn sie nur endlich oder abzählbar viele Werte $x_i$ annimmt. Die **Wahrscheinlichkeitsverteilung** gibt zu jedem Wert die Wahrscheinlichkeit $p_i=P(X=x_i)$ an, mit $\sum_i p_i=1$.

> [!definition] Erwartungswert, Varianz, Standardabweichung #definition #formel
> $$E(X)=\mu=\sum_i x_i\,p_i\qquad\text{(langfristiger Durchschnitt)}$$
> $$V(X)=\sigma^2=\sum_i (x_i-\mu)^2 p_i=E(X^2)-\mu^2,\qquad \sigma=\sqrt{V(X)}.$$
> $\sigma$ misst die Streuung um den Erwartungswert. Vertiefung: [[Erwartungswert & Varianz]].

> [!beispiel] Fairer Würfel #beispiel
> $X$ = Augenzahl: $E(X)=\frac{1}{6}(1+\dots+6)=3{,}5$, $\sigma\approx1{,}71$.

> [!merke] Faires Spiel #merke
> Ein Glücksspiel ist **fair**, wenn $E(\text{Gewinn})=0$. $E(X)>0$ vorteilhaft, $E(X)<0$ auf Dauer Verlust.

## 2. Binomialverteilung

> [!definition] Binomialkoeffizient #definition #formel
> $$\binom{n}{k}=\frac{n!}{k!\,(n-k)!}$$
> = Anzahl der Möglichkeiten, aus $n$ Objekten $k$ **ohne Beachtung der Reihenfolge** auszuwählen (Pascalsches Dreieck).

> [!definition] Binomialverteilung #definition #satz #formel
> **Bernoulli-Kette:** $n$ **unabhängige** Versuche mit je zwei Ausgängen, Erfolgswahrscheinlichkeit $p$ konstant. $X$ = Anzahl der Erfolge ist **binomialverteilt**:
> $$P(X=k)=\binom{n}{k}\,p^{k}(1-p)^{\,n-k},\quad k=0,1,\dots,n.$$
> $$E(X)=n\,p,\qquad \sigma=\sqrt{n\,p\,(1-p)}.$$
> Vollständig: [[Binomialverteilung]].

![[binomialverteilung.svg|520]]
*Abbildung: Wahrscheinlichkeitsverteilung von $X\sim B(10;\,0{,}5)$; symmetrisch um den Erwartungswert $E(X)=5$.*

> [!beispiel] Münzwürfe #beispiel
> Münze 10× werfen, $p=0{,}5$: $P(X=5)=\binom{10}{5}0{,}5^{10}\approx0{,}246$; $E(X)=5$, $\sigma\approx1{,}58$.

> [!merke] „Mindestens / höchstens" #merke
> $P(X\ge1)=1-P(X=0)$ (Gegenereignis). „Höchstens $k$" = kumuliert $\sum_{i=0}^{k}P(X=i)$.

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. **Definieren Sie Zufallsvariable und Erwartungswert.** Deuten Sie $E(X)$ und $\sigma$ anschaulich.
> 2. Wann ist ein Spiel fair? Berechnen Sie $E(X)$ für ein Beispiel.
> 3. Was zählt der Binomialkoeffizient? Bezug zum Pascalschen Dreieck.
> 4. Nennen Sie die **Voraussetzungen** der Binomialverteilung und ihre Formel samt $E(X),\sigma$.
> 5. Berechnen Sie eine „mindestens"-Wahrscheinlichkeit über das Gegenereignis.

## Verwandte Themen
[[TP16 Statistik & Wahrscheinlichkeit]] · [[TP18 Stetige Verteilungen]] · [[Erwartungswert & Varianz]] · [[Binomialverteilung]]
