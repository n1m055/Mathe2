---
typ: konzept
titel: "Logarithmus"
tags: [konzept, definition, formel, funktionen]
verwandt: ["[[TP09 Exponential- & Logarithmusfunktion]]", "[[Wachstums- und Zerfallsmodelle]]"]
---

# Logarithmus

> [!definition] Definition #definition #formel
> Der **Logarithmus** von $x$ zur Basis $b$ ist der Exponent, mit dem man $b$ potenzieren muss, um $x$ zu erhalten:
> $$y=\log_b x \iff b^{y}=x\qquad(b>0,\ b\neq1,\ x>0).$$
> Er ist die **Umkehrfunktion** der Exponentialfunktion. Spezialfälle: $\ln=\log_e$, $\lg=\log_{10}$.

![[logarithmus.svg|420]]
*Abbildung: $\ln x$ als Spiegelung von $e^x$ an der Geraden $y=x$.*

> [!satz] Rechenregeln (Logarithmengesetze) #satz #formel
> $$\log(uv)=\log u+\log v,\quad \log\tfrac{u}{v}=\log u-\log v,\quad \log(u^r)=r\log u.$$
> **Basiswechsel:** $\log_b x=\dfrac{\ln x}{\ln b}$.

> [!merke] Graph #merke
> $D=(0;\infty)$, $W=\mathbb{R}$, Nullstelle bei $x=1$, senkrechte Asymptote $x=0$, streng monoton steigend (für $b>1$).

> [!beispiel] Gleichung lösen #beispiel
> $5\cdot1{,}03^{t}=20\Rightarrow1{,}03^{t}=4\Rightarrow t=\frac{\ln4}{\ln1{,}03}\approx46{,}9$.

Verwendet in: [[TP09 Exponential- & Logarithmusfunktion]] · [[Wachstums- und Zerfallsmodelle]].
