---
Date-Added: 2025-10-21T10:22:00
Category:
  - Math
MOC: "[[Wstęp do Matematyki - Ćwiczenia]]"
type:
  - basic-note
  - zadania
---
Notatki na podstawie filmów:
[Video](https://www.youtube.com/watch?v=Wf9wBm2j5oo&list=PLn4jDcZVwTZ7OD2_SiPI2ywiUJq_jdYig)
#### Logika:
Zdanie -> jest możliwe jednoznaczne przypisanie czy zdanie jest prawdziwe lub fałszywe

Przykłady:

2+2 = 5 -> zdanie fałszywe => zdanie w znaczeniu logicznym

Dziś jest ładna pogoda => nie jest to zdanie w znaczeniu logicznym, bo nie wiadomo kiedy jest dzisiaj i czym jest ładna pogoda

xEN => nie jest zdaniem bo nie wiadomo czym jest x

Zdaniom przypisuje się litery: pq,r,s,t ...
##### Wartości logiczne:
- 1 -> prawda
- 0 -> fałsz

w(p) = 1 -> wartość logiczna zdania 'p' jest równe 1. Zdanie logiczne 'p' jest prawdziwe

#### Spójniki logiczne i negacja

##### Negacja '~':
 -  $\neg$ zamiana zdania z prawdy -> fałsz lub fałsz -> prawda
 - w(p) = 1 -> w($\neg$p) = 0
###### Tablica prawdy:
 

| p   | $\neg$p |
| --- | ------- |
| 0   | 1       |
| 1   | 0       |

##### Spójnik - koniunkcja:
- opisany słowem {i, oraz} łączy dwa zdania na tym samym szczeblu
- $\land$ -> spójnik, który wymusza że oba zdania były prawdziwe

| p   | q   | p$\land$q |
| --- | --- | --------- |
| 0   | 0   | 0         |
| 1   | 0   | 0         |
| 0   | 1   | 0         |
| 1   | 1   | 1         |
##### Spójnik - alternatywa:
- opisany słowem {lub} łączy dwa zdania na tym samym szczeblu
- $\lor$ -> spójnik, który wymusza że chociaż jedno ze zdań musi być prawdziwa

| p   | q   | p$\lor$q |
| --- | --- | -------- |
| 0   | 0   | 0        |
| 1   | 0   | 1        |
| 0   | 1   | 1        |
| 1   | 1   | 1        |
##### Spójnik - Równoważność zdań:
- zdania są takie same, maja taką samą wartość logiczną
- <=> -> spójnik który wymusza żeby oba zdania miały jednakową wartość logiczną

| p   | q   | p$\iff$q |
| --- | --- | -------- |
| 0   | 0   | 1        |
| 1   | 0   | 0        |
| 0   | 1   | 0        |
| 1   | 1   | 1        |
##### Spójnik - Implikacja:
- "obietnica" (Jeżeli dziś jest wtorek, to się nie wyśpię).**Jeśli ..., to ...**
- $\implies$ -> jeśli pierwsze zdanie jest fałszywe to"obietnica" nie obejmuje zdania drugiego)
- poprzednik (założenie)$\implies$następnik (teza)

| p   | q   | p$\implies$q |
| --- | --- | ------------ |
| 0   | 0   | 1            |
| 1   | 0   | 0            |
| 0   | 1   | 1            |
| 1   | 1   | 1            |
##### Interpunkcja - kolejność spójników logicznych
 - Zdania należy analizować zgodnie z nawiasami
 - Najbardziej wiążąca jest negacja, póżniej koniunkcja i alternatywa, a nastpenie dopiero implikacja i równoważność
 

#### Prawa Rachunku Zdań - tautologia:
- Niezależnie od poszczególnych zdań, zdanie zawsze jest prawdziwe
$p\land \neg q \implies (p \implies q)$ <- nie jest to tautologia

| p   | q   | $\neg$q | p$\land \neg$q | p=>q | $p\land \neg q \implies (p \implies q)$ |
| --- | --- | ------- | -------------- | ---- | --------------------------------------- |
| 0   | 0   | 1       | 0              | 1    | 1                                       |
| 0   | 1   | 0       | 0              | 1    | 1                                       |
| 1   | 0   | 1       | 1              | 0    | 0                                       |
| 1   | 1   | 0       | 0              | 1    | 1                                       |
##### Prawa de Morgana - negacja koniunkcji i alternatywy:
- $\neg (p\lor q)\iff \neg p\land \neg q$ -> Negacja alternatywy

| p   | q   | $(p\lor q)$ | $\neg (p\lor q)$ | $\neg p\land \neg q$ | $\neg (p\lor q)\iff \neg p\land \neg q$ |     |
| --- | --- | ----------- | ---------------- | -------------------- | --------------------------------------- | --- |
| 0   | 0   | 0           | 1                | 1                    | 1                                       |     |
| 1   | 0   | 1           | 0                | 0                    | 1                                       |     |
| 0   | 1   | 1           | 0                | 0                    | 1                                       |     |
| 1   | 1   | 1           | 0                | 0                    | 1                                       |     |
- $\neg (p\land q)\iff \neg p \lor \neg q$ -> Negacja koniunkcji

| p   | q   | $(p\land q)$ | $\neg (p\land q)$ | $\neg p\lor \neg q$ | $\neg (p\land q)\iff \neg p\lor \neg q$ |
| --- | --- | ------------ | ----------------- | ------------------- | --------------------------------------- |
| 0   | 0   | 0            | 1                 | 1                   | 1                                       |
| 1   | 0   | 0            | 1                 | 1                   | 1                                       |
| 0   | 1   | 0            | 1                 | 1                   | 1                                       |
| 1   | 1   | 1            | 0                 | 0                   | 1                                       |
##### Łączność alternatywy i koniunkcji:
