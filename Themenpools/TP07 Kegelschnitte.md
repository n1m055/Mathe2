---
themenpool: 7
titel: "Kurven und nichtlineare analytische Geometrie (Kegelschnitte)"
gebiet: Geometrie
tags: [themenpool, geometrie, kegelschnitte, kreis, ellipse, hyperbel, parabel]
quelle: ["Themenpool 7", "Notizbuch 6B (2023/24)", "Notizbuch 7B (2024/25)"]
verwandt: ["[[TP02 Lineare & quadratische Modelle]]", "[[TP04 Vektoren in R2]]"]
---

# TP07 — Kegelschnitte & nichtlineare analytische Geometrie

> [!info] Leitidee
> **Kegelschnitte** entstehen als Schnitt eines Doppelkegels mit einer Ebene: Kreis, Ellipse, Parabel, Hyperbel. Jeder lässt sich als **Ortslinie** (Punktmenge mit einer Abstandseigenschaft) definieren und durch eine Gleichung 2. Grades beschreiben. Der Schnitt mit Geraden führt auf eine quadratische Gleichung, deren [[Mitternachtsformel|Diskriminante]] über Sekante/Tangente/Passante entscheidet.
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 7]] · Notizbuch **6B/7B**

## 1. Definitionen als Ortslinien

> [!definition] Kreis #definition #formel
> **Ortslinie** aller Punkte mit konstantem Abstand $r$ (Radius) vom Mittelpunkt $M(m\mid n)$:
> $$(x-m)^2+(y-n)^2=r^2\quad\big(\text{Mittelpunkt im Ursprung: } x^2+y^2=r^2\big).$$

> [!definition] Ellipse #definition #formel
> Ortslinie aller Punkte, für die die **Summe der Abstände** zu zwei festen Punkten (Brennpunkten $F_1,F_2$) konstant $=2a$ ist:
> $$\frac{x^2}{a^2}+\frac{y^2}{b^2}=1\quad(a>b>0).$$
> Halbachsen $a$ (groß), $b$ (klein); lineare Exzentrizität $e$ mit $a^2=b^2+e^2$; Brennpunkte $(\pm e\mid0)$.

![[ellipse.svg|480]]
*Abbildung: Ellipse mit Halbachsen $a,b$ und Brennpunkten $F_1,F_2$. Für jeden Punkt der Ellipse ist $|PF_1|+|PF_2|=2a$.*

> [!definition] Hyperbel #definition #formel
> Ortslinie aller Punkte, für die der **Betrag der Differenz** der Abstände zu zwei Brennpunkten konstant $=2a$ ist:
> $$\frac{x^2}{a^2}-\frac{y^2}{b^2}=1.$$
> **Asymptoten** $y=\pm\frac{b}{a}x$; Exzentrizität $e^2=a^2+b^2$.

![[hyperbel.svg|480]]
*Abbildung: Hyperbel mit zwei Ästen; die gestrichelten Asymptoten $y=\pm\frac{b}{a}x$ geben das Fernverhalten an.*

> [!definition] Parabel #definition #formel
> Ortslinie aller Punkte mit **gleichem Abstand** zu einem Brennpunkt $F$ und einer Leitlinie $\ell$:
> $$y^2=2px\quad(\text{Öffnung in }x)\qquad\text{bzw.}\qquad y=ax^2+bx+c.$$
> Bezug zu den [[TP02 Lineare & quadratische Modelle|quadratischen Funktionen]].

![[parabel-leitlinie.svg|420]]
*Abbildung: Für jeden Parabelpunkt $P$ ist der Abstand zum Brennpunkt $F$ gleich dem Abstand zur Leitlinie.*

## 2. Lagebeziehung Kegelschnitt – Gerade

> [!definition] Sekante, Tangente, Passante #definition #satz #merke
> Setzt man die Geradengleichung in die Kegelschnittgleichung ein, entsteht eine quadratische Gleichung. Die **Diskriminante $D$** bestimmt die Lage:
>
> | $D$ | Schnittpunkte | Lage |
> |---|---|---|
> | $D>0$ | zwei | **Sekante** |
> | $D=0$ | einer (Berührpunkt) | **Tangente** |
> | $D<0$ | keiner | **Passante** |
>
> → Diskriminante: [[Mitternachtsformel]].

> [!formel] Tangenten — Berührbedingung & Spaltform #formel
> - **Berührbedingung:** $D=0$ liefert eine Bedingung an die Geradenparameter ($k,d$).
> - **Kreis-Tangente:** Abstand $M$–Gerade $=r$.
> - **Spaltformel** (Tangente im Kurvenpunkt $P(x_0\mid y_0)$): jeweils ein Faktor wird „aufgespalten":
>   - Kreis: $x\,x_0+y\,y_0=r^2$
>   - Ellipse: $\dfrac{x x_0}{a^2}+\dfrac{y y_0}{b^2}=1$
>   - Hyperbel: $\dfrac{x x_0}{a^2}-\dfrac{y y_0}{b^2}=1$

> [!beispiel] Tangente an Kreis #beispiel
> Kreis $x^2+y^2=25$, $P(3\mid4)$ (liegt darauf: $9+16=25$). Spaltform: $3x+4y=25$. Probe: durch $P$ ✓ und senkrecht zum Radius $\overrightarrow{MP}=(3,4)$.

> [!beispiel] Schnitt Gerade/Ellipse #beispiel
> Ellipse $\frac{x^2}{16}+\frac{y^2}{4}=1$, Gerade $y=x+c$. Einsetzen, auf Normalform bringen, $D=0$ setzen → liefert die $c$-Werte der **Tangenten**.

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. Definieren Sie die vier Kegelschnitte **als Ortslinien** und geben Sie ihre Gleichungen in Mittelpunktslage an.
> 2. Wie unterscheiden sich Ellipse und Hyperbel in Definition, Gleichung und Brennpunktlage? Was sind die Asymptoten der Hyperbel?
> 3. Wie bestimmt man die Lagebeziehung Gerade–Kegelschnitt mit der Diskriminante?
> 4. Was besagt die Berührbedingung? Bestimmen Sie die Tangente an $x^2+y^2=25$ in $P(3\mid4)$.
> 5. Welcher Zusammenhang besteht zwischen Parabel als Kegelschnitt und quadratischer Funktion?

## Verwandte Themen
[[TP02 Lineare & quadratische Modelle]] · [[TP04 Vektoren in R2]] · [[Mitternachtsformel]]
