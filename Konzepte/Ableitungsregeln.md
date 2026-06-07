---
typ: konzept
titel: "Ableitungsregeln"
tags: [konzept, formel, analysis, ableitung]
verwandt: ["[[Differentialquotient]]", "[[Stammfunktion & Integrationsregeln]]", "[[TP12 Funktionsuntersuchungen]]"]
---

# Ableitungsregeln

> [!formel] Grundableitungen #formel
> | $f(x)$ | $f'(x)$ |
> |---|---|
> | $c$ (konstant) | $0$ |
> | $x^n$ | $n\,x^{n-1}$ |
> | $\sqrt{x}=x^{1/2}$ | $\frac{1}{2\sqrt{x}}$ |
> | $\frac{1}{x}=x^{-1}$ | $-\frac{1}{x^2}$ |
> | $e^{x}$ | $e^{x}$ |
> | $a^{x}$ | $a^{x}\ln a$ |
> | $\ln x$ | $\frac{1}{x}$ |
> | $\sin x$ | $\cos x$ |
> | $\cos x$ | $-\sin x$ |

> [!important] Verknüpfungsregeln #formel #satz
> - **Faktorregel:** $(c\,f)'=c\,f'$
> - **Summenregel:** $(f\pm g)'=f'\pm g'$
> - **Produktregel:** $(f\cdot g)'=f'g+fg'$
> - **Quotientenregel:** $\left(\dfrac{f}{g}\right)'=\dfrac{f'g-fg'}{g^2}$
> - **Kettenregel:** $\big(f(g(x))\big)'=f'(g(x))\cdot g'(x)$ („äußere mal innere Ableitung")

> [!example] Beispiele #beispiel
> - $\big(3x^4\big)'=12x^3$
> - $\big(x^2 e^x\big)'=2x e^x+x^2 e^x=e^x(x^2+2x)$ *(Produktregel)*
> - $\big(\sin(3x)\big)'=3\cos(3x)$ *(Kettenregel)*
> - $\big(e^{-2x}\big)'=-2e^{-2x}$

> [!note] Höhere Ableitungen #merke
> $f''=(f')'$ (Krümmung), $f'''$ usw. Brauchst du für [[Kurvendiskussion]] und [[TP12 Funktionsuntersuchungen]].

Umkehrung = Integrieren: [[Stammfunktion & Integrationsregeln]]. Definition: [[Differentialquotient]].
