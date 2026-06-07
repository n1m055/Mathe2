---
themenpool: 15
titel: "Anwendungen der Integralrechnung: Flächen, Volumina, Wirtschaft und Naturwissenschaften"
gebiet: Analysis
tags: [themenpool, analysis, integral, flaeche, volumen, rotationskoerper]
quelle: ["Themenpool 15", "Notizbuch 7B (2024/25)", "Notizbuch 8B (2025/26)"]
verwandt: ["[[TP14 Grundlagen Integralrechnung]]", "[[Stammfunktion & Integrationsregeln]]"]
---

# TP15 — Anwendungen der Integralrechnung

> [!info] Leitidee
> Das Integral berechnet **Flächen, Volumina** und **aufsummierte Größen**. Entscheidend ist, das Sachproblem als „Integral über eine Rate bzw. einen Querschnitt" zu erkennen und auf **Vorzeichen** zu achten.
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 15]] · Notizbuch **7B/8B**

## 1. Flächenberechnung

> [!definition] Fläche zwischen Kurve und Achse / zwischen zwei Kurven #definition #formel
> $$A=\int_a^b |f(x)|\,dx\qquad\text{bzw.}\qquad A=\int_a^b\big(f_{\text{oben}}(x)-f_{\text{unten}}(x)\big)\,dx.$$
> Bei der Fläche zur $x$-Achse mit **Nullstellen** im Intervall: aufteilen und Teilintegrale **betraglich** addieren. Bei zwei Kurven sind die Grenzen die Schnittstellen ($f=g$).

![[flaeche-zwischen-kurven.svg|500]]
*Abbildung: Fläche zwischen $f(x)=x^2$ und $g(x)=x+2$; integriert wird „obere minus untere Funktion" zwischen den Schnittstellen $x=-1$ und $x=2$.*

> [!beispiel] Fläche zwischen Parabel und Gerade #beispiel
> Schnitt $x^2=x+2\Rightarrow x=-1,\,2$.
> $A=\int_{-1}^{2}\big((x+2)-x^2\big)dx=\Big[\tfrac{x^2}{2}+2x-\tfrac{x^3}{3}\Big]_{-1}^{2}=\tfrac{10}{3}-(-\tfrac{7}{6})=\tfrac{27}{6}=4{,}5.$

## 2. Volumen von Rotationskörpern

> [!definition] Rotation um die $x$-Achse #definition #satz #formel
> Rotiert die Fläche unter $f$ um die $x$-Achse, hat der entstehende Körper das Volumen
> $$V=\pi\int_a^b \big(f(x)\big)^2\,dx.$$
> **Idee:** dünne Scheiben, jede ein Zylinder mit Radius $f(x)$, Querschnitt $\pi f(x)^2$, Dicke $dx$.

![[rotationskoerper.svg|520]]
*Abbildung: Rotiert der Halbkreis $f(x)=\sqrt{r^2-x^2}$ um die $x$-Achse, entsteht eine Kugel mit $V=\frac{4}{3}\pi r^3$.*

> [!beispiel] Kugelvolumen herleiten #herleitung #beispiel
> $f(x)=\sqrt{r^2-x^2}$, $-r\le x\le r$:
> $$V=\pi\int_{-r}^{r}(r^2-x^2)\,dx=\pi\Big[r^2x-\tfrac{x^3}{3}\Big]_{-r}^{r}=\pi\Big(2r^3-\tfrac{2r^3}{3}\Big)=\frac{4}{3}\pi r^3.\ \blacksquare$$

## 3. Weitere Anwendungen

> [!merke] Aufsummieren von Raten / Mittelwert #merke #formel
> - **Naturwissenschaft:** Weg $=\int v(t)\,dt$, Arbeit $=\int F(s)\,ds$, Wassermenge $=\int(\text{Zufluss})\,dt$.
> - **Wirtschaft:** Kostenfunktion aus Grenzkosten $K(x)=\int K'(x)\,dx+K_{\text{fix}}$; Konsumenten-/Produzentenrente als Fläche.
> - **Mittelwert** einer Funktion: $\displaystyle \bar f=\frac{1}{b-a}\int_a^b f(x)\,dx$.

> [!beispiel] Vom Zufluss zur Menge #beispiel
> Zufluss $r(t)=4t$ (L/min) über $[0;3]$: Gesamtmenge $=\int_0^3 4t\,dt=[2t^2]_0^3=18$ L.

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. Wie berechnet man die Fläche zwischen zwei Kurven? Wie findet man die Grenzen?
> 2. Warum muss man bei der Fläche zur $x$-Achse auf Nullstellen/Beträge achten?
> 3. **Leiten Sie die Volumenformel des Rotationskörpers** anschaulich her.
> 4. Berechnen Sie das Kugelvolumen durch Rotation eines Halbkreises.
> 5. Wie gewinnt man aus einer Änderungsrate die Gesamtmenge?

## Verwandte Themen
[[TP14 Grundlagen Integralrechnung]] · [[TP11 Grundlagen Differentialrechnung]] · [[Stammfunktion & Integrationsregeln]] · [[Hauptsatz der Differential- und Integralrechnung]]
