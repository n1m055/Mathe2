---
themenpool: 14
titel: "Grundlagen der Integralrechnung: Stammfunktionen, bestimmtes Integral"
gebiet: Analysis
tags: [themenpool, analysis, integralrechnung, stammfunktion, hauptsatz]
quelle: ["Themenpool 14", "Notizbuch 7B (2024/25)"]
verwandt: ["[[TP15 Anwendungen Integralrechnung]]", "[[Stammfunktion & Integrationsregeln]]", "[[Hauptsatz der Differential- und Integralrechnung]]"]
---

# TP14 — Grundlagen der Integralrechnung

> [!info] Leitidee
> Das **bestimmte Integral** entsteht aus der Idee, eine Fläche durch immer feinere Rechtecke (Unter-/Obersummen) anzunähern. Der **Hauptsatz** verknüpft diese Flächenidee mit der Umkehrung des Ableitens (**Stammfunktion**): Differenzieren und Integrieren sind Gegenoperationen.
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 14]] · Notizbuch **7B**

## 1. Vom Flächenproblem zum Integral

> [!definition] Bestimmtes Integral (Riemann) #definition #formel
> Die Fläche unter $f$ über $[a;b]$ wird durch Rechtecke angenähert: die **Untersumme** (kleinster Funktionswert je Streifen) ist $\le$ Fläche $\le$ **Obersumme** (größter Wert). Verfeinert man die Streifenbreite ($n\to\infty$), streben beide gegen denselben Grenzwert, das **bestimmte Integral**:
> $$\int_a^b f(x)\,dx=\lim_{n\to\infty}\sum_{i=1}^{n} f(\xi_i)\,\Delta x.$$

![[integral-flaeche.svg|530]]
*Abbildung: Die Rechtecke (Riemann-Summe) nähern die Fläche unter $f$ an; im Grenzwert unendlich vieler, beliebig schmaler Rechtecke ergibt sich $\int_0^3 f(x)\,dx$.*

> [!definition] Deutung des Integrals #definition #merke
> - **Geometrisch:** (orientierter) Flächeninhalt zwischen Graph und $x$-Achse. Flächen **unter** der Achse zählen **negativ**.
> - **Inhaltlich:** aufsummierte Wirkung einer **Änderungsrate** → Gesamtänderung. Ist $f$ eine Rate (z. B. Zufluss in L/s), so ist $\int_a^b f\,dt$ die Gesamtmenge.

## 2. Stammfunktion und Hauptsatz

> [!definition] Stammfunktion / unbestimmtes Integral #definition #formel
> $F$ heißt **Stammfunktion** von $f$, wenn $F'(x)=f(x)$. Stammfunktionen sind nur bis auf eine additive **Konstante** eindeutig:
> $$\int f(x)\,dx=F(x)+C.$$
> Grundintegrale & Regeln: [[Stammfunktion & Integrationsregeln]]. Z. B. $\int x^n dx=\frac{x^{n+1}}{n+1}+C$ ($n\neq-1$).

> [!satz] Hauptsatz der Differential- und Integralrechnung #satz #formel
> Ist $F$ eine Stammfunktion von $f$, dann
> $$\int_a^b f(x)\,dx=\big[F(x)\big]_a^b=F(b)-F(a).$$
> Man braucht also keinen Grenzwert von Summen, sondern nur eine Stammfunktion. Begründung: [[Hauptsatz der Differential- und Integralrechnung]].

> [!beispiel] Bestimmtes Integral #beispiel
> $\int_0^2 (3x^2+1)\,dx=\big[x^3+x\big]_0^2=(8+2)-0=10.$

> [!beispiel] Vorzeichen beachten #beispiel #merke
> $\int_0^{2\pi}\sin x\,dx=[-\cos x]_0^{2\pi}=0$ — die Flächen über und unter der Achse heben sich auf. Für den **tatsächlichen Flächeninhalt** bei Nullstellen aufteilen und Beträge addieren → [[TP15 Anwendungen Integralrechnung]].

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. Erklären Sie die Idee der **Unter- und Obersummen**. Wie entsteht daraus das bestimmte Integral?
> 2. **Definieren Sie die Stammfunktion.** Warum die Integrationskonstante $C$?
> 3. Formulieren und deuten Sie den Hauptsatz.
> 4. Warum kann ein bestimmtes Integral null oder negativ sein, obwohl eine Fläche vorhanden ist?
> 5. Deuten Sie $\int_a^b f(t)\,dt$, wenn $f$ eine Änderungsrate ist (Kontextbeispiel).

## Verwandte Themen
[[TP15 Anwendungen Integralrechnung]] · [[TP11 Grundlagen Differentialrechnung]] · [[Stammfunktion & Integrationsregeln]] · [[Hauptsatz der Differential- und Integralrechnung]]
