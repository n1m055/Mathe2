---
typ: konzept
titel: "Polynomdivision"
tags: [konzept, verfahren, algebra, herleitung]
verwandt: ["[[Fundamentalsatz der Algebra]]", "[[TP08 Funktionen & Polynomfunktionen]]"]
---

# Polynomdivision

> [!definition] Zweck #definition #merke
> Spaltet aus einem Polynom einen bekannten **Linearfaktor** $(x-x_1)$ ab (nachdem man eine Nullstelle $x_1$ geraten hat) und reduziert so den Grad. Funktioniert wie schriftliches Dividieren.

> [!example] Beispiel — $(x^3-2x^2-5x+6):(x-1)$ #beispiel #herleitung
> $$
> \begin{aligned}
> &x^3-2x^2-5x+6 \;:\;(x-1)= x^2-x-6\\
> &\underline{-(x^3-\;x^2)}\\
> &\qquad\;\; -x^2-5x\\
> &\qquad\underline{-(-x^2+x)}\\
> &\qquad\qquad\;-6x+6\\
> &\qquad\qquad\underline{-(-6x+6)}\\
> &\qquad\qquad\qquad\quad 0
> \end{aligned}
> $$
> Ergebnis $x^2-x-6$, Rest $0$ (bestätigt: $x=1$ war Nullstelle). Restpolynom weiter mit [[Mitternachtsformel]]: $x=3,\ x=-2$.

> [!tip] Horner-Schema #merke
> Schnellere Alternative zur Division durch $(x-x_1)$: Koeffizienten tabellarisch „durchschleifen". Liefert Quotient **und** Funktionswert $p(x_1)$.

Verwendet in: [[TP01 Zahlenbereiche & Mengen]] · [[TP08 Funktionen & Polynomfunktionen]] · [[Fundamentalsatz der Algebra]].
