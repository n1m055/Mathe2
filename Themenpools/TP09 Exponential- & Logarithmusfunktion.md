---
themenpool: 9
titel: "Exponential- und Logarithmusfunktion: Wachstums- und Abnahmeprozesse"
gebiet: Funktionen
tags: [themenpool, funktionen, exponentialfunktion, logarithmus, wachstum]
quelle: ["Themenpool 9", "Notizbuch 6B (2023/24)"]
verwandt: ["[[TP08 Funktionen & Polynomfunktionen]]", "[[TP11 Grundlagen Differentialrechnung]]", "[[Wachstums- und Zerfallsmodelle]]"]
---

# TP09 — Exponential- & Logarithmusfunktion

> [!info] Leitidee
> Die Exponentialfunktion beschreibt Prozesse mit **konstantem prozentuellem** Wachstum/Zerfall — jeder gleich große Schritt multipliziert mit demselben **Faktor** (im Gegensatz zur konstanten *Differenz* beim linearen Modell). Der **Logarithmus** ist die Umkehrung und beantwortet „mit welchem Exponenten?".
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 9]] · Notizbuch **6B**

## 1. Exponentialfunktion

> [!definition] Exponentialfunktion #definition #formel
> $$f(x)=a\cdot b^{x}\quad(a>0,\ b>0,\ b\neq1)\qquad\text{bzw.}\qquad f(x)=a\cdot e^{\lambda x}.$$
> Die Variable steht im **Exponenten**. $a=f(0)$ ist der **Anfangswert**, $b$ der **Wachstumsfaktor** ($b>1$ Wachstum, $0<b<1$ Zerfall). Die **Eulersche Zahl** $e\approx2{,}718$ ist die natürliche Basis mit $(e^x)'=e^x$.

> [!definition] Eigenschaften des Graphen #definition #merke
> - **Wertemenge** $W=(0;\infty)$ — der Graph ist **immer positiv**, die $x$-Achse ist waagrechte **Asymptote**.
> - streng monoton, **keine Nullstelle**, geht durch $(0\mid a)$.

![[exponential-vs-linear.svg|500]]
*Abbildung: Exponentielles Wachstum ($2^x$) überholt jedes lineare Wachstum ($1+4x$) — bei der Exponentialfunktion ist der Wachstums*faktor* konstant, bei der linearen die Differenz.*

> [!formel] Umrechnung der Basen #formel #merke
> $$b^x=e^{x\ln b}\quad\Rightarrow\quad \lambda=\ln b.$$
> Jedes Wachstum lässt sich mit Basis $e$ schreiben; $\lambda>0$ Wachstum, $\lambda<0$ Zerfall.

## 2. Logarithmusfunktion

> [!definition] Logarithmus #definition #formel
> Der **Logarithmus** ist die Umkehrfunktion der Exponentialfunktion:
> $$y=\log_b x \iff b^{y}=x\qquad(x>0).$$
> Er beantwortet: „Mit welchem Exponenten muss ich $b$ potenzieren, um $x$ zu erhalten?" $D=(0;\infty)$, $W=\mathbb{R}$, Nullstelle bei $x=1$, senkrechte Asymptote $x=0$. Spezialfall **natürlicher Logarithmus** $\ln=\log_e$.

![[logarithmus.svg|440]]
*Abbildung: $\ln x$ ist die Spiegelung von $e^x$ an der Geraden $y=x$ (Umkehrfunktion).*

> [!satz] Logarithmengesetze #satz #formel
> $$\log(uv)=\log u+\log v,\quad \log\tfrac{u}{v}=\log u-\log v,\quad \log(u^{r})=r\log u.$$
> Anwendungen & Basiswechsel: [[Logarithmus]].

> [!beispiel] Exponentialgleichung lösen #beispiel
> $3\cdot2^{x}=96\Rightarrow2^{x}=32\Rightarrow x=\log_2 32=5$. Allgemein $b^x=c\Rightarrow x=\frac{\ln c}{\ln b}$.

## 3. Wachstums- und Abnahmeprozesse

> [!satz] Modelltypen #satz #merke
> | Modell | Gleichung | Kennzeichen |
> |---|---|---|
> | linear | $N(t)=N_0+k t$ | konstante **Differenz** pro Schritt |
> | exponentiell | $N(t)=N_0 b^{t}=N_0 e^{\lambda t}$ | konstanter **Faktor** pro Schritt |
>
> - **Verdopplungszeit:** $t_2=\frac{\ln2}{\lambda}$ — **Halbwertszeit:** $t_{1/2}=\frac{\ln2}{|\lambda|}$.
> - Kontinuierlich gilt $N'(t)=\lambda N(t)$: die Änderungsrate ist **proportional zum Bestand** (Brücke zur [[TP11 Grundlagen Differentialrechnung|Differentialrechnung]]). Weitere Modelle (begrenzt, logistisch): [[Wachstums- und Zerfallsmodelle]].

> [!beispiel] Radioaktiver Zerfall #beispiel
> C-14, Halbwertszeit 5730 a: $N(t)=N_0 e^{\lambda t}$ mit $\lambda=-\frac{\ln2}{5730}\approx-1{,}21\cdot10^{-4}\,\text{a}^{-1}$. Noch 30 %: $0{,}3=e^{\lambda t}\Rightarrow t=\frac{\ln0{,}3}{\lambda}\approx9953$ Jahre.

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. **Definieren Sie die Exponentialfunktion** und nennen Sie die Eigenschaften ihres Graphen (Asymptote, Monotonie, Nullstellen).
> 2. Vergleichen Sie lineares und exponentielles Wachstum an Term, Tabelle und Graph.
> 3. Definieren Sie den Logarithmus als Umkehrfunktion und nennen Sie die Rechenregeln.
> 4. Leiten Sie die Halbwertszeit-Formel aus $N(t)=N_0e^{\lambda t}$ her.
> 5. Warum ist $e$ eine besondere Basis? *(Transfer zur Ableitung)*

## Verwandte Themen
[[TP08 Funktionen & Polynomfunktionen]] · [[TP11 Grundlagen Differentialrechnung]] · [[Logarithmus]] · [[Wachstums- und Zerfallsmodelle]]
