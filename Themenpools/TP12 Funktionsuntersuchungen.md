---
themenpool: 12
titel: "Differentialrechnung: Funktionsuntersuchungen, Wirtschaft, Naturwissenschaften"
gebiet: Analysis
tags: [themenpool, analysis, kurvendiskussion, extremstellen, wendestellen, wirtschaft]
quelle: ["Themenpool 12", "Notizbuch 7B (2024/25)"]
verwandt: ["[[TP11 Grundlagen Differentialrechnung]]", "[[TP13 Extremwertaufgaben]]", "[[Kurvendiskussion]]"]
---

# TP12 — Differentialrechnung: Funktionsuntersuchungen

> [!info] Leitidee
> Mit erster und zweiter Ableitung liest man das Verhalten eines Graphen ab: $f'$ steuert **Monotonie und Extremstellen**, $f''$ steuert **Krümmung und Wendestellen**. Umgekehrt rekonstruiert man aus geforderten Eigenschaften die Funktionsgleichung (**Steckbriefaufgaben**).
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 12]] · Notizbuch **7B**
>
> Zugehörige offizielle Beispiel-Maturaaufgabe → [[Beispielaufgabe TP12 - Radrennfahrer]].

## 1. Monotonie, Extrem- und Wendestellen

> [!definition] Lokales Extremum, Wendestelle, Sattelpunkt #definition
> - $x_0$ heißt **lokale Extremstelle**, wenn $f(x_0)$ in einer Umgebung der größte (Hochpunkt) bzw. kleinste (Tiefpunkt) Wert ist.
> - $x_0$ heißt **Wendestelle**, wenn die **Krümmung** dort das Vorzeichen wechselt (von konvex zu konkav oder umgekehrt).
> - Ein **Sattelpunkt** ist ein Wendepunkt mit waagrechter Tangente ($f'=0$ und $f''=0$).

> [!satz] Erste Ableitung — Monotonie & Extremstellen #satz #formel
> - $f'(x)>0$ auf einem Intervall ⇒ streng **steigend**; $f'(x)<0$ ⇒ **fallend**.
> - **Notwendig** für Extremum: $f'(x_0)=0$.
> - **Hinreichend:** $f'$ wechselt bei $x_0$ das Vorzeichen — $+\to-$ ⇒ **Hochpunkt**, $-\to+$ ⇒ **Tiefpunkt**. Alternativ: $f'(x_0)=0$ und $f''(x_0)<0$ ⇒ Hochpunkt, $f''(x_0)>0$ ⇒ Tiefpunkt.

> [!satz] Zweite Ableitung — Krümmung & Wendestellen #satz #formel
> - $f''(x)>0$ ⇒ **linksgekrümmt (konvex)**; $f''(x)<0$ ⇒ **rechtsgekrümmt (konkav)**.
> - **Wendestelle:** notwendig $f''(x_0)=0$, hinreichend zusätzlich Vorzeichenwechsel von $f''$ (bzw. $f'''(x_0)\neq0$).

![[kurvendiskussion.svg|480]]
*Abbildung: $f(x)=x^3-3x$ mit Hochpunkt $(-1\mid2)$, Tiefpunkt $(1\mid-2)$ und Wendepunkt $(0\mid0)$.*

> [!merke] Schema der Kurvendiskussion #merke
> 1. Definitionsmenge, Symmetrie, Verhalten im Unendlichen / Asymptoten
> 2. Nullstellen ($f(x)=0$)
> 3. Extremstellen ($f'(x)=0$, Art über Vorzeichen/$f''$)
> 4. Wendestellen ($f''(x)=0$, Vorzeichenwechsel)
> 5. Skizze
>
> Komplett-Beispiel: [[Kurvendiskussion]]. Regeln: [[Ableitungsregeln]].

## 2. Funktionsgleichung aus Eigenschaften (Steckbrief)

> [!merke] Vorgehen #merke
> Jede Eigenschaft liefert eine Gleichung für die Koeffizienten:
> | Bedingung | Gleichung |
> |---|---|
> | Punkt $(x_0\mid y_0)$ auf $f$ | $f(x_0)=y_0$ |
> | waagrechte Tangente / Extremum in $x_0$ | $f'(x_0)=0$ |
> | Wendepunkt in $x_0$ | $f''(x_0)=0$ |
> | Steigung $m$ in $x_0$ | $f'(x_0)=m$ |
> Anzahl Bedingungen = Anzahl Koeffizienten → [[TP03 Gleichungssysteme & Ungleichungen|LGS]] lösen.

## 3. Anwendung: Kosten-Preis-Theorie

> [!definition] Wirtschaftliche Funktionen #definition #formel
> | Funktion | Bedeutung | Ableitung |
> |---|---|---|
> | $K(x)$ Kosten | Gesamtkosten bei Menge $x$ | $K'(x)$ **Grenzkosten** |
> | $E(x)=p\cdot x$ Erlös | Umsatz | $E'(x)$ Grenzerlös |
> | $G(x)=E(x)-K(x)$ Gewinn | | $G'(x)=0$ → **Gewinnmaximum** |
> - **Break-even-Punkt:** $E(x)=K(x)$ (Gewinnschwelle).
> - **Stückkosten** $\bar K(x)=\frac{K(x)}{x}$, Minimum im **Betriebsoptimum**.

## 4. Anwendung: Naturwissenschaft
$s(t)\xrightarrow{\ '\ }v(t)\xrightarrow{\ '\ }a(t)$ — Weg → Geschwindigkeit → Beschleunigung. Vollständig: [[Beispielaufgabe TP12 - Radrennfahrer]].

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. **Definieren Sie Extrem-, Wende- und Sattelpunkt** und nennen Sie die zugehörigen Ableitungsbedingungen.
> 2. Welche Aussagen liefert die zweite Ableitung über den Graphen?
> 3. Beschreiben Sie das Schema einer Kurvendiskussion an $f(x)=x^3-3x$.
> 4. Erklären Sie Grenzkosten und Gewinnmaximum mithilfe der Ableitung.
> 5. Bestimmen Sie aus gegebenen Eigenschaften die Gleichung einer Polynomfunktion (Steckbrief).

## Verwandte Themen
[[TP11 Grundlagen Differentialrechnung]] · [[TP13 Extremwertaufgaben]] · [[TP08 Funktionen & Polynomfunktionen]] · [[Kurvendiskussion]] · [[Ableitungsregeln]] · [[Beispielaufgabe TP12 - Radrennfahrer]]
