# Złożoność obliczeniowa algorytmów, notacja duże O, 10.10.2023

Dobry algorytm jest:
- skuteczny
    - wykonuje to co w specyfikacji
- poprawny
    - przy poprawnych danych daje poprawny wynik
    - musi zakończyć obliczenia
    - ma własność stop
- szybki
    - rozsądny czas algorytmu
    - czy jest możliwy natychmiastowy wynik?


Złożoność alogrytmu
---

- złożoność pamięciowa
    - określa ile pamięci zużywa program
- złożoność czasowa
    - ile operacji wiodących potrzebuje algorytm

Złożoność obliczeniowa
---
Złożoność dokładna
- dane pesymistyczne
- dane optymistyczne

```cpp
int sum(int[] numbers){
    int sum = 0;
    for(int number:numbers){
        sum += number
    }
    return sum;
}
```

$f(n) = 1+(n+1)$

$f(n) = n+2$

#### Złożoność tego algorytmu to  O(n)


Notacja duże O
---
- $O(1)$ - złożoność stała
    - algorytm nie iteruje, czas wykonania nie zależy od ilości danych
- $O(n)$ - złożoność liniowa
    - czas wykonania zależy od ilości elementów *wprost proporcjonalnie*
    - np. iteracja przez wszyskie elementy
- $O(log\;n)$ - złożoność logarytmiczna
    - np. zależy od $log_2(n)$, bo dzieli tabelę na 2 i dla każdej połówki powtarza rekurencyjnie algorytm
    - *quicksort*
- $O(n\;log\;n)$ - złożoność liniowo-logarytmiczna
    - zależy od $log_2(n)$ ale dla każdej iteracji iteruje przez wszystkie elementy jeszcze raz
    - *mergesort*
- $O(n^2)$ - złożoność kwadratowa
    - iteracja przez wszystkie elementy *dla każdego elementu*
    - *bubble sort, select sort, shaker sort*
- $O(x^n)$ - złożoność wykładnicza
    - wszystkie podzbiory tabeli
    - wszystkie możliwe funkcje między dwoma zbiorami
- $O(n!)$ - złożoność silni
    - problem komiwojażera
    - wszystkie permutacje zbioru