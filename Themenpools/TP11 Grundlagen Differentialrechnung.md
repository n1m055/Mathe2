---
themenpool: 11
titel: "Grundlagen Differentialrechnung"
gebiet: Analysis
tags: [themenpool, analysis, differentialrechnung, ableitung, grenzwert]
quelle: ["Themenpool 11", "Notizbuch 7B (2024/25)"]
verwandt: ["[[TP12 Funktionsuntersuchungen]]", "[[Differentialquotient]]", "[[Ableitungsregeln]]"]
---

# TP11 — Grundlagen der Differentialrechnung

> [!info] Leitidee
> Die Ableitung misst die **momentane Änderungsrate**. Sie entsteht aus der mittleren Änderungsrate (**Differenzenquotient**, Sekante), indem man den Abstand der Stellen gegen null gehen lässt → **Differentialquotient** (Tangente). Daraus folgen alle Funktionsuntersuchungen.
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 11]] · Notizbuch **7B**

## 1. Vom Differenzen- zum Differentialquotienten

> [!definition] Mittlere Änderungsrate (Differenzenquotient) #definition #formel
> Die **mittlere Änderungsrate** von $f$ auf dem Intervall $[x_1;x_2]$ ist
> $$\frac{\Delta y}{\Delta x}=\frac{f(x_2)-f(x_1)}{x_2-x_1}.$$
> Sie ist die **Steigung der Sekante** durch $(x_1\mid f(x_1))$ und $(x_2\mid f(x_2))$.

> [!definition] Ableitung (Differentialquotient) #definition #formel
> Die **Ableitung** von $f$ an der Stelle $x_0$ ist der Grenzwert der Differenzenquotienten:
> $$f'(x_0)=\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}{h}=\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0},$$
> sofern dieser Grenzwert existiert. Geometrisch ist $f'(x_0)$ die **Steigung der Tangente** im Punkt $(x_0\mid f(x_0))$. Ausführlich: [[Differentialquotient]].

![[sekante-tangente.svg|520]]
*Abbildung: Die Sekante (rot, mittlere Rate über $[x_0;x_1]$) geht in die Tangente (grün, momentane Rate in $x_0$) über, wenn der zweite Punkt entlang der Kurve auf $x_0$ zuwandert ($h\to0$).*

> [!beispiel] Herleitung aus der Definition #herleitung #beispiel
> $f(x)=x^2$:
> $$f'(x)=\lim_{h\to0}\frac{(x+h)^2-x^2}{h}=\lim_{h\to0}\frac{2xh+h^2}{h}=\lim_{h\to0}(2x+h)=2x.$$
> So entsteht jede Regel; die fertigen Regeln stehen in [[Ableitungsregeln]].

## 2. Deutung der Ableitung

> [!definition] Differenzierbarkeit & Tangente #definition #formel
> $f$ heißt **differenzierbar** in $x_0$, wenn der obige Grenzwert existiert — der Graph hat dort eine eindeutige Tangente (glatt, keine Ecke). Tangentengleichung:
> $$t(x)=f(x_0)+f'(x_0)\,(x-x_0).$$

> [!merke] Drei Sichtweisen auf $f'(x_0)$ #merke
> | Sicht | Bedeutung |
> |---|---|
> | geometrisch | Steigung der Tangente in $x_0$ |
> | analytisch | Grenzwert des Differenzenquotienten |
> | inhaltlich | momentane Änderungsrate der Größe |
>
> | Kontext $f$ | $f'$ bedeutet |
> |---|---|
> | Weg $s(t)$ | Geschwindigkeit $v(t)$ |
> | Geschwindigkeit $v(t)$ | Beschleunigung $a(t)$ |
> | Kosten $K(x)$ | Grenzkosten $K'(x)$ |
> | Bestand $N(t)$ | Wachstumsgeschwindigkeit |

> [!beispiel] Mittlere vs. momentane Rate #beispiel
> $f(t)=t^2$ (Weg in m). Mittlere Geschwindigkeit auf $[1;3]$: $\frac{9-1}{2}=4$ m/s. Momentane bei $t=2$: $f'(2)=4$ m/s. → durchgerechnet: [[Beispielaufgabe TP12 - Radrennfahrer]].

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. **Definieren Sie Differenzen- und Differentialquotient** und erklären Sie den Übergang anhand der Abbildung.
> 2. Geben Sie die Grenzwertdefinition der Ableitung an und leiten Sie $f'(x)$ für $f(x)=x^2$ her.
> 3. Was bedeutet $f'(x_0)$ geometrisch und inhaltlich? Zwei Kontextbeispiele.
> 4. Was heißt **differenzierbar**? Wann ist eine Funktion an einer Stelle nicht differenzierbar?
> 5. Bestimmen Sie die Tangente an $f(x)=x^2$ in $x_0=2$.

## Verwandte Themen
[[TP12 Funktionsuntersuchungen]] · [[TP09 Exponential- & Logarithmusfunktion]] · [[TP10 Winkelfunktionen]] · [[Differentialquotient]] · [[Ableitungsregeln]]
