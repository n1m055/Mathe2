---
typ: konzept
titel: "Stammfunktion & Integrationsregeln"
tags: [konzept, formel, analysis, integral]
verwandt: ["[[Ableitungsregeln]]", "[[Hauptsatz der Differential- und Integralrechnung]]", "[[TP14 Grundlagen Integralrechnung]]"]
---

# Stammfunktion & Integrationsregeln

> [!definition] Stammfunktion #definition #formel
> $F$ ist Stammfunktion von $f$, wenn $F'(x)=f(x)$. Eindeutig nur bis auf Konstante:
> $$\int f(x)\,dx=F(x)+C$$

> [!important] Grundintegrale #formel
> | $f(x)$ | $\int f\,dx$ |
> |---|---|
> | $x^n\ (n\neq-1)$ | $\dfrac{x^{n+1}}{n+1}+C$ |
> | $\dfrac{1}{x}$ | $\ln|x|+C$ |
> | $e^{x}$ | $e^{x}+C$ |
> | $\sin x$ | $-\cos x+C$ |
> | $\cos x$ | $\sin x+C$ |

> [!important] Regeln #formel #merke
> - **Faktor-/Summenregel:** $\int c\,f=c\int f$, $\int(f\pm g)=\int f\pm\int g$.
> - **Lineare Substitution:** $\int f(ax+b)\,dx=\frac{1}{a}F(ax+b)+C$.
> - ⚠️ Es gibt **keine** allgemeine Produkt-/Quotienten-/Kettenregel fürs Integrieren — Integrieren ist schwieriger als Ableiten!

> [!example] Beispiel #beispiel
> $\int(6x^2-4x+5)\,dx=2x^3-2x^2+5x+C$. $\;\int e^{-2x}dx=-\tfrac12 e^{-2x}+C$.

Umkehrung = [[Ableitungsregeln]]. Bestimmtes Integral berechnen mit [[Hauptsatz der Differential- und Integralrechnung]]. Theorie: [[TP14 Grundlagen Integralrechnung]].
