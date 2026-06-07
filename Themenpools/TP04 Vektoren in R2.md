---
themenpool: 4
titel: "Vektoren im ℝ²: Analytische Geometrie der Ebene"
gebiet: Geometrie
tags: [themenpool, geometrie, vektoren, analytische-geometrie]
quelle: ["Themenpool 4", "Notizbuch 5B (2022/23)", "Notizbuch 6B (2023/24)"]
verwandt: ["[[TP05 Vektoren in R3]]", "[[TP03 Gleichungssysteme & Ungleichungen]]", "[[TP06 Trigonometrie]]"]
---

# TP04 — Vektoren im ℝ²: Analytische Geometrie der Ebene

> [!info] Leitidee
> Ein Vektor beschreibt eine **Verschiebung** (Richtung und Länge), unabhängig vom Ort. Mit Vektoren übersetzt man geometrische Fragen (Geraden, Schnitte, Winkel, Flächen) in Rechnung. Das [[Skalarprodukt]] misst Winkel, der Normalvektor steht senkrecht.
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 4]] · Notizbuch **5B/6B**

## 1. Was ist ein Vektor?

> [!definition] Vektor (geometrisch) #definition
> Ein **Vektor** ist die Menge aller **gleich langen, gleich gerichteten und parallelen Pfeile** (gerichteten Strecken). Alle diese Pfeile sind nur verschiedene Repräsentanten **desselben** Vektors — ein Vektor ist also durch **Länge und Richtung** eindeutig festgelegt, **nicht** durch seinen Anfangspunkt.
> Der Pfeil vom Punkt $A$ zum Punkt $B$ heißt $\overrightarrow{AB}$.

> [!definition] Vektor (analytisch, in Koordinaten) #definition #formel
> In einem Koordinatensystem wird ein Vektor durch seine **Komponenten** (Koordinaten) dargestellt:
> $$\vec a=\begin{pmatrix}a_1\\a_2\end{pmatrix}.$$
> Die Komponenten geben an, um wie viel man in $x$- bzw. $y$-Richtung verschiebt. Für zwei Punkte $A(a_1\mid a_2)$, $B(b_1\mid b_2)$ gilt **„Spitze minus Schaft"**:
> $$\overrightarrow{AB}=\begin{pmatrix}b_1-a_1\\ b_2-a_2\end{pmatrix}.$$

![[vektor-definition.svg|500]]
*Abbildung: Der Vektor $\vec a=\overrightarrow{AB}=\binom{3}{2}$. Die hellblauen Pfeile sind parallel, gleich lang und gleich orientiert — sie stellen denselben Vektor dar.*

> [!definition] Ortsvektor vs. freier Vektor #definition #merke
> Der **Ortsvektor** eines Punktes $P$ ist der besondere Vektor $\overrightarrow{OP}$ vom Ursprung $O$ zu $P$; seine Komponenten sind genau die **Koordinaten** von $P$. Ein **freier Vektor** (Verschiebung) ist dagegen ortsunabhängig. So unterscheidet man **Punkt** ($P(2\mid3)$, ein Ort) und **Vektor** ($\binom{2}{3}$, eine Verschiebung), obwohl beide dieselben Zahlen tragen.

## 2. Rechnen mit Vektoren

> [!formel] Grundoperationen #formel
> $$\vec a+\vec b=\begin{pmatrix}a_1+b_1\\a_2+b_2\end{pmatrix},\qquad \lambda\vec a=\begin{pmatrix}\lambda a_1\\ \lambda a_2\end{pmatrix},\qquad |\vec a|=\sqrt{a_1^2+a_2^2}$$
> $|\vec a|$ = **Betrag/Länge** (Satz des Pythagoras über die Komponenten). **Nullvektor** $\vec 0=\binom00$. **Einheitsvektor** (Länge 1): $\vec a^0=\frac{1}{|\vec a|}\vec a$.

![[vektor-addition.svg|480]]
*Abbildung: Vektoraddition als Aneinanderhängen ($\vec a$ dann $\vec b$) bzw. als Diagonale des aufgespannten Parallelogramms (Kräfteparallelogramm).*

