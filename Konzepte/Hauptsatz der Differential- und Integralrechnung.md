---
typ: konzept
titel: "Hauptsatz der Differential- und Integralrechnung"
tags: [konzept, satz, formel, analysis]
verwandt: ["[[Stammfunktion & Integrationsregeln]]", "[[TP14 Grundlagen Integralrechnung]]"]
---

# Hauptsatz der Differential- und Integralrechnung

> [!satz] Satz #satz #formel
> Ist $F$ eine Stammfunktion von $f$ (also $F'=f$), dann
> $$\int_a^b f(x)\,dx=\big[F(x)\big]_a^b=F(b)-F(a).$$
> **Kernaussage:** Differenzieren und Integrieren sind **Umkehroperationen**. Die Flächenfunktion $\Phi(x)=\int_a^x f(t)\,dt$ erfüllt $\Phi'(x)=f(x)$.

![[integral-flaeche.svg|480]]
*Abbildung: Das bestimmte Integral ist der Grenzwert der Riemann-Summe — der Hauptsatz berechnet ihn als $F(b)-F(a)$.*

> [!merke] Bedeutung #merke
> Statt mühsamer Grenzwerte von Unter-/Obersummen genügt **eine Stammfunktion**. Das macht Flächen-, Volumen- und Mengenberechnungen praktisch durchführbar.

> [!beispiel] Beispiel #beispiel
> $\int_1^3 2x\,dx=[x^2]_1^3=9-1=8$. (Probe: Trapezfläche unter $y=2x$: $\frac{2+6}{2}\cdot2=8$ ✓.)

Stammfunktionen: [[Stammfunktion & Integrationsregeln]]. Anwendungen: [[TP15 Anwendungen Integralrechnung]].
