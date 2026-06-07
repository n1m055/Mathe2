---
typ: konzept
titel: "Bedingte Wahrscheinlichkeit"
tags: [konzept, definition, formel, satz, stochastik]
verwandt: ["[[TP16 Statistik & Wahrscheinlichkeit]]"]
---

# Bedingte Wahrscheinlichkeit

> [!definition] Definition #definition #formel
> Die **bedingte Wahrscheinlichkeit** von $A$ unter der Bedingung $B$ ist
> $$P(A\mid B)=\frac{P(A\cap B)}{P(B)}\qquad(P(B)>0).$$
> Sie misst die Wahrscheinlichkeit von $A$, **wenn man bereits weiß**, dass $B$ eingetreten ist.

![[venn.svg|440]]
*Abbildung: $P(A\mid B)$ betrachtet nur noch den Bereich $B$ als „neue Grundmenge" und fragt nach dem Anteil $A\cap B$ darin.*

> [!satz] Multiplikationssatz & Bayes #satz #formel
> $$P(A\cap B)=P(B)\cdot P(A\mid B)=P(A)\cdot P(B\mid A)$$
> **Satz von Bayes:** $P(A\mid B)=\dfrac{P(B\mid A)\,P(A)}{P(B)}$.
> **Unabhängigkeit:** $A,B$ unabhängig $\iff P(A\mid B)=P(A)\iff P(A\cap B)=P(A)P(B)$.

> [!beispiel] Beispiel (Basisraten-Falle) #beispiel
> Krankheit $P(K)=1\%$, Sensitivität $P(+\mid K)=99\%$, Falsch-Positiv $P(+\mid\bar K)=5\%$.
> $P(+)=0{,}01\cdot0{,}99+0{,}99\cdot0{,}05=0{,}0594$, also $P(K\mid+)=\frac{0{,}0099}{0{,}0594}\approx16{,}7\%$ — trotz positivem Test eher gesund.

Theorie: [[TP16 Statistik & Wahrscheinlichkeit]].
