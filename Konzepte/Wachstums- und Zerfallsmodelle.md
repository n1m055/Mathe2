---
typ: konzept
titel: "Wachstums- und Zerfallsmodelle"
tags: [konzept, definition, formel, funktionen, wachstum, anwendung]
verwandt: ["[[TP09 Exponential- & Logarithmusfunktion]]", "[[Logarithmus]]"]
---

# Wachstums- und Zerfallsmodelle

> [!definition] Lineares vs. exponentielles Wachstum #definition #formel
> - **Lineares Wachstum:** konstante **Differenz** pro Zeitschritt, $N(t)=N_0+k\,t$.
> - **Exponentielles Wachstum:** konstanter **Faktor** (Prozentsatz) pro Zeitschritt, $N(t)=N_0\cdot b^{t}=N_0 e^{\lambda t}$.

![[exponential-vs-linear.svg|480]]
*Abbildung: Exponentielles Wachstum überholt jedes lineare — der Unterschied liegt darin, was konstant ist (Faktor vs. Differenz).*

> [!formel] Weitere Modelle & Kennzahlen #formel
> | Typ | Gleichung |
> |---|---|
> | begrenzt | $N(t)=S-(S-N_0)e^{-kt}$ (nähert sich Schranke $S$) |
> | logistisch | $N(t)=\dfrac{S}{1+c\,e^{-kt}}$ (S-Kurve) |
>
> $\lambda=\ln b$, Verdopplungszeit $\frac{\ln2}{\lambda}$, Halbwertszeit $\frac{\ln2}{|\lambda|}$. Es gilt $N'(t)=\lambda N(t)$ — Änderungsrate proportional zum Bestand.

> [!beispiel] Beispiel #beispiel
> Bakterien verdoppeln sich stündlich: $b=2$, $N(t)=N_0\cdot2^t$. Nach 5 h das 32-fache, Verdopplungszeit $=\frac{\ln2}{\ln2}=1$ h.

Gleichungen lösen über [[Logarithmus]]. Theorie: [[TP09 Exponential- & Logarithmusfunktion]].
