---
themenpool: 5
titel: "Vektoren im ℝ³: Analytische Geometrie des Raumes"
gebiet: Geometrie
tags: [themenpool, geometrie, vektoren, raum, kreuzprodukt]
quelle: ["Themenpool 5", "Notizbuch 6B (2023/24)"]
verwandt: ["[[TP04 Vektoren in R2]]", "[[TP03 Gleichungssysteme & Ungleichungen]]"]
---

# TP05 — Vektoren im ℝ³: Analytische Geometrie des Raumes

> [!info] Leitidee
> Im Raum kommt eine dritte Koordinate dazu. Alle Begriffe aus [[TP04 Vektoren in R2|ℝ²]] gelten weiter; neu sind das [[Kreuzprodukt]] (liefert einen Normalvektor zu zwei Vektoren) und die **Ebene** als eigenständiges Objekt.
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 5]] · Notizbuch **6B**

## 1. Vektoren im Raum

> [!definition] Vektor im ℝ³ #definition #formel
> Ein **Vektor im Raum** wird durch drei Komponenten dargestellt:
> $$\vec a=\begin{pmatrix}a_1\\a_2\\a_3\end{pmatrix},\qquad |\vec a|=\sqrt{a_1^2+a_2^2+a_3^2}.$$
> Wie in der Ebene ist er die Klasse aller gleich langen, gleich gerichteten parallelen Pfeile; die Koordinaten von $P(p_1\mid p_2\mid p_3)$ sind die Komponenten des Ortsvektors $\overrightarrow{OP}$.

![[vektoren-r3.svg|420]]
*Abbildung: Ortsvektor zum Punkt $P(2\mid3\mid2)$ im räumlichen Koordinatensystem; die gestrichelten Linien zeigen die Komponenten.*

> [!definition] Skalarprodukt im Raum #definition #formel
> $$\vec a\cdot\vec b=a_1b_1+a_2b_2+a_3b_3=|\vec a||\vec b|\cos\varphi,\qquad \vec a\perp\vec b\iff\vec a\cdot\vec b=0.$$
> Misst wie in 2D den Winkel. → [[Skalarprodukt]]

## 2. Vektorielles Produkt (Kreuzprodukt)

> [!definition] Kreuzprodukt #definition #satz #formel
> Für $\vec a,\vec b\in\mathbb{R}^3$:
> $$\vec a\times\vec b=\begin{pmatrix}a_2b_3-a_3b_2\\a_3b_1-a_1b_3\\a_1b_2-a_2b_1\end{pmatrix}.$$
> Das Ergebnis ist ein **Vektor** mit den Eigenschaften:
> - $\vec a\times\vec b$ steht **senkrecht** auf $\vec a$ und $\vec b$ → liefert direkt einen **Normalvektor** einer Ebene.
> - $|\vec a\times\vec b|=|\vec a||\vec b|\sin\varphi$ = **Flächeninhalt** des aufgespannten Parallelogramms.
> - antikommutativ: $\vec a\times\vec b=-(\vec b\times\vec a)$; $\;\vec a\times\vec b=\vec0\iff\vec a\parallel\vec b$.
>
> Spatprodukt/Volumen: [[Kreuzprodukt]].

![[kreuzprodukt.svg|440]]
*Abbildung: Das von $\vec a,\vec b$ aufgespannte Parallelogramm hat den Flächeninhalt $|\vec a\times\vec b|$; der Kreuzproduktvektor steht senkrecht auf der Fläche.*

> [!beispiel] Normalvektor & Dreiecksfläche #beispiel
> $\vec a=(1,0,2),\ \vec b=(0,3,1)$: $\vec a\times\vec b=(0\cdot1-2\cdot3,\ 2\cdot0-1\cdot1,\ 1\cdot3-0\cdot0)=(-6,-1,3)$.
> Probe: $\vec a\cdot(\vec a\times\vec b)=-6+0+6=0$ ✓. Dreiecksfläche $=\tfrac12\sqrt{36+1+9}=\tfrac12\sqrt{46}\approx3{,}39$.

## 3. Geraden und Ebenen im Raum

> [!definition] Gerade und Ebene #definition #formel
> - **Gerade:** $g:\ \vec X=\vec P+t\,\vec r$ (im Raum **nur** Parameterform — keine einfache Hauptform).
> - **Ebene, Parameterform:** $E:\ \vec X=\vec P+s\,\vec u+t\,\vec v$ (Punkt + zwei nicht-parallele Richtungsvektoren).
> - **Ebene, Normalvektorform:** $\vec n\cdot(\vec X-\vec P)=0$ mit $\vec n=\vec u\times\vec v$.
> - **Ebene, Koordinatenform:** $n_1x+n_2y+n_3z=c$.

> [!satz] Lagebeziehungen #satz
> - **Gerade–Gerade:** identisch · parallel · **schneidend** · **windschief**.
> - **Gerade–Ebene:** Gerade liegt in $E$ · parallel · genau ein Schnittpunkt.
> - **Ebene–Ebene:** identisch · parallel · Schnittgerade.
> Rechnerisch: einsetzen → [[TP03 Gleichungssysteme & Ungleichungen|LGS]]; die Lösbarkeit bestimmt die Lage.

> [!definition] Windschief #definition #merke
> Zwei Geraden heißen **windschief**, wenn sie **weder parallel** sind **noch einen Schnittpunkt** haben. Das ist nur im Raum möglich — in der Ebene schneiden sich nicht-parallele Geraden immer.

> [!beispiel] Schnitt Gerade/Ebene #beispiel
> $g:\ \vec X=(1,2,0)+t(1,1,1)$, $E:\ x+y+z=12$. Einsetzen: $(1+t)+(2+t)+t=12\Rightarrow t=3$. Schnittpunkt $S=(4,5,3)$. (Wäre $\vec r\cdot\vec n=0$ und $P\notin E$, so wäre $g$ **parallel** zu $E$, keine Lösung.)

> [!formel] Abstände und Winkel #formel #merke
> - **Winkel Gerade/Ebene:** $\sin\alpha=\dfrac{|\vec r\cdot\vec n|}{|\vec r||\vec n|}$.
> - **Abstand Punkt–Ebene** (Hesse'sche Normalform): $d=\dfrac{|n_1x_0+n_2y_0+n_3z_0-c|}{|\vec n|}$.

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. Definieren Sie das Kreuzprodukt und erklären Sie Richtung und Betrag geometrisch.
> 2. Nennen Sie die drei Darstellungsformen einer Ebene und den Weg von der Parameter- zur Normalvektorform.
> 3. **Definieren Sie „windschief".** Warum gibt es das nur im Raum?
> 4. Wie bestimmt man den Schnittpunkt einer Geraden mit einer Ebene? Wann existiert keiner?
> 5. Wie misst man den Abstand eines Punktes von einer Ebene?

## Verwandte Themen
[[TP04 Vektoren in R2]] · [[TP03 Gleichungssysteme & Ungleichungen]] · [[Skalarprodukt]] · [[Kreuzprodukt]]
