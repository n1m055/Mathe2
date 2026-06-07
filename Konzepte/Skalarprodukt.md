---
typ: konzept
titel: "Skalarprodukt (inneres Produkt)"
tags: [konzept, definition, formel, geometrie, vektoren]
verwandt: ["[[Kreuzprodukt]]", "[[TP04 Vektoren in R2]]", "[[TP05 Vektoren in R3]]"]
---

# Skalarprodukt

> [!definition] Definition #definition #formel
> Das **Skalarprodukt** zweier Vektoren ist die Zahl
> $$\vec a\cdot\vec b=\sum_i a_i b_i=|\vec a|\,|\vec b|\cos\varphi,$$
> wobei $\varphi$ der von $\vec a,\vec b$ eingeschlossene Winkel ist. Das Ergebnis ist ein **Skalar** (Zahl), kein Vektor. (2D: $a_1b_1+a_2b_2$; 3D: $a_1b_1+a_2b_2+a_3b_3$.)

![[skalarprodukt.svg|420]]
*Abbildung: Der Winkel $\varphi$ zwischen zwei Vektoren steckt im Skalarprodukt.*

> [!formel] Anwendungen #formel #merke
> - **Winkel:** $\cos\varphi=\dfrac{\vec a\cdot\vec b}{|\vec a||\vec b|}$
> - **Orthogonalität:** $\vec a\perp\vec b\iff\vec a\cdot\vec b=0$
> - **Länge:** $|\vec a|=\sqrt{\vec a\cdot\vec a}$
> - **Projektion** von $\vec a$ auf $\vec b$: $\dfrac{\vec a\cdot\vec b}{|\vec b|}$

> [!merke] Rechenregeln #merke
> Kommutativ $\vec a\cdot\vec b=\vec b\cdot\vec a$, distributiv, $(\lambda\vec a)\cdot\vec b=\lambda(\vec a\cdot\vec b)$. Kein Assoziativgesetz (Ergebnis ist skalar).

> [!beispiel] Beispiel #beispiel
> $\vec a=(2,1),\ \vec b=(1,-1)$: $\vec a\cdot\vec b=2-1=1$, $\cos\varphi=\frac{1}{\sqrt5\sqrt2}\Rightarrow\varphi\approx71{,}6^\circ$.

Verwendet in: [[TP04 Vektoren in R2]] · [[TP05 Vektoren in R3]] · [[TP06 Trigonometrie]]. Vergleiche [[Kreuzprodukt]].
