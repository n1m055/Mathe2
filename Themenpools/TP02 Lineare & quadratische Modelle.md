---
themenpool: 2
titel: "Lineare und quadratische Modelle"
gebiet: Algebra
tags: [themenpool, algebra, funktionen, lineare-funktion, quadratische-funktion]
quelle: ["Themenpool 2", "Notizbuch 5B (2022/23)"]
verwandt: ["[[TP01 Zahlenbereiche & Mengen]]", "[[TP08 Funktionen & Polynomfunktionen]]", "[[TP12 Funktionsuntersuchungen]]"]
---

# TP02 — Lineare und quadratische Modelle

> [!info] Leitidee
> Lineare und quadratische Funktionen sind die einfachsten Modelle realer Zusammenhänge: konstante Änderung (linear) bzw. konstante Krümmung (quadratisch). Aus den Parametern lassen sich alle Eigenschaften ablesen — und umgekehrt.
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 2]] · Notizbuch **5B**

![[lineare-quadratische.svg|520]]
*Abbildung: Eine Gerade $f(x)=0{,}5x+1$ (blau) und eine Parabel $g(x)=(x-2)^2-1$ (rot) mit Scheitel $S(2\mid-1)$ und $y$-Achsenabschnitt $d=1$.*

## 1. Lineare Modelle

> [!definition] Lineare Funktion #definition #formel
> Eine Funktion $f:\mathbb{R}\to\mathbb{R}$ heißt **linear (affin)**, wenn sie sich schreiben lässt als
> $$f(x)=k\cdot x+d,\qquad k,d\in\mathbb{R}.$$
> Ihr Graph ist eine **Gerade**. Dabei ist $k$ die **Steigung** und $d=f(0)$ der **$y$-Achsenabschnitt**.

> [!formel] Steigung als Änderungsrate #formel
> $$k=\frac{\Delta y}{\Delta x}=\frac{f(x_2)-f(x_1)}{x_2-x_1}$$
> $k>0$ steigend, $k<0$ fallend, $k=0$ konstant. Die Steigung ist bei einer linearen Funktion **überall gleich** — das ist ihr Kennzeichen.

**Charakteristikum (Transfer):** Eine Größe wächst *linear*, wenn sie in gleichen Schritten um den **gleichen Betrag** (konstante Differenz) zunimmt — im Gegensatz zum konstanten *Faktor* beim exponentiellen Wachstum, [[TP09 Exponential- & Logarithmusfunktion]].

> [!beispiel] Lineares Modell #beispiel
> Taxi: 4 € Grundgebühr + 1,80 €/km. $K(x)=1{,}8x+4$. Steigung $k=1{,}8$ €/km = Preis pro Kilometer, $d=4$ € = Grundgebühr. Bei $x=10$: $K=22$ €.

## 2. Quadratische Modelle

> [!definition] Quadratische Funktion und Parabel #definition #formel
> Eine Funktion der Form
> $$f(x)=ax^2+bx+c,\qquad a\neq0$$
> heißt **quadratisch**; ihr Graph ist eine **Parabel**. **Allgemeine Form** $ax^2+bx+c$, **Scheitelform** $f(x)=a(x-x_S)^2+y_S$ mit Scheitel $S(x_S\mid y_S)$.
> $a>0$: nach oben offen (Minimum), $a<0$: nach unten offen (Maximum); $|a|$ steuert die Breite.

> [!satz] Scheitelkoordinaten #satz #formel
> $$x_S=-\frac{b}{2a},\qquad y_S=f(x_S)$$

> [!beispiel] Herleitung der Scheitelform (quadratische Ergänzung) #herleitung
> $f(x)=ax^2+bx+c=a\left(x^2+\frac{b}{a}x\right)+c=a\left(x+\frac{b}{2a}\right)^2-\frac{b^2}{4a}+c.$
> Ablesbar: $x_S=-\frac{b}{2a}$, $y_S=c-\frac{b^2}{4a}$. Dieselbe Idee liefert die [[Mitternachtsformel]]. $\blacksquare$

> [!satz] Nullstellen und Diskriminante #satz #formel
> $ax^2+bx+c=0 \Rightarrow x_{1,2}=\dfrac{-b\pm\sqrt{D}}{2a}$ mit **Diskriminante** $D=b^2-4ac$.
>
> | $D$ | reelle Lösungen | Parabel & $x$-Achse |
> |---|---|---|
> | $D>0$ | zwei verschiedene | schneidet |
> | $D=0$ | eine (doppelte) | berührt (Scheitel auf der Achse) |
> | $D<0$ | keine (zwei komplexe) | kein Schnitt |
>
> Vollständige Herleitung: [[Mitternachtsformel]].

> [!satz] Satz von Vieta #satz #formel
> Für $x^2+px+q=0$: $\;x_1+x_2=-p,\ x_1\cdot x_2=q$. Nützlich zum Kontrollieren und Faktorisieren. → [[Satz von Vieta]]

> [!beispiel] Wurfparabel (Kontext) #beispiel
> $h(t)=-5t^2+20t+1{,}5$ ($h$ in m, $t$ in s).
> Maximale Höhe: $t_S=-\frac{20}{-10}=2$ s, $h(2)=21{,}5$ m. Aufprall ($h=0$): $t\approx4{,}07$ s. Deutung: $c=1{,}5$ m Abwurfhöhe, Scheitel = Steighöhe.

## 3. Grundbegriffe reeller Funktionen

> [!definition] Definitions- und Wertemenge, Darstellungsformen #definition
> **Definitionsmenge $D$** = erlaubte $x$-Werte, **Wertemenge $W$** = angenommene $y$-Werte. Vier gleichwertige **Darstellungsformen**: Term (Formel), Tabelle, Graph, verbale Beschreibung.
> Linear: $D=W=\mathbb{R}$ (für $k\neq0$); quadratisch: $D=\mathbb{R}$, $W=[y_S;\infty)$ bzw. $(-\infty;y_S]$.

Vertiefung aller Funktionseigenschaften: [[Funktionseigenschaften]] und [[TP08 Funktionen & Polynomfunktionen]].

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. Definieren Sie „lineare Funktion" und „quadratische Funktion" präzise. Was bedeuten die Parameter jeweils?
> 2. Leiten Sie die Scheitelform und damit $x_S=-\frac{b}{2a}$ durch quadratische Ergänzung her.
> 3. Welche Rolle spielt die Diskriminante? Skizzieren Sie die drei Fälle.
> 4. Erklären Sie den Satz von Vieta und kontrollieren Sie damit eine Lösung.
> 5. Eine Parabel hat Nullstellen bei $x=1,\,5$ und geht durch $(0\mid5)$ — bestimmen Sie die Funktionsgleichung. *(Transfer: Eigenschaften → Term)*

## Verwandte Themen
[[TP01 Zahlenbereiche & Mengen]] · [[TP08 Funktionen & Polynomfunktionen]] · [[TP12 Funktionsuntersuchungen]] · [[Mitternachtsformel]] · [[Satz von Vieta]] · [[Funktionseigenschaften]]
