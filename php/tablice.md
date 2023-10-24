# Tablice w PHP

# tablica asocjacyjna
```php
$tab = array(
        'name' => 'Marian',
        'surname' => 'Paździoch',
        'age' => 40,
        'job'  => 'menda jedna zarośnięta',
        'homo' => true
    );

```
### pobieranie elementów
```php
var_dump($tab["name"]) // pobiera elemęt o kluczu name
```
## sortowanie
```php
asort($tab) // według wartości
ksort($tab) // według kluczy
```
## iteracja
```php
foreach($tab as $key){
    echo $key . "<br>";
}
```
albo
```php
foreach($tab as $key => $value){
    echo $key . "=>". $value . "<br>";
}
```

<br>
<br>
<br>

# tablica nieasocjacyjna
```php
$tab = [4,1,6,5] // dekraracja i definicja tablicy
```
## pobieranie elementów
```php
var_dump($tab[1]) // zwróci 4
```
## sortowanie
```php
sort($tab) // rosnąco
rsort($tab) // majejąco
```