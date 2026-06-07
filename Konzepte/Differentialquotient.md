---
typ: konzept
titel: "Differenzen- und Differentialquotient"
tags: [konzept, definition, formel, analysis, herleitung]
verwandt: ["[[Ableitungsregeln]]", "[[TP11 Grundlagen Differentialrechnung]]"]
---

# Differenzen- & Differentialquotient

> [!definition] Differenzenquotient (mittlere Änderungsrate) #definition #formel
> $$\frac{\Delta y}{\Delta x}=\frac{f(x_2)-f(x_1)}{x_2-x_1}$$
> = Steigung der **Sekante** = durchschnittliche Änderung im Intervall $[x_1;x_2]$.

> [!definition] Differentialquotient (Ableitung) #definition #formel
> $$f'(x_0)=\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}{h}=\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}$$
> = Steigung der **Tangente** = momentane Änderungsrate (sofern der Grenzwert existiert).

![[sekante-tangente.svg|480]]
*Abbildung: Lässt man den zweiten Punkt auf $x_0$ zuwandern ($h\to0$), geht die Sekante in die Tangente über.*

> [!merke] Drei Deutungen #merke
> geometrisch (Tangentensteigung) · analytisch (Grenzwert) · inhaltlich (momentane Rate: $v=s'$, Grenzkosten $=K'$).

> [!beispiel] Herleitung am Beispiel #herleitung #beispiel
> $f(x)=x^2$: $\dfrac{(x+h)^2-x^2}{h}=2x+h\xrightarrow{h\to0}2x$. Also $f'(x)=2x$.

Fertige Regeln: [[Ableitungsregeln]]. Vertiefung: [[TP11 Grundlagen Differentialrechnung]].
