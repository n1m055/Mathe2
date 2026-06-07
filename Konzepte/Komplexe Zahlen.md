---
typ: konzept
titel: "Komplexe Zahlen"
tags: [konzept, definition, algebra, komplexe-zahlen]
verwandt: ["[[Fundamentalsatz der Algebra]]", "[[TP01 Zahlenbereiche & Mengen]]"]
---

# Komplexe Zahlen

> [!definition] Definition #definition #formel
> Imaginäre Einheit $i$ mit $i^2=-1$. $\;z=a+bi$ mit $\operatorname{Re}(z)=a,\ \operatorname{Im}(z)=b$.
> - **Konjugiert:** $\bar z=a-bi$
> - **Betrag:** $|z|=\sqrt{a^2+b^2}$
> - $z\bar z=a^2+b^2=|z|^2$

> [!note] Rechenregeln #formel
> - Addition: komponentenweise $(a+bi)+(c+di)=(a+c)+(b+d)i$.
> - Multiplikation: ausmultiplizieren, $i^2=-1$ einsetzen.
> - Division: mit konjugiertem Nenner erweitern: $\dfrac{z}{w}=\dfrac{z\bar w}{|w|^2}$.

> [!note] Gauß'sche Zahlenebene & Polarform #definition
> $z$ als Punkt/Vektor $(a\mid b)$. **Polarform:** $z=r(\cos\varphi+i\sin\varphi)$ mit $r=|z|$, $\varphi=\arg z$.
> Potenzen der $i$: $i^1=i,\ i^2=-1,\ i^3=-i,\ i^4=1$ (Periode 4). #merke

> [!tip] Wozu komplexe Zahlen? #merke
> In $\mathbb{C}$ ist **jede** Polynomgleichung lösbar (z. B. $x^2+1=0\Rightarrow x=\pm i$) → [[Fundamentalsatz der Algebra]].

> [!example] Beispiel #beispiel
> $(2+3i)(1-5i)=2-10i+3i-15i^2=2-7i+15=17-7i$. $\;|3+4i|=\sqrt{9+16}=5$.

Verwendet in: [[TP01 Zahlenbereiche & Mengen]] · [[Fundamentalsatz der Algebra]].
