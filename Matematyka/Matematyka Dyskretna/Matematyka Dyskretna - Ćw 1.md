---
Date-Added: 2025-10-02T10:00:00
Category:
  - Math
MOC: "[[Matematyka Dyskretna - Ćwiczenia]]"
type: basic-note
---

## Temat:Wstęp do matematyki dyskretnej
- - -


### Zbiory - Przykłady:
- {0,1,2} - zbiór 3 elementowy
- {A,B,C,...Z} - Alfabet
- {1,2,3,4,5,6,....} = N+ - Liczby naturalne
- {0,1,2,3,4,5,6,....} = N0 - Liczby naturalne z zerem
- {p: p=2*n, n E N0} - liczby parzyste (Zero jest liczbą parzystą)
- {...,-2,-1,0,1,2...} - Z - liczby rzeczywiste
-  an = 2^n ,n E N

### Zadania:
##### Twierdzenie małego Gaussa:
1+2+3+4... +n = (n*(n+1)) / 2 
z1:
$$
\sum_{k=-3}^{0} \to (1-k) = (1-(-3))+(1-(-2))+(1-(-1))+(1-0)
$$
z2:
$$ \sum_{i=1}^{3} (\sum_{j=1}^{2}ij^2) = \sum_{i=1}^{3}(i*1^2+i*2^2) = (1*1^2 + 1*2^2) + (2*1^2 + 2*2^2) + (3*1^2 + 3*2^2) =\dots
$$
z3:
$$ \sum_{k=1}^{2} \sum_{n=1}^{4} (k-n) =\sum_{k=1}^{2} [(k-1)+(k-2)+(k-3)+(k-4)] = \sum_{k=1}^{2}(4k-10) = (4*1-10)+(4*2-10) = (4-10)+(*-10) = 8
$$
z4:
$$ \prod_{k=-3}^{-1}(2-k)^k = (2-(-3))^{-3} \space \cdot (2-(-2))^{-2} \space \cdot (2-(-1))^{-1} = \dots
$$
### Różnica symetryczna suma zbiorów (współczynnik kartezjański): 
$$(A-B) \cup(B-A)=A\oplus B$$
##### Przykład:
$$A=\{ 1,2,3 \} ,B=\{ 1,4,6\}$$
$$A\oplus B=\{ 2,6 \}$$

### Iloczny Kartezjański:
$$AXB = \{ \{a,b  \}: a\in A,b\in B \}$$
$$AXB=\{ (1,1) (1,4), (1,6), (2,1), (2,4), (2,6), (4,1), (4,4), (4,6) \}$$

###### Ilość elementów Iloczynu kartezjańskiego ->Ilość elementów zbioru A * Ilość elementów zbioru B.