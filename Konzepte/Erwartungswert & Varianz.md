---
typ: konzept
titel: "Erwartungswert & Varianz (Zufallsvariable)"
tags: [konzept, formel, stochastik, zufallsvariable]
verwandt: ["[[TP17 Diskrete Verteilungen]]", "[[Binomialverteilung]]", "[[Kennzahlen der Statistik]]"]
---

# Erwartungswert & Varianz

> [!definition] Definition #definition #formel
> Diskrete Zufallsvariable $X$ mit $P(X=x_i)=p_i$:
> $$E(X)=\mu=\sum_i x_i p_i$$
> $$V(X)=\sigma^2=\sum_i (x_i-\mu)^2 p_i = E(X^2)-\mu^2,\qquad \sigma=\sqrt{V(X)}$$

> [!note] Deutung #merke
> - $E(X)$ = langfristiger **Durchschnitt** bei sehr vielen Wiederholungen (Schwerpunkt der Verteilung).
> - $\sigma$ = typische **Streuung** um $\mu$.
> - **Faires Spiel:** $E(\text{Gewinn})=0$.

> [!important] Rechenregeln #formel
> $E(aX+b)=a\,E(X)+b$, $\;V(aX+b)=a^2 V(X)$. Bei Unabhängigkeit $E(X+Y)=E(X)+E(Y)$, $V(X+Y)=V(X)+V(Y)$.

> [!example] Beispiel #beispiel
> Würfel: $E(X)=3{,}5$, $V(X)=E(X^2)-\mu^2=\frac{91}{6}-12{,}25\approx2{,}92$, $\sigma\approx1{,}71$.

Statistik-Pendant (Datenlisten): [[Kennzahlen der Statistik]]. Spezialfall: [[Binomialverteilung]]. Theorie: [[TP17 Diskrete Verteilungen]].
