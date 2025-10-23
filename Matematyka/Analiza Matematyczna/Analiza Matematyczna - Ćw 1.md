---
Date-Added: 2025-10-09T12:15:00
Category:
  - Math
MOC: "[[Analiza Matematyczna - Ćwiczenia]]"
type: basic-note
---

## Temat: Ciągi

---

- [ ] Uzupełnić notatkę

#### Podstawowe działania na ciągach

$$x_{n} = 1+(-1)^{n}$$
$$x_{2008}= 1+(-1)^{2008} = 2$$
$$x_{2008}= 1+(-1)^{2009} = 0$$

#### Definicja silni:

$$x_{n} = 1+2+3\dots + n = \frac{(n+1)}{2}*n$$

$$x_{2008}= \frac{2008+1}{2}*2008$$
$$x_{2009}-x_{2008}= 1+2+3\dots+2008+2009 - (1+2+3+\dots+2008) = 2009$$

$$x_{n}=\frac{1}{n!}+\frac{1}{(n+1)!}\dots+\frac{1}{2n!}$$

$$x_{1}=\frac{1}{1!}+\frac{1}{2!}$$
$$x_{2}=\frac{1}{2!}+\frac{1}{3!}+\frac{1}{4!}$$
$$x_{2n}=\frac{1}{2n!}+\frac{1}{(2n+1)!}\dots+\frac{1}{4n!}$$
$$x_{2n}=\frac{1}{2n-1!}+\frac{1}{(2n+1)!}\dots+\frac{1}{(4n-2!)}$$
$$x_{2n}-x_{2n-1}= \frac{1}{2n!}+\frac{1}{(2n+1!)}+\dots+\frac{1}{(4n-1)!}+\frac{1}{(4n)!}=\frac{1}{(4n-1)!}+\frac{1}{(4n!)}-\frac{1}{(2n-1)!}$$

###### Układ równań:

x*{1} = 1
x*{n} = 2x\_{n-1}+1, n>=2

x*{2} = 2x*{1}+1 = 3
x*{3} = 2x*{2}+1 = 7

#### Badanie monotoniczności:

$$x_{n+1}-x_{n}>0$$
$$x_{n+1}>x_{n}$$
$$\frac{x_{n+1}}{x_{n}}>1$$
$$x_{n+1}>x_{n}$$
$$x_{n}=\frac{n}{3n+1}$$
$$x_{n+1}=\frac{n+1}{3(n+1)+1}$$
$$x_{n+1}-x_{n}=\frac{n+1}{3(n+1)+1} - \frac{n}{3n+1} = \frac{(n+1)(3n+1)-n(3n+4)}{(3n+4)(3n+1)}=\frac{3n^2+n+3n+1-3n^2-4n}{(3n+4)(3n+1)}>0 $$
$$x*{n}=\frac{10^n}{(2n)!}$$
$$X*{n+1}=\frac{10^{n+1}}{(2n+2)!}$$

$$
\frac{x_{n+1}}{x_{n}} = \frac{\frac{10^{n+1}}{(2n+2)!}}{\frac{10^n}{(2n)!}} = \frac{10}{(2n+1)(2n+2)}\leq \frac{10}{12}<1
$$

- ciag malejący
  $$x_{n} = n-2^n$$
  $$x_{n+1}- x_{n} = n+1-2^{n+1}-(n-2^n) = 1-2^n(2-1) = 1-2^n<0$$

###### Sprawdzenie:

$$n\geq 1$$
$$2^n\geq 2$$
$$-2^n\leq -2$$
$$1-2^n\leq -2+1 < 0$$
$$x_{n}=n^2-n$$
$$x_{n+1}=(n+1)^2-(n+1)$$
$$x_{n+1}-x_{n}=(n+1)^2-(n+1)-(n^2-n) = 2n>0$$
$$x_{n}=n!$$
$$x_{n+1} = (n+1)!$$
$$\frac{x_{n+1}}{x_{n}}=\frac{(n+1)!}{n!} = n+1>1$$

$$x_{n} = \frac{n+2}{n}$$
$$x_{n+1}=\frac{n+3}{n+1}$$
$$x_{n+1}-x_{n}=\frac{(n+2)(n+1)}{n^2+n}-\frac{(n^2+2n)}{n^2+n}=\frac{n^2+2n+n+2 -n^2-2n}{n^2+n}=\frac{-2}{n(n+1)}<0$$
ciąg malejący - poprawić obliczenia!

$$x_{n}=\frac{n}{3^n}$$
$$\frac{x_{n+1}}{x_{n}}=\frac{n+1}{3*3^n}* \frac{3^n}{n} = \frac{1}{3}\left( \frac{n+1}{n} \right)<1$$
ciąg malejący - uzupełnić o sprawdzenie
$$x_{n}=\sqrt{n^2+1 }$$
$$x_{n}=\sqrt{(n+1)^2+1 }$$
$$\frac{x_{n+1}}{x_{n}}=\frac{\sqrt{(n+1)^2+1 }}{\sqrt{ n^2+1 }} = \sqrt{ \frac{n^2+2n+2}{n^2+1} }>1$$
Dopisać uzasadnienie

Wykres kosinusa:

$$x_{n}=\cos \frac{\pi}{n}$$
$$x_{1}=\cos \frac{\pi}{1} = -1$$
$$x_{2}=\cos \frac{\pi}{2} = 0$$
$$\cos \frac{\pi}{n}<\cos \frac{\pi}{n+1}$$

Ograniczoność ciągu:
