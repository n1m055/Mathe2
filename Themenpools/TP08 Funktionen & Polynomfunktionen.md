---
themenpool: 8
titel: "Allgemeines über Funktionen, Potenz- und Polynomfunktionen"
gebiet: Funktionen
tags: [themenpool, funktionen, polynomfunktion, potenzfunktion, eigenschaften]
quelle: ["Themenpool 8", "Notizbuch 6B (2023/24)", "Notizbuch 7B (2024/25)"]
verwandt: ["[[TP02 Lineare & quadratische Modelle]]", "[[TP12 Funktionsuntersuchungen]]", "[[Funktionseigenschaften]]"]
---

# TP08 — Funktionen, Potenz- & Polynomfunktionen

> [!info] Leitidee
> Eine **Funktion** ordnet jedem Eingang genau einen Ausgang zu. Dieser Themenpool sammelt das Vokabular der Funktionsuntersuchung (Monotonie, Krümmung, Symmetrie, Extrem-/Wendestellen) — dieselbe Sprache, die später die [[TP12 Funktionsuntersuchungen|Differentialrechnung]] mit Ableitungen präzisiert.
>
> Quelle: [[00 Start - Maturastoff Mathematik 2026|Themenpool 8]] · Notizbuch **6B/7B**

## 1. Der Funktionsbegriff

> [!definition] Funktion #definition
> Eine **Funktion** $f:D\to Z$ ist eine Zuordnung, die **jedem** Element $x$ der **Definitionsmenge** $D$ **genau ein** Element $f(x)$ der **Zielmenge** $Z$ zuordnet. $f(x)$ heißt **Funktionswert** an der Stelle $x$.
> Die **Wertemenge** $W=\{f(x)\mid x\in D\}\subseteq Z$ ist die Menge der tatsächlich angenommenen Werte.
> **Senkrechten-Test:** Jede vertikale Gerade schneidet den Graphen höchstens einmal.

> [!definition] Eigenschaften von Funktionen #definition #merke
> - **Monotonie:** streng steigend, falls $x_1<x_2\Rightarrow f(x_1)<f(x_2)$ (analog fallend).
> - **Krümmung:** linksgekrümmt = **konvex**, rechtsgekrümmt = **konkav**.
> - **Symmetrie:** **gerade** $f(-x)=f(x)$ (achsensymmetrisch zur $y$-Achse), **ungerade** $f(-x)=-f(x)$ (punktsymmetrisch zum Ursprung).
> - **Extremstelle** (lokaler Hoch-/Tiefpunkt), **Wendestelle** (Krümmungswechsel), **Nullstelle** ($f(x)=0$), **Pol/Asymptote**, **Periodizität**.
> Bildliche Übersicht: [[Funktionseigenschaften]].

> [!definition] Injektiv, surjektiv, bijektiv, Umkehrfunktion #definition #satz
> - **injektiv:** verschiedene Argumente → verschiedene Werte ($x_1\neq x_2\Rightarrow f(x_1)\neq f(x_2)$; Horizontaltest).
> - **surjektiv:** jeder Wert der Zielmenge wird angenommen ($W=Z$).
> - **bijektiv** = injektiv **und** surjektiv ⇒ **umkehrbar**: es existiert die **Umkehrfunktion** $f^{-1}$ mit $f^{-1}(f(x))=x$. Ihr Graph entsteht durch Spiegelung an $y=x$ (Beispiel: [[Logarithmus]] als Umkehrung der Exponentialfunktion, [[TP09 Exponential- & Logarithmusfunktion]]).

## 2. Potenzfunktionen

> [!definition] Potenzfunktion #definition #formel
> $$f(x)=a\cdot x^{z},\qquad z\in\mathbb{Z}\ (\text{bzw. }\mathbb{Q}).$$
> | $z$ | Gestalt | Symmetrie | Verhalten |
> |---|---|---|---|
> | gerade $>0$ | parabelartig | gerade | $W=[0;\infty)$, U-/∩-Form |
> | ungerade $>0$ | $x^3$-artig | ungerade | streng monoton |
> | $z<0$ | hyperbelartig $\frac{1}{x^{|z|}}$ | je nach $z$ | Pol bei $x=0$, Asymptoten |
>
> Parameter $a$: streckt/staucht ($|a|$) und spiegelt ($a<0$).

## 3. Polynomfunktionen

> [!definition] Polynomfunktion #definition #formel
> $$f(x)=a_nx^n+a_{n-1}x^{n-1}+\dots+a_1x+a_0,\qquad a_n\neq0.$$
> $n$ = **Grad**, $a_n$ = **Leitkoeffizient**, $a_0=f(0)$ = absolutes Glied. Definitionsmenge $D=\mathbb{R}$.

![[polynom.svg|470]]
*Abbildung: $f(x)=x^3-3x$ mit den Nullstellen $0,\pm\sqrt3$ (alle einfach, der Graph schneidet); ungerade Funktion mit Globalverhalten von $-\infty$ nach $+\infty$.*

> [!satz] Zentrale Eigenschaften #satz #merke
> - **Höchstens $n$ Nullstellen** ([[Fundamentalsatz der Algebra]]); Faktorisierung über [[Polynomdivision]] / [[Satz von Vieta]].
> - **Vielfachheit** einer Nullstelle: ungerade → Graph **schneidet** die $x$-Achse, gerade → **berührt** sie.
> - **Globalverhalten** ($x\to\pm\infty$) bestimmt allein der höchste Term $a_nx^n$:
>   - $n$ gerade, $a_n>0$: beide Äste $+\infty$; $a_n<0$: beide $-\infty$.
>   - $n$ ungerade, $a_n>0$: von $-\infty$ nach $+\infty$; $a_n<0$ umgekehrt.
> - **Symmetrie:** nur gerade Exponenten → gerade Funktion; nur ungerade → ungerade.

> [!beispiel] Polynom analysieren #beispiel
> $f(x)=x^3-3x=x(x^2-3)=x(x-\sqrt3)(x+\sqrt3)$. Nullstellen $0,\pm\sqrt3$ (einfach → schneiden), ungerade Funktion, Globalverhalten $-\infty\to+\infty$. Genaue Hoch-/Tiefpunkte → [[TP12 Funktionsuntersuchungen]].

---

## Mündliche Prüfungsfragen
> [!frage] #frage
> 1. **Definieren Sie den Funktionsbegriff** präzise (Definitions-, Ziel-, Wertemenge). Was prüft der Senkrechten-Test?
> 2. Definieren Sie Monotonie, Krümmung und die beiden Symmetriearten — wie erkennt man sie am Term?
> 3. Was bedeutet **bijektiv** und welcher Zusammenhang besteht zur Umkehrfunktion?
> 4. Wie bestimmen Grad und Leitkoeffizient das Globalverhalten?
> 5. Was sagt die Vielfachheit einer Nullstelle über den Graphen?

## Verwandte Themen
[[TP02 Lineare & quadratische Modelle]] · [[TP09 Exponential- & Logarithmusfunktion]] · [[TP12 Funktionsuntersuchungen]] · [[Funktionseigenschaften]] · [[Polynomdivision]] · [[Satz von Vieta]] · [[Fundamentalsatz der Algebra]]
