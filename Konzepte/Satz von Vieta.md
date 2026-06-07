---
typ: konzept
titel: "Satz von Vieta"
tags: [konzept, satz, formel, algebra]
verwandt: ["[[Mitternachtsformel]]", "[[TP02 Lineare & quadratische Modelle]]"]
---

# Satz von Vieta

> [!satz] Satz #satz #formel
> Hat $x^2+px+q=0$ die Lösungen $x_1,x_2$, so gilt:
> $$x_1+x_2=-p,\qquad x_1\cdot x_2=q$$
> Allgemein für $ax^2+bx+c=0$: $\;x_1+x_2=-\frac{b}{a}$, $\;x_1 x_2=\frac{c}{a}$.

> [!note] Begründung #herleitung
> Aus der Faktorisierung $x^2+px+q=(x-x_1)(x-x_2)=x^2-(x_1+x_2)x+x_1x_2$ folgt durch Koeffizientenvergleich $p=-(x_1+x_2)$ und $q=x_1x_2$. ∎

> [!tip] Wozu? #merke
> - **Lösungen kontrollieren** (schnelle Probe).
> - **Faktorisieren** / Lösungen raten (Teiler von $q$).
> - Rückwärts: quadratische Gleichung aus gegebenen Nullstellen aufstellen.

> [!example] Beispiel #beispiel
> $x^2-5x+6=0$: gesucht zwei Zahlen mit Summe $5$ und Produkt $6$ → $2$ und $3$. Also $x_1=2,\ x_2=3$.

Verwendet in: [[TP02 Lineare & quadratische Modelle]] · [[TP01 Zahlenbereiche & Mengen]] · [[TP08 Funktionen & Polynomfunktionen]].
