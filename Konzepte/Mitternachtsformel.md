---
typ: konzept
titel: "Mitternachtsformel (Lösungsformel quadratischer Gleichungen)"
tags: [konzept, formel, algebra, herleitung]
verwandt: ["[[TP02 Lineare & quadratische Modelle]]", "[[Satz von Vieta]]"]
---

# Mitternachtsformel

> [!formel] Lösungsformel #formel
> Für $ax^2+bx+c=0$ ($a\neq0$):
> $$x_{1,2}=\frac{-b\pm\sqrt{\,b^2-4ac\,}}{2a}$$
> **Diskriminante** $D=b^2-4ac$: $D>0$ zwei, $D=0$ eine (doppelte), $D<0$ keine reelle Lösung (zwei komplexe → [[Komplexe Zahlen]]).

> [!note] Herleitung (quadratische Ergänzung) #herleitung
> $ax^2+bx+c=0 \mid :a \Rightarrow x^2+\frac{b}{a}x+\frac{c}{a}=0$.
> $x^2+\frac{b}{a}x=-\frac{c}{a}$, quadratisch ergänzen mit $\left(\frac{b}{2a}\right)^2$:
> $$\left(x+\frac{b}{2a}\right)^2=\frac{b^2}{4a^2}-\frac{c}{a}=\frac{b^2-4ac}{4a^2}.$$
> Wurzelziehen: $x+\frac{b}{2a}=\pm\frac{\sqrt{b^2-4ac}}{2a}$ → Formel. ∎

> [!note] Spezialfall — kleine Lösungsformel (pq-Formel) #formel
> Für $x^2+px+q=0$: $\;x_{1,2}=-\frac{p}{2}\pm\sqrt{\left(\frac{p}{2}\right)^2-q}$. Kontrolle über [[Satz von Vieta]].

Verwendet in: [[TP02 Lineare & quadratische Modelle]] · [[TP01 Zahlenbereiche & Mengen]] · [[TP07 Kegelschnitte]] (Diskriminante für Tangenten).