> [!merke] Geometrische Bedeutung #merke
> - **Addition** = Pfeile aneinanderhängen (oder Parallelogramm-Diagonale).
> - **Skalare Multiplikation** $\lambda\vec a$ = strecken/stauchen; $\lambda<0$ kehrt die Richtung um.
> - **Mittelpunkt** von $AB$: $\overrightarrow{OM}=\tfrac12(\overrightarrow{OA}+\overrightarrow{OB})$.

## 3. Skalarprodukt, parallele und normale Vektoren

> [!definition] Skalarprodukt #definition #satz #formel
> $$\vec a\cdot\vec b=a_1b_1+a_2b_2=|\vec a|\,|\vec b|\cos\varphi$$
> Das Ergebnis ist eine **Zahl** (Skalar). Daraus der Winkel $\cos\varphi=\dfrac{\vec a\cdot\vec b}{|\vec a||\vec b|}$ und das Kriterium **Orthogonalität:** $\vec a\perp\vec b\iff\vec a\cdot\vec b=0$. Vollständig: [[Skalarprodukt]].

![[skalarprodukt.svg|440]]
*Abbildung: Der von zwei Vektoren eingeschlossene Winkel $\varphi$ folgt aus dem Skalarprodukt.*

> [!formel] Parallel und normal #formel #merke
> - **Parallel:** $\vec a\parallel\vec b \iff \vec b=\lambda\vec a \iff a_1b_2-a_2b_1=0$.
> - **Normalvektor** zu $\vec a=\binom{a_1}{a_2}$: $\;\vec n=\binom{-a_2}{a_1}$ (Komponenten tauschen, **ein** Vorzeichen drehen). Probe: $\vec a\cdot\vec n=0$.

## 4. Geraden in der Ebene

> [!definition] Darstellungsformen einer Geraden #definition #formel
> - **Parameterform:** $g:\ \vec X=\vec P+t\cdot\vec r,\quad t\in\mathbb{R}$ ($\vec P$ Punkt auf $g$, $\vec r$ Richtungsvektor).
> - **Normalvektorform:** $\vec n\cdot(\vec X-\vec P)=0$, ausmultipliziert $n_1x+n_2y=c$.
> - **Hauptform** $y=kx+d$ mit Steigung $k=\frac{r_2}{r_1}$.

> [!satz] Lagebeziehungen zweier Geraden #satz
> | Richtungsvektoren | LGS-Lösung | Lage |
> |---|---|---|
> | parallel, Punkt nicht auf $g$ | keine | echt parallel |
> | parallel, Punkt auf $g$ | unendlich | identisch |
> | nicht parallel | genau eine | Schnittpunkt |
>
> Schnittpunkt: Parameterformen gleichsetzen → [[TP03 Gleichungssysteme & Ungleichungen|LGS]]. **Schnittwinkel** über das [[Skalarprodukt]] der Richtungsvektoren.

> [!beispiel] Schnittwinkel #beispiel
> $\vec r_1=\binom{2}{1}$, $\vec r_2=\binom{1}{-1}$: $\cos\varphi=\dfrac{2-1}{\sqrt5\sqrt2}=\dfrac{1}{\sqrt{10}}\Rightarrow\varphi\approx71{,}6^\circ$.

> [!merke] Geometrische Anwendungen #merke
> - **Abstand Punkt–Gerade** über die Normalvektorform (Lotfußpunkt).
> - **Flächeninhalt** des von $\vec a,\vec b$ aufgespannten Parallelogramms: $A=|a_1b_2-a_2b_1|$ (Determinante; in 3D → [[Kreuzprodukt]]). Dreieck: $\tfrac12|a_1b_2-a_2b_1|$.

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. **Definieren Sie den Begriff Vektor** (geometrisch und in Koordinaten). Worin unterscheidet sich ein Vektor von einem Punkt?
> 2. Erklären Sie Orts- und Verbindungsvektor sowie die Regel „Spitze minus Schaft".
> 3. Wie berechnet man den Winkel zwischen zwei Vektoren? Wann sind sie orthogonal, wann parallel?
> 4. Geben Sie zu $\vec a=\binom{3}{4}$ einen Normalvektor und den Einheitsvektor an.
> 5. Nennen Sie die Darstellungsformen einer Geraden und die drei Lagebeziehungen.

## Verwandte Themen
[[TP05 Vektoren in R3]] · [[TP03 Gleichungssysteme & Ungleichungen]] · [[TP06 Trigonometrie]] · [[Skalarprodukt]] · [[Kreuzprodukt]]
