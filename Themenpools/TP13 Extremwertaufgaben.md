---
themenpool: 13
titel: "Differentialrechnung: Extremwertaufgaben"
gebiet: Analysis
tags: [themenpool, analysis, extremwertaufgabe, optimierung]
quelle: ["Themenpool 13", "Notizbuch 7B (2024/25)"]
verwandt: ["[[TP12 Funktionsuntersuchungen]]", "[[Kurvendiskussion]]"]
---

# TP13 — Extremwertaufgaben (Optimierung)

> [!info] Leitidee
> Bei **Extremwertaufgaben** soll eine Größe maximal oder minimal werden (größte Fläche, kürzester Weg, geringste Kosten). Das Problem hat zunächst zwei Variablen; eine **Nebenbedingung** reduziert es auf eine Variable, dann optimiert man mit der Ableitung.
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 13]] · Notizbuch **7B**

## 1. Begriffe und Schema

> [!definition] Zielfunktion, Haupt- und Nebenbedingung #definition
> - Die **Hauptbedingung (Zielfunktion)** beschreibt die zu optimierende Größe (z. B. Fläche $A=x\cdot y$).
> - Die **Nebenbedingung** ist eine zusätzliche Gleichung zwischen den Variablen (z. B. fester Umfang), mit der man eine Variable ersetzt.

> [!merke] Lösungsschema #merke #satz
> 1. **Zielfunktion** aufstellen (was soll extremal werden?).
> 2. **Nebenbedingung** notieren.
> 3. **Einsetzen** → Zielgröße als Funktion **einer** Variablen $f(x)$, mit sinnvoller Definitionsmenge.
> 4. **Ableiten und $f'(x)=0$** lösen (Kandidaten).
> 5. **Art prüfen** ($f''$ oder Vorzeichenwechsel) **und Randstellen** vergleichen.
> 6. **Antwort im Kontext** + geforderte Größen.

> [!warning] Randstellen nicht vergessen #merke
> Das globale Maximum/Minimum kann am **Rand** der Definitionsmenge liegen, wo $f'\neq0$ ist. Immer die Randwerte mit den inneren Kandidaten vergleichen.

![[extremwert-rechteck.svg|500]]
*Abbildung: Für ein Rechteck mit Umfang 20 ist die Fläche $A(x)=x(10-x)$ — eine Parabel mit Maximum bei $x=5$ (das Quadrat mit $A=25$).*

## 2. Durchgerechnete Beispiele

> [!beispiel] Größte Rechteckfläche bei festem Umfang #beispiel #herleitung
> Umfang $U=20$, größte Fläche gesucht.
> 1. Hauptbedingung $A=x\cdot y$. 2. Nebenbedingung $2x+2y=20\Rightarrow y=10-x$.
> 3. $A(x)=x(10-x)=10x-x^2$, $D=(0;10)$. 4. $A'(x)=10-2x=0\Rightarrow x=5$.
> 5. $A''(x)=-2<0$ ⇒ Maximum; Ränder $x\to0,10$ geben $A\to0$.
> 6. $x=5,\ y=5$ → **Quadrat**, $A=25$. (Allgemein: bei festem Umfang ist das Quadrat optimal.)

> [!beispiel] Dose mit minimalem Materialverbrauch #beispiel
> Zylinder mit $V=1000\,\text{cm}^3$, minimiere $O=2\pi r^2+2\pi r h$. Nebenbedingung $V=\pi r^2 h\Rightarrow h=\frac{1000}{\pi r^2}$.
> $O(r)=2\pi r^2+\frac{2000}{r}$, $O'(r)=4\pi r-\frac{2000}{r^2}=0\Rightarrow r=\sqrt[3]{\frac{500}{\pi}}\approx5{,}42$ cm, $h\approx10{,}84$ cm ($h=2r$).

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. **Definieren Sie Haupt- und Nebenbedingung** an einem selbst gewählten Beispiel.
> 2. Warum muss man bei Extremwertaufgaben die Randstellen überprüfen?
> 3. Lösen Sie: größte Rechteckfläche bei Umfang 20, und begründen Sie, warum das Quadrat optimal ist.
> 4. Wie weist man nach, dass ein Kandidat ein Maximum ist?
> 5. Beschreiben Sie den Lösungsweg einer geometrischen Optimierung (z. B. offene Schachtel).

## Verwandte Themen
[[TP12 Funktionsuntersuchungen]] · [[TP11 Grundlagen Differentialrechnung]] · [[Kurvendiskussion]]
