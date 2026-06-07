---
typ: konzept
titel: "Binomialverteilung"
tags: [konzept, definition, formel, satz, stochastik, verteilung]
verwandt: ["[[Erwartungswert & Varianz]]", "[[Normalverteilung]]", "[[TP17 Diskrete Verteilungen]]"]
---

# Binomialverteilung

> [!definition] Definition #definition #satz #formel
> Bei einer **Bernoulli-Kette** ($n$ unabhängige Versuche, je „Erfolg/Misserfolg" mit konstanter Erfolgswahrscheinlichkeit $p$) ist die Anzahl $X$ der Erfolge **binomialverteilt**:
> $$P(X=k)=\binom{n}{k}\,p^{k}(1-p)^{\,n-k},\quad k=0,1,\dots,n.$$
> $$E(X)=n p,\qquad V(X)=n p(1-p),\qquad \sigma=\sqrt{n p(1-p)}.$$
> $\binom{n}{k}=\frac{n!}{k!(n-k)!}$ = Anzahl der Reihenfolgen der $k$ Erfolge.

![[binomialverteilung.svg|500]]
*Abbildung: $B(10;\,0{,}5)$ — symmetrische Säulen um $E(X)=5$.*

> [!merke] Kumuliert / Gegenereignis #merke
> „Höchstens $k$": $P(X\le k)=\sum_{i=0}^k P(X=i)$. „Mindestens 1": $P(X\ge1)=1-P(X=0)$.

> [!beispiel] Beispiel #beispiel
> $n=10,\ p=0{,}5$: $P(X=5)=\binom{10}{5}0{,}5^{10}\approx0{,}246$; $E(X)=5$, $\sigma\approx1{,}58$.

> [!merke] Approximation #merke
> Für großes $n$ ($\sigma>3$): $B(n,p)\approx N(np,\,np(1-p))$ → [[Normalverteilung]].

Kennzahlen allgemein: [[Erwartungswert & Varianz]]. Theorie: [[TP17 Diskrete Verteilungen]].
