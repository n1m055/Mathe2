---
themenpool: 18
titel: "Stetige Wahrscheinlichkeitsverteilungen"
gebiet: Stochastik
tags: [themenpool, stochastik, normalverteilung, dichtefunktion, approximation]
quelle: ["Themenpool 18", "Notizbuch 8B (2025/26)"]
verwandt: ["[[TP17 Diskrete Verteilungen]]", "[[Normalverteilung]]", "[[Binomialverteilung]]"]
---

# TP18 — Stetige Wahrscheinlichkeitsverteilungen

> [!info] Leitidee
> Bei **stetigen** Zufallsvariablen (Länge, Gewicht, Zeit) gibt es überabzählbar viele Werte — Wahrscheinlichkeiten werden zu **Flächen unter einer Dichtefunktion** ([[TP14 Grundlagen Integralrechnung|Integral]]). Die wichtigste stetige Verteilung ist die **Normalverteilung**; sie approximiert auch die [[Binomialverteilung]].
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 18]] · Notizbuch **8B**

## 1. Dichtefunktion

> [!definition] Stetige Zufallsvariable, Dichtefunktion #definition #formel
> Eine Zufallsvariable $X$ heißt **stetig**, wenn ihre Wahrscheinlichkeiten durch eine **Dichtefunktion** $f$ mit $f(x)\ge0$ und $\int_{-\infty}^{\infty}f(x)\,dx=1$ beschrieben werden:
> $$P(a\le X\le b)=\int_a^b f(x)\,dx.$$
> **Folge:** $P(X=a)=0$ für jeden Einzelwert (Fläche der Breite 0); daher ist es egal, ob $\le$ oder $<$.

## 2. Normalverteilung

> [!definition] Normalverteilung #definition #satz #formel
> $X$ ist **normalverteilt**, $X\sim N(\mu,\sigma^2)$, mit der Dichte
> $$\varphi(x)=\frac{1}{\sigma\sqrt{2\pi}}\,e^{-\frac{1}{2}\left(\frac{x-\mu}{\sigma}\right)^2}.$$
> Sie ist **glockenförmig**, symmetrisch um den Erwartungswert $\mu$ (= Median = Modus); $\sigma$ steuert die Breite, die Wendestellen liegen bei $\mu\pm\sigma$. Vollständig: [[Normalverteilung]].

![[normalverteilung.svg|560]]
*Abbildung: Glockenkurve mit den $\sigma$-Bereichen — rund 68 %, 95 % bzw. 99,7 % der Werte liegen innerhalb von einer, zwei bzw. drei Standardabweichungen um $\mu$.*

> [!satz] σ-Regeln #satz #formel
> $$P(\mu-\sigma\le X\le\mu+\sigma)\approx68{,}3\%,\quad \pm2\sigma\approx95{,}4\%,\quad \pm3\sigma\approx99{,}7\%.$$

> [!satz] Standardisierung #satz #formel
> $$Z=\frac{X-\mu}{\sigma}\sim N(0,1),\qquad P(X\le x)=\Phi\!\left(\frac{x-\mu}{\sigma}\right),$$
> wobei $\Phi$ die tabellierte Verteilungsfunktion der Standardnormalverteilung ist. So werden beliebige Normalverteilungen vergleichbar.

> [!beispiel] Normalverteilung anwenden #beispiel
> Körpergröße $X\sim N(178,\,7^2)$ cm: $P(X\le185)=\Phi\!\big(\frac{185-178}{7}\big)=\Phi(1)\approx0{,}841$ → ca. 84 %. Mit der $1\sigma$-Regel liegen ca. 68 % zwischen 171 und 185 cm.

## 3. Normalapproximation der Binomialverteilung

> [!satz] Approximation #satz #formel
> Für großes $n$ (Laplace-Bedingung $\sigma=\sqrt{np(1-p)}>3$):
> $$X\sim B(n,p)\ \approx\ N\big(\mu=np,\ \sigma^2=np(1-p)\big).$$
> Man ersetzt die Summe vieler Binomialwahrscheinlichkeiten durch **eine** Normalverteilungsfläche (genauer mit Stetigkeitskorrektur $\pm0{,}5$).

> [!beispiel] Approximation #beispiel
> $X\sim B(100;\,0{,}5)$: $\mu=50$, $\sigma=5$. $P(X\le60)\approx\Phi\!\big(\frac{60-50}{5}\big)=\Phi(2)\approx0{,}977$.

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. **Definieren Sie die Dichtefunktion.** Warum ist $P(X=a)=0$ bei stetigen Verteilungen?
> 2. Beschreiben Sie Form und Eigenschaften der Normalverteilung ($\mu,\sigma$, Symmetrie, Wendestellen).
> 3. Erklären Sie die σ-Regeln anhand der Abbildung.
> 4. Was bedeutet **Standardisierung** und wozu braucht man sie?
> 5. Wann und wie approximiert man die Binomial- durch die Normalverteilung?

## Verwandte Themen
[[TP17 Diskrete Verteilungen]] · [[TP16 Statistik & Wahrscheinlichkeit]] · [[TP14 Grundlagen Integralrechnung]] · [[Normalverteilung]] · [[Binomialverteilung]]
