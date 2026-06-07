---
themenpool: 6
titel: "Trigonometrie"
gebiet: Geometrie
tags: [themenpool, geometrie, trigonometrie, dreieck]
quelle: ["Themenpool 6", "Notizbuch 5B (2022/23)", "Notizbuch 8B (2025/26) – Wiederholung"]
verwandt: ["[[TP10 Winkelfunktionen]]", "[[TP04 Vektoren in R2]]"]
---

# TP06 — Trigonometrie

> [!info] Leitidee
> Trigonometrie verknüpft **Seiten und Winkel** in Dreiecken. Im rechtwinkligen Dreieck genügen $\sin,\cos,\tan$; im beliebigen Dreieck übernehmen **Sinus-** und **Cosinussatz**. Anwendung: Höhen und Entfernungen bestimmen, ohne sie direkt zu messen (Vermessung).
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 6]] · Notizbuch **5B** (Grundlagen), **8B** (Wiederholung)

## 1. Rechtwinkliges Dreieck

> [!definition] Sinus, Cosinus, Tangens #definition #formel
> Bezogen auf einen spitzen Winkel $\alpha$ im rechtwinkligen Dreieck (Hypotenuse = längste Seite gegenüber dem rechten Winkel):
> $$\sin\alpha=\frac{\text{Gegenkathete}}{\text{Hypotenuse}},\qquad \cos\alpha=\frac{\text{Ankathete}}{\text{Hypotenuse}},\qquad \tan\alpha=\frac{\text{Gegenkathete}}{\text{Ankathete}}=\frac{\sin\alpha}{\cos\alpha}.$$
> Diese Verhältnisse hängen **nur vom Winkel** ab (ähnliche Dreiecke), nicht von der Größe.

![[rechtwinkliges-dreieck.svg|470]]
*Abbildung: Im rechtwinkligen Dreieck bezeichnet man die Seiten relativ zum Winkel $\alpha$ als Gegenkathete, Ankathete und Hypotenuse.*

> [!formel] Grundbeziehungen #formel #merke
> Satz des Pythagoras $a^2+b^2=c^2$ und der trigonometrische Pythagoras $\sin^2\alpha+\cos^2\alpha=1$.

> [!beispiel] Höhe bestimmen #beispiel
> Turmspitze unter $32^\circ$ aus 50 m Abstand: $\tan32^\circ=\frac{h}{50}\Rightarrow h=50\tan32^\circ\approx31{,}2$ m.

## 2. Beliebiges Dreieck

![[dreieck-allgemein.svg|460]]
*Abbildung: Standardbezeichnungen — Seite $a$ liegt dem Winkel $\alpha$ gegenüber usw.*

> [!satz] Sinussatz #satz #formel
> Im beliebigen Dreieck mit Seiten $a,b,c$ gegenüber $\alpha,\beta,\gamma$:
> $$\frac{a}{\sin\alpha}=\frac{b}{\sin\beta}=\frac{c}{\sin\gamma}=2R\qquad(R=\text{Umkreisradius}).$$
> Anwendbar bei **WSW/SWW** oder **SSW**. → [[Sinussatz]]
> ⚠️ **SSW ist mehrdeutig**, da $\sin\alpha=\sin(180^\circ-\alpha)$ — beide Lösungen prüfen. #merke

> [!satz] Cosinussatz #satz #formel
> $$c^2=a^2+b^2-2ab\cos\gamma$$
> Verallgemeinerung des Pythagoras (für $\gamma=90^\circ$ ist $\cos\gamma=0$). Anwendbar bei **SWS** oder **SSS**. → [[Cosinussatz]]

> [!merke] Welcher Satz wann? #merke
> | Gegeben | Satz |
> |---|---|
> | SWS (2 Seiten + Zwischenwinkel) | Cosinussatz |
> | SSS (3 Seiten) | Cosinussatz (nach Winkel umstellen) |
> | WSW / SWW | Sinussatz |
> | SSW | Sinussatz (Mehrdeutigkeit prüfen) |

> [!satz] Flächeninhalt #satz #formel
> $$A=\tfrac12\,a\,b\,\sin\gamma$$

> [!beispiel] Herleitung der Flächenformel #herleitung
> Höhe auf $b$: $h_b=a\sin\gamma$. Mit $A=\tfrac12\,b\,h_b$ folgt $A=\tfrac12 ab\sin\gamma$. $\blacksquare$

> [!beispiel] Vermessungsaufgabe #beispiel
> $A,B$ im Abstand $c=200$ m, Winkel zum Zielpunkt $C$: $\alpha=65^\circ,\ \beta=78^\circ$. Dann $\gamma=37^\circ$ und $b=\frac{c\sin\beta}{\sin\gamma}=\frac{200\sin78^\circ}{\sin37^\circ}\approx325$ m.

## 3. Brücke zu den Winkelfunktionen
Erweitert man $\alpha$ über $90^\circ$ hinaus, definiert man $\sin,\cos,\tan$ am **Einheitskreis** → [[Einheitskreis]] und [[TP10 Winkelfunktionen]] (periodische Funktionen, Bogenmaß, Schwingungen).

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. Definieren Sie $\sin,\cos,\tan$ am rechtwinkligen Dreieck. Warum hängen sie nur vom Winkel ab?
> 2. Formulieren Sie Sinus- und Cosinussatz und entscheiden Sie für gegebene Stücke, welcher passt.
> 3. **Warum** ist der SSW-Fall mehrdeutig?
> 4. Leiten Sie die Flächenformel $A=\tfrac12 ab\sin\gamma$ her.
> 5. Lösen Sie eine Vermessungsaufgabe (unzugängliche Strecke über ein Dreieck).

## Verwandte Themen
[[TP10 Winkelfunktionen]] · [[TP04 Vektoren in R2]] · [[Sinussatz]] · [[Cosinussatz]] · [[Einheitskreis]]
