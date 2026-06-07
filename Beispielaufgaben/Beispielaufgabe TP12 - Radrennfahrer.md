---
typ: beispielaufgabe
themenpool: 12
titel: "Beispiel-Maturaaufgabe — Radrennfahrer (Anwendung der Differentialrechnung)"
gebiet: Analysis
tags: [beispiel, matura, analysis, differentialrechnung, kinematik]
quelle: ["Themenpool-Katalog 2026, S. 3 — offizielle Beispielaufgabe"]
verwandt: ["[[TP12 Funktionsuntersuchungen]]", "[[TP11 Grundlagen Differentialrechnung]]"]
---

# Beispiel-Maturaaufgabe (Themengebiet 12) — Radrennfahrer

> [!quote] Originalangabe
> Ein Radrennfahrer startet bei einem Einzelzeitfahren. Sein zurückgelegter Weg in den ersten neun Sekunden lässt sich annähernd durch $s\colon t\mapsto s(t)$ mit
> $$s(t)=\frac{t^3}{30}+\frac{t^2}{20}\qquad(t\text{ in s},\ s\text{ in m})$$
> modellieren.
> 1. Ermitteln Sie die Geschwindigkeitsfunktion $v$ und die Beschleunigungsfunktion $a$. *(Reproduktion, Transfer)*
> 2. Stellen Sie beide Funktionen im Zeitintervall $0\le t\le9$ graphisch dar. *(Reproduktion)*
> 3. Welche Schlüsse über die Bewegung lassen sich aus dem Verlauf der Graphen ziehen? *(Reflexion)*
> 4. Berechnen Sie die mittlere Geschwindigkeit in den ersten neun Sekunden und die Momentangeschwindigkeit bei $t=5$ s; geben Sie beide in km/h an und erklären Sie die Begriffe. *(Reproduktion, Transfer)*

Quelle: offizieller Themenpool-Katalog 2026. Theorie: [[TP12 Funktionsuntersuchungen]], [[TP11 Grundlagen Differentialrechnung]].

---

## Lösung

### Teil 1 — Geschwindigkeit & Beschleunigung
Geschwindigkeit = Ableitung des Weges, Beschleunigung = Ableitung der Geschwindigkeit ([[Ableitungsregeln|Potenzregel]]):
$$v(t)=s'(t)=\frac{3t^2}{30}+\frac{2t}{20}=\frac{t^2}{10}+\frac{t}{10}=\frac{t^2+t}{10}\ \left[\tfrac{\text{m}}{\text{s}}\right]$$
$$a(t)=v'(t)=\frac{2t}{10}+\frac{1}{10}=\frac{2t+1}{10}\ \left[\tfrac{\text{m}}{\text{s}^2}\right]$$

### Teil 2 — Graphen

![[radrennfahrer.svg|520]]
*Abbildung: $v(t)$ (blau, nach oben geöffnete Parabel) und $a(t)$ (rot, steigende Gerade) auf $[0;9]$. Beide sind durchgehend positiv und steigend.*

| $t$ (s) | 0 | 3 | 5 | 7 | 9 |
|---|---|---|---|---|---|
| $v(t)$ (m/s) | 0 | 1,2 | 3,0 | 5,6 | 9,0 |
| $a(t)$ (m/s²) | 0,1 | 0,7 | 1,1 | 1,5 | 1,9 |

### Teil 3 — Deutung der Bewegung (Reflexion)
- $v(t)>0$ und **streng steigend** auf $[0;9]$ → der Fahrer wird **durchgehend schneller**, bremst nie.
- $v(0)=0$ → er startet **aus dem Stand**.
- $a(t)>0$ und ebenfalls steigend → die **Beschleunigung nimmt selbst zu**: er wird nicht nur schneller, sondern *immer stärker* schneller.
- Zusammenhang: Weil $a(t)=v'(t)>0$ ist, ist $v$ monoton steigend — die Aussagen über $a$ erklären die Form von $v$.

### Teil 4 — Mittlere vs. momentane Geschwindigkeit
**Mittlere Geschwindigkeit** auf $[0;9]$ (Differenzenquotient = Sekantensteigung):
$$\bar v=\frac{s(9)-s(0)}{9-0}=\frac{\frac{729}{30}+\frac{81}{20}}{9}=\frac{24{,}3+4{,}05}{9}=\frac{28{,}35}{9}=3{,}15\ \tfrac{\text{m}}{\text{s}}$$
$$3{,}15\ \tfrac{\text{m}}{\text{s}}\times3{,}6=11{,}34\ \tfrac{\text{km}}{\text{h}}$$

**Momentangeschwindigkeit** bei $t=5$ (Differentialquotient = Tangentensteigung):
$$v(5)=\frac{5^2+5}{10}=\frac{30}{10}=3{,}0\ \tfrac{\text{m}}{\text{s}}=3{,}0\times3{,}6=10{,}8\ \tfrac{\text{km}}{\text{h}}$$

> [!note] Begriffe erklärt
> - **Mittlere Geschwindigkeit** = gesamte Strecke ÷ gesamte Zeit = durchschnittliche Änderungsrate des Weges über das ganze Intervall (Steigung der **Sekante**).
> - **Momentangeschwindigkeit** = Geschwindigkeit in **einem** Augenblick = Grenzwert des Differenzenquotienten = Wert der Ableitung $v(t)$ (Steigung der **Tangente**).
> - Hier ist $\bar v=3{,}15>v(5)=3{,}0$, weil die Geschwindigkeit in der zweiten Hälfte stark zunimmt; der Durchschnitt wird vom schnellen Endstück „nach oben gezogen" (es gilt $\bar v=v(t)$ erst bei $t\approx5{,}13$ s).

---

## Was die Prüfer:innen hören wollen
Diese eine Aufgabe verbindet alle drei Kompetenzbereiche (siehe [[00 Prüfungsformat & Kompetenzbereiche]]): **rechnen** (Ableiten, Werte), **erklären** (Zusammenhang $s\to v\to a$), **reflektieren** (Bewegungsdeutung) und **Einheiten umrechnen** (m/s ↔ km/h, Faktor $3{,}6$).

## Verwandte Themen
[[TP12 Funktionsuntersuchungen]] · [[TP11 Grundlagen Differentialrechnung]] · [[Differentialquotient]] · [[Ableitungsregeln]]
