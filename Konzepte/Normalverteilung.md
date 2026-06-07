---
typ: konzept
titel: "Normalverteilung"
tags: [konzept, definition, formel, satz, stochastik, verteilung]
verwandt: ["[[Binomialverteilung]]", "[[TP18 Stetige Verteilungen]]"]
---

# Normalverteilung

> [!definition] Definition #definition #formel
> Eine stetige Zufallsvariable $X$ ist **normalverteilt**, $X\sim N(\mu,\sigma^2)$, wenn sie die Dichte
> $$\varphi(x)=\frac{1}{\sigma\sqrt{2\pi}}\,e^{-\frac{1}{2}\left(\frac{x-\mu}{\sigma}\right)^2}$$
> besitzt. Die Kurve ist glockenförmig, symmetrisch um $\mu$ (= Median = Modus), mit Wendestellen bei $\mu\pm\sigma$; die Gesamtfläche ist $1$.

![[normalverteilung.svg|540]]
*Abbildung: Glockenkurve mit den σ-Bereichen (68,3 % / 95,4 % / 99,7 %).*

> [!satz] σ-Regeln & Standardisierung #satz #formel
> $$P(|X-\mu|\le\sigma)\approx68{,}3\%,\quad \le2\sigma\approx95{,}4\%,\quad \le3\sigma\approx99{,}7\%$$
> $$Z=\frac{X-\mu}{\sigma}\sim N(0,1),\qquad P(X\le x)=\Phi\!\left(\frac{x-\mu}{\sigma}\right)$$
> $\Phi$ = tabellierte Verteilungsfunktion der Standardnormalverteilung.

> [!beispiel] Beispiel #beispiel
> $X\sim N(178,7^2)$: $P(X\le185)=\Phi(1)\approx0{,}841$. Zwischen 171 und 185 cm liegen ca. 68 % ($1\sigma$).

> [!merke] Approximation #merke
> Ersetzt für großes $n$ die [[Binomialverteilung]]: $\mu=np$, $\sigma=\sqrt{np(1-p)}$.

Wahrscheinlichkeit = Fläche = Integral der Dichte ([[TP14 Grundlagen Integralrechnung]]). Theorie: [[TP18 Stetige Verteilungen]].
