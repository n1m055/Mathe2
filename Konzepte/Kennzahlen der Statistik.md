---
typ: konzept
titel: "Kennzahlen der beschreibenden Statistik"
tags: [konzept, definition, formel, stochastik, statistik]
verwandt: ["[[TP16 Statistik & Wahrscheinlichkeit]]", "[[Erwartungswert & Varianz]]"]
---

# Kennzahlen der Statistik

> [!definition] Lagemaße #definition #formel
> Für Daten $x_1,\dots,x_n$:
> - **Arithmetisches Mittel** $\bar x=\frac{1}{n}\sum x_i$ (nutzt alle Werte, ausreißerempfindlich).
> - **Median** $\tilde x$: mittlerer Wert der geordneten Liste (robust).
> - **Modus:** häufigster Wert.

> [!definition] Streumaße #definition #formel
> - **Spannweite** $R=x_{\max}-x_{\min}$.
> - **Varianz** $s^2=\frac{1}{n}\sum(x_i-\bar x)^2$, **Standardabweichung** $s=\sqrt{s^2}$.
> - **Quartile** $Q_1,Q_2(=\tilde x),Q_3$; Interquartilsabstand $\text{IQR}=Q_3-Q_1$.

![[boxplot.svg|500]]
*Abbildung: Der Boxplot stellt die fünf Kennzahlen Min, $Q_1$, Median, $Q_3$, Max dar; die Box umfasst die mittleren 50 % der Daten.*

> [!merke] Deutung #merke
> $\bar x>\tilde x$: rechtsschief (wenige große Ausreißer). Kleine $s$ = Werte eng um den Mittelwert. Median/IQR sind robuster gegen Ausreißer als Mittel/Spannweite.

> [!beispiel] Beispiel #beispiel
> $2,3,3,5,12$: $\bar x=5$, $\tilde x=3$, $R=10$, $s\approx3{,}6$.

Wahrscheinlichkeits-Pendant (Zufallsvariablen): [[Erwartungswert & Varianz]]. Theorie: [[TP16 Statistik & Wahrscheinlichkeit]].
