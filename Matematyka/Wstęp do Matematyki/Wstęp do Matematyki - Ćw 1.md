---
Date-Added: 2025-10-07T14:19:00
Category:
  - Math
MOC: "[[Wstęp do Matematyki - Ćwiczenia]]"
type: basic-note
---
## Temat: Wprowadzenie do logiki
- - -
Logika:
Zdania (matematyczne) mogą być prawdziwe lub fałszywe

Zmienne p i q:

| p   | q   | p^q | pvq | p=>q | XOR |
| --- | --- | --- | --- | ---- | --- |
| 0   | 0   | 0   | 1   | 1    | 0   |
| 0   | 1   | 0   | 1   | 0    | 1   |
| 1   | 0   | 0   | 0   | 0    | 1   |
| 1   | 1   | 1   | 1   | 0    | 0   |

| p   | ~p  |
| --- | --- |
| 0   | 1   |
| 1   | 0   |
^ -> koniunkcja 'i'
v -> lub
<=> -> równoważnośc

Zdania:
p=q=1
r=s=0
(p^r)=>(pvs) -> 1 zdanie prawdziwe
(p<=>q)<=>(r<=>s) -> 1 zdanie prawdziwe
(p^r)v(q^s) -> 0 Zdanie fałszywe

tautologia =? (definicja)
> Zdanie zawsze prawdziwe
#### Przykłady:
##### Przykład 1:

$$\psi = \neg (p\land q)\iff(\neg p\land\neg q)
$$
###### Tablica prawdy:

| p   | q   | p^q | ~(p^q) | ~p  | ~q  | ~p^~q | \psi |
| --- | --- | --- | ------ | --- | --- | ----- | ---- |
| 0   | 0   | 0   | 1      | 1   | 1   | 1     | 1    |
| 0   | 1   | 0   | 1      | 1   | 0   | 0     | 0    |
| 1   | 0   | 0   | 1      | 0   | 1   | 0     | 0    |
| 1   | 1   | 1   | 0      | 0   | 0   | 0     | 1    |
##### Przykład 2:
$$(p\implies q)/\iff(\neg p\implies\neg q)
$$

###### Tablica prawdy:

| p   | q   | p=>q | ~p  | ~q  | ~p=>~q | (p=>q)<=>(~p=>~q) | \psi |
| --- | --- | ---- | --- | --- | ------ | ----------------- | ---- |
| 0   | 0   | 1    | 1   | 1   | 1      | 1                 | 1    |
| 0   | 1   | 1    | 1   | 0   | 0      | 0                 | 0    |
| 1   | 0   | 0    | 0   | 1   | 1      | 0                 | 0    |
| 1   | 1   | 1    | 0   | 0   | 1      | 1                 | 1    |
##### Przykład 3:
$$(p\implies q\lor(p\implies\neg q))
$$
###### Tablica Prawdy:

| p   | q   | p=>q | p=>~q | (p=>q)v(p=>~q) | \psi |
| --- | --- | ---- | ----- | -------------- | ---- |
| 0   | 0   | 1    | 0     | 1              | 1    |
| 0   | 1   | 1    | 1     | 1              | 0    |
| 1   | 0   | 0    | 1     | 1              | 0    |
| 1   | 1   | 1    | 1     | 1              | 1    |
##### Prawa logiczne:
###### Prawo 1:
$$\neg\neg p \iff p$$
###### Prawo 2:
$$\neg(p\land q) \iff (\neg p\land\neg q)$$
###### Prawo 3:
$$\neg(p\lor q)\iff(\neg p\lor\neg q)$$
###### Prawo 4:
$$(p\implies q)\iff(\neg p\implies\neg q)$$

###### Prawo 5:
$$(p\land q)\implies p$$
###### Prawo 6:
$$p\implies(p\lor q)$$
###### Prawo 7:
$$(p\iff q)\iff[(p\implies q)\land (p\implies q)]$$


Zapis poprzez operatory ~ v
(p^q)<=>~(~pv~q)
(p=>q)<=>~(p^~q)<=>~pvq

(p<=>q)<=>[(p=>q)^(p=>q)]<=>[(~pvq)^(~pvq)]

(p o+ q)<=>[~(p=>q)v~(q=>p)]<=>~(q=>p^q=>p)<=>~(p<=>q)

(p^~q)=>(qv~q) -> 1
(pv~ ~ ~p)<=>(p v ~p) -> 1
~(p^~p)-> 1
~(p^q^r^s)<=>~(~p v ~q v ~r v ~s)<=>(~(p^q)v~(r^s))<=>((~pv~q)v(~rv~s))

Kfantyfikatory:
\forall_{xER} p(x) -> X^2 >=0 --> Dla każdego XER zdanie X^2 jest prawdziwe

\exists_{xER} p(x) -> X^2 < X --> Istnieje taki X dla którego zdanie X^2>X jest prawdziwe

\forall_{xER} X^2 =X -> 1 - Zdanie prawdziwe

\forall_{xER} (x<1) ^ (X^2>x)
\forall_{xER} \forall_{yER} (y^2=x => \exists_{zER} z<5 ^ z>7)

\forall_{x} p(x)=>\exists_{x}

~(\forall_{x} )<=>\exists_{x} ~p(x)
~\exists_{x} p(x) <=>\forall_{x} ~p(x) 

(~\exists_{x} x^2<2 ^ x>7)<=> \forall_{x} x^2>=2 v x<=7

każde 2 liczby naturalne mają wspólnu dzilenik:

Nie isteniej najwieksa liczba rzeczywista:

Każda liczba podzilna przez 6 jest pażysta:
\forall_{xEN} 6|x=>2|x
30 i 20


