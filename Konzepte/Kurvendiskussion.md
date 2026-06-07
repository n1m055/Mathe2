---
typ: konzept
titel: "Kurvendiskussion (Schema)"
tags: [konzept, verfahren, analysis, herleitung]
verwandt: ["[[TP12 Funktionsuntersuchungen]]", "[[Ableitungsregeln]]", "[[Funktionseigenschaften]]"]
---

# Kurvendiskussion

> [!definition] Was ist eine Kurvendiskussion? #definition
> Die **Kurvendiskussion** ist die systematische Untersuchung aller charakteristischen Eigenschaften eines Funktionsgraphen (Nullstellen, Extrem-, Wendestellen, Symmetrie, Verhalten im Unendlichen) mithilfe von $f$, $f'$ und $f''$.

> [!merke] Schema #merke
> 1. **Definitionsmenge**, Symmetrie, Verhalten für $x\to\pm\infty$, Asymptoten
> 2. **Nullstellen:** $f(x)=0$
> 3. **Extremstellen:** $f'(x)=0$; Art über $f''$ ($<0$ Hoch, $>0$ Tief) oder Vorzeichenwechsel
> 4. **Wendestellen:** $f''(x)=0$ mit Vorzeichenwechsel; ggf. Sattelpunkt
> 5. **Skizze**

![[kurvendiskussion.svg|460]]
*Abbildung: $f(x)=x^3-3x$ mit Hochpunkt $(-1\mid2)$, Tiefpunkt $(1\mid-2)$ und Wendepunkt $(0\mid0)$.*

> [!beispiel] Durchgerechnet — $f(x)=x^3-3x$ #beispiel #herleitung
> $D=\mathbb{R}$, ungerade, $x\to\pm\infty\Rightarrow f\to\pm\infty$. Nullstellen $x=0,\pm\sqrt3$.
> $f'(x)=3x^2-3=0\Rightarrow x=\pm1$; $f''(x)=6x$: $f''(1)>0$ → Tief $(1\mid-2)$, $f''(-1)<0$ → Hoch $(-1\mid2)$.
> $f''(x)=0\Rightarrow x=0$, Vorzeichenwechsel → Wendepunkt $(0\mid0)$.

Theorie & Anwendungen: [[TP12 Funktionsuntersuchungen]]. Regeln: [[Ableitungsregeln]]. Begriffe: [[Funktionseigenschaften]].
