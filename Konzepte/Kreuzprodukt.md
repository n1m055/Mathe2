---
typ: konzept
titel: "Kreuzprodukt (Vektorprodukt)"
tags: [konzept, definition, formel, geometrie, vektoren, raum]
verwandt: ["[[Skalarprodukt]]", "[[TP05 Vektoren in R3]]"]
---

# Kreuzprodukt (Vektorprodukt)

> [!definition] Definition (nur im $\mathbb{R}^3$) #definition #formel
> Das **Kreuzprodukt** zweier Vektoren $\vec a,\vec b\in\mathbb{R}^3$ ist der Vektor
> $$\vec a\times\vec b=\begin{pmatrix}a_2b_3-a_3b_2\\a_3b_1-a_1b_3\\a_1b_2-a_2b_1\end{pmatrix}.$$
> Das Ergebnis ist ein **Vektor** (anders als beim [[Skalarprodukt]]).

![[kreuzprodukt.svg|420]]
*Abbildung: $|\vec a\times\vec b|$ ist der Flächeninhalt des aufgespannten Parallelogramms; der Vektor selbst steht senkrecht darauf.*

> [!formel] Bedeutung #formel #merke
> - $\vec a\times\vec b\perp\vec a$ und $\perp\vec b$ → **Normalvektor** einer Ebene (Richtung per Rechte-Hand-Regel).
> - $|\vec a\times\vec b|=|\vec a||\vec b|\sin\varphi$ = **Flächeninhalt** des Parallelogramms; Dreieck $=\tfrac12|\vec a\times\vec b|$.
> - $\vec a\times\vec b=\vec0\iff\vec a\parallel\vec b$.

> [!merke] Eigenschaften #merke
> Antikommutativ: $\vec a\times\vec b=-(\vec b\times\vec a)$. **Spatprodukt** $(\vec a\times\vec b)\cdot\vec c$ = Volumen des Spats.

> [!beispiel] Beispiel #beispiel
> $\vec a=(1,0,2),\ \vec b=(0,3,1)$: $\vec a\times\vec b=(-6,-1,3)$. Probe $\vec a\cdot(\vec a\times\vec b)=-6+0+6=0$ ✓.

Verwendet in: [[TP05 Vektoren in R3]]. Gegenstück: [[Skalarprodukt]].
