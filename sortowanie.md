# Algorytmy wyszukiwania

## algorytm sekwencyjny - O(n)
przeszukujemy powoli wszystkie elementy
## wyszukiwanie binarne - O(log n)
kolejność jest potrzebna, elementy muszą być posortowane

# Algorytmy sortowania

## sortowanie przez wstawianie (insert sort) O(n^2)

kolejne elementy wstawiamy na właściwe miejsca, zamieniając elementy

```
tabela a[8]

wskażnik na jeden z nich - x* = a
``````

elementy są przesuwane z prawej na lewo, są zamieniane miejscami jeśli są w złej kolejności

```
x++;

if(*x<*(x-1)){
	zamień x i x-1
}
```

## sortowanie bąbelkowe (bubble sort) O(n^2)

koejne pary elementów zamieniamy, jeśli są w złej kolejności, od pierwszej pary (a[0] i a[1]) do ostatniej (a[7] i a[8])
po zamienieniu wszystkich par, wracamy do początku
element umieszczony na końcu, już się z niego nie ruszy, więc możemy go usunąć (lub "zablokować")


## quick sort O(n log n)


Wybieramy jeden element (**pivot**), elementy mniejsze od niego ładujemy na jedną tablicę, większe na drugą.
Każdą z nich sortujemy tym samym algorytmem (rekurencyjnie)


## select sort

Wybieramy jeden element i idziemy w prawo od niego. Jeśli znajdziemy element mniejszy, zamieniamy je.


## Merge sort - O(n log n)

Dzielimy tablicę w połowie, tak długo aż mamy tablice jednoelementowe,
następnie scalamy tablice specjalnym algorytmem scalania.
Algorytm wykorzystuje drugą tablicę, złożoność pamięciowa jest więc większa