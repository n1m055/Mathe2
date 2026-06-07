---
themenpool: 10
titel: "Winkelfunktionen"
gebiet: Funktionen
tags: [themenpool, funktionen, winkelfunktionen, sinus, schwingung]
quelle: ["Themenpool 10", "Notizbuch 6B (2023/24)"]
verwandt: ["[[TP06 Trigonometrie]]", "[[Einheitskreis]]", "[[TP11 Grundlagen Differentialrechnung]]"]
---

# TP10 — Winkelfunktionen

> [!info] Leitidee
> Aus den Seitenverhältnissen im Dreieck ([[TP06 Trigonometrie]]) werden am **Einheitskreis** echte **Funktionen** $\sin,\cos,\tan$ für beliebige Winkel. Ihre periodischen Graphen modellieren **Schwingungen** (Töne, Wechselstrom, Gezeiten).
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 10]] · Notizbuch **6B**

## 1. Definition am Einheitskreis

> [!definition] Sinus, Cosinus, Tangens (allgemein) #definition #formel
> Am **Einheitskreis** (Kreis mit Radius 1 um den Ursprung) gehört zum Winkel $\varphi$ (von der positiven $x$-Achse gegen den Uhrzeigersinn) der Punkt $P$. Dann sind
> $$\cos\varphi=x_P,\qquad \sin\varphi=y_P,\qquad \tan\varphi=\frac{\sin\varphi}{\cos\varphi}.$$
> Damit sind $\sin,\cos$ für **alle** $\varphi\in\mathbb{R}$ definiert (nicht nur spitze Winkel). Grundbeziehung $\sin^2\varphi+\cos^2\varphi=1$. → [[Einheitskreis]]

![[einheitskreis.svg|420]]
*Abbildung: Am Einheitskreis ist $\cos\varphi$ die $x$- und $\sin\varphi$ die $y$-Koordinate des Punktes $P$.*

> [!definition] Bogenmaß #definition #formel
> Das **Bogenmaß** eines Winkels ist die Länge des zugehörigen Kreisbogens am Einheitskreis:
> $$180^\circ\ \widehat{=}\ \pi,\qquad \varphi_{\text{rad}}=\frac{\pi}{180^\circ}\cdot\varphi_{\text{grad}},\qquad 360^\circ=2\pi.$$
> In der Analysis **immer** Bogenmaß — sonst gilt $(\sin x)'=\cos x$ nicht. #merke

## 2. Graphen und Eigenschaften

![[sinus-cosinus.svg|560]]
*Abbildung: $\sin x$ (blau) und $\cos x$ (rot) über einer Periode $[0;2\pi]$; $\cos$ ist der um $\frac{\pi}{2}$ nach links verschobene Sinus.*

> [!definition] Eigenschaften von $\sin$ und $\cos$ #definition
> | | $\sin x$ | $\cos x$ |
> |---|---|---|
> | Periode | $2\pi$ | $2\pi$ |
> | Wertemenge | $[-1;1]$ | $[-1;1]$ |
> | Nullstellen | $k\pi$ | $\frac{\pi}{2}+k\pi$ |
> | Symmetrie | ungerade | gerade |
>
> $\tan x$ hat Periode $\pi$ und **Polstellen** bei $\frac{\pi}{2}+k\pi$.

## 3. Harmonische Schwingungen

> [!definition] Allgemeine Sinusschwingung #definition #satz #formel
> $$f(x)=A\cdot\sin\!\big(b\,(x-c)\big)+d.$$
> | Parameter | Wirkung | Name |
> |---|---|---|
> | $A$ | vertikale Streckung | **Amplitude** |
> | $b$ | horizontale Stauchung | Kreisfrequenz, **Periode** $T=\frac{2\pi}{b}$ |
> | $c$ | horizontale Verschiebung | **Phasenverschiebung** |
> | $d$ | vertikale Verschiebung | Mittellage |

> [!beispiel] Schwingung deuten #beispiel
> $f(t)=3\sin\!\big(\frac{\pi}{6}(t-2)\big)+5$: Amplitude 3, Periode $T=\frac{2\pi}{\pi/6}=12$, um 2 nach rechts verschoben, Mittellage 5. Werte schwanken zwischen 2 und 8.

> [!merke] Brücke zur Analysis #merke
> $(\sin x)'=\cos x$, $(\cos x)'=-\sin x$ — die Ableitung „verschiebt" die Schwingung um $\frac{\pi}{2}$. Siehe [[Ableitungsregeln]], [[TP11 Grundlagen Differentialrechnung]].

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. **Definieren Sie $\sin,\cos,\tan$ am Einheitskreis.** Wie entstehen daraus ihre Graphen?
> 2. Erklären Sie das Bogenmaß und warum man es in der Analysis verwendet.
> 3. Nennen Sie Periode, Wertemenge, Nullstellen und Symmetrie von $\sin$ und $\cos$.
> 4. Welche Wirkung haben $A,b,c,d$ in $f(x)=A\sin(b(x-c))+d$?
> 5. Modellieren Sie eine periodische Größe (Tageslänge, Gezeiten) als Sinusfunktion.

## Verwandte Themen
[[TP06 Trigonometrie]] · [[Einheitskreis]] · [[TP11 Grundlagen Differentialrechnung]] · [[Ableitungsregeln]]
