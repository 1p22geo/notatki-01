# Paradygmat oprogramowania
- obiektowy
- funkcyjny
- strukturalny
- imperatywny

# Programowanie obiektowe
- abstrakcja
    - interfejsy
    - metody wirtualne
    - klasy abstrakcyjne
- hermetyzacja
    - pola prywatne
    - metody prywatne i chronione
    - przestrzenie nazw
- polimorfizm
    - jedna metoda ma wiele implementacji
    - implementacja dobierana na podstawie typu
    - abstrakcja wyrażenia od typu
- dziedziczenie
    - klasy nadrzędne i pochodne

## Zasady paradygmatu obiektowego

### Zasady SOLID
- Single Responsibility Principle
    - Klasa lub moduł ma tylko jedną odpowiedzialność
    - Klasa powinna mieć jeden powód do zmiany
- Open/close Principle
    - Klasa jest otwarta na rozbudowę, a zamknięta na modyfikacje
- Liskov Substitution Principle
    - Jeśli w danej funkcji będzie wykorzystywany obiekt klasy potomnej, to wywołanie na nim metody pierwotnie zdefiniowanej w klasie bazowej powinno dać te same rezultaty
    - Obiekt klasy potomnej powinno dać się zastąpić obiektem klasy bazowej
- Interface Segregation Principle
    - Klient wykorzystujący interfejs nie musi obsługiwać metod których nie używa
    - Jeden interfejs na jeden typ klienta
- Dependency Inversion Principle
    - Wysokopoziomowe moduły nie powinny zależeć od modułów niskopoziomowych
    - Abstrakcje nie powinny być zależne od implementacji, tylko odwrotnie
### Keep it simple, stupid
- Nie pisać kodu "na zaś"
- Zawsze sprawdzać czy nie da się uprościć
- Jeśli fragment kodu jest zbędny, nie ma po co go trzymać
### Don't repeat yourself
- Wprowadzanie zmian jest łatwiejsze, gdy trzeba to zrobić w jednym miejscu
- Nie kopiować kodu, zrobić funkcje i klasy