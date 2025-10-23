---
Date-Added: 2025-10-03T15:24:00
Category:
  - Math
MOC: "[[Analiza Matematyczna - Wykłady]]"
type: basic-note
---
## Temat:
- - -


### Notatka Główna:
- [[Analiza Matematyczna - Wykłady]]
- - -
## Temat:Ciągi
##### Data: 03-09-2025
 - - -

### Ciąg geometryczny:
> to taki ciąg liczbowy, w którym każda kolejna liczba powstaje przez pomnożenie poprzedniej liczby przez q. Czyli dla dowolnego n∈ℕ+ zachodzi:
$$ a_{n+1} = a_{n} \cdot q
$$
##### Wzory na n-ty wyraz ciągu:
$$ a_{n} = a_{1} \cdot q^{n-1}
$$
$$ a_{n} = a_{k} \cdot q^{n-k}
$$
### Ciąg arytmetyczny:
>to taki ciąg liczbowy, w którym każda kolejna liczba różni się od poprzedniej o ustaloną wartość r, czyli dla dowolnego n∈ℕ+ zachodzi:
$$a_{n+1}=a_{n}+r$$


#### Definicja:
###### O ciągu (x_n) mówimy, że jest on 
###### 1. Rosnący:
 $$ \forall_{n \in N}, x_{n+1}>x_{n}
 $$
###### 2. Malejący:
 $$ \forall n \in N, x_{n+1}<x_{n}
 $$
###### 3. Niemalejący:
 $$ \forall n \in N, x_{n+1}\geq x_{n}
 $$
###### 4. Nierosnący:
 $$\forall n \in N, x_{n+1}\leq x_{n}
 $$
 
###### 5. Stały:
$$\forall n \in N, x_{n+1}=x_{n}
$$
- - - 
#### Badanie monotoniczności ciągu:
###### Badanie różnicą:
$$ a_{n+1}-a_{n}>0 \to \text{Ciąg rosnący}
$$
$$ a_{n+1}-a_{n}<0 \to \text{Ciąg malejący}
$$
###### Badanie ilorazem:
$$ \frac{a_{n+1}}{a_{n}} >1 \implies a_{n+1}>a_{n} \to \text{Ciąg rosnący}
$$
#### Ograniczenia ciągu:
###### Ograniczony z dołu:
$$ \exists_{m \in R} \forall_{n \in N}\space a_{n} \geq m
$$
$$ a_{n}= \frac{1}{n}, \exists_{m = 0} \forall_{n \in N}\space a_{n} \geq 0
$$
###### Nie istnieje ograniczenie z dołu:
$$ \exists_{m \in R} \forall_{n \in N}\space a_{n} < m
$$
###### Ograniczony z góry
$$ \exists_{M \in R} \forall_{n \in N}\space a_{n}\leq M
$$
###### Nie istnieje ograniczenie ciągu z góry:
$$ \exists_{M \in R} \forall_{n \in N} \space a_{n}> M
$$
###### Ograniczony (z dołu i z góry):