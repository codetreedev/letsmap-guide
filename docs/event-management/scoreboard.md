# Tabela wyników

Tabela wyników w aplikacji Let's Map to kompleksowy system rankingowy, który umożliwia śledzenie postępów drużyn oraz wyświetlanie aktualnych wyników gry. System składa się z dwóch głównych widoków: tabeli wyników z rankingiem drużyn oraz przeglądu postępu gry.

## Dostęp do tabeli wyników

Tabela wyników jest dostępna dla wszystkich uczestników wydarzenia. Aby ją otworzyć:

1. Przejdź do głównego ekranu wydarzenia
2. Znajdź w menu przycisk **"Tabela wyników"** 
3. Kliknij, aby otworzyć widok wyników

## Interfejs tabeli wyników

System składa się z dwóch zakładek:

### Zakładka "Ranking"

Główny widok przedstawiający klasyfikację drużyn z podium dla najlepszych zespołów.

#### Podium zwycięzców

- **Top 3 drużyny** wyświetlane są w formie podium z wizualnym wyróżnieniem
- **1. miejsce**: Złoty kolor, ikona pucharu, największy rozmiar
- **2. miejsce**: Główny kolor aplikacji, średni rozmiar
- **3. miejsce**: Akcentowy kolor, najmniejszy rozmiar

#### Lista rankingowa

Pod podium wyświetlana jest pełna lista wszystkich drużyn:

- **Pozycja w rankingu** - numer miejsca drużyny
- **Nazwa drużyny** - pełna nazwa zespołu
- **Końcowy wynik** - łączna liczba punktów z jednostką "pkt"
- **Paginacja** - początkowo 3 drużyny (podium), następnie po 10 na stronę
- **Pozycja drużyny użytkownika** - widoczna dla lidera i członka drużyny przed listą wszystkich drużyn

#### Szczegóły drużyny

Kliknięcie przycisku **"więcej"** (trzy kropki) przy drużynie otwiera szczegółowy widok:

**Dostępne informacje:**
- **Końcowy wynik** - suma wszystkich punktów
- **Wynik punktowy** - punkty z zebranych kategorii punktowych
- **Wynik plecaka** - wartość przedmiotów w plecaku drużyny
- **Ostatni zebrany punkt** - znacznik czasu ostatniej aktywności
- **Lista zebranych punktów** z ikonami, nazwami i wartościami
- **Opcja "Pokaż na mapie"** dla każdego punktu

### Zakładka "Progress gry"

Widok ogólnego postępu w grze z wizualizacją ukończenia.

#### Wskaźnik postępu

- **Okrągły pasek postępu** pokazujący procent ukończenia gry
- **Duża liczba procentowa** w centrum
- **Tekst opisowy** "Gra ukończona w X%"

#### Postęp według kategorii

- **Siatka kategorii punktowych** (4 kolumny)
- **Kolorowe ikony** kategorii z niestandardowymi kolorami
- **Postęp** wyświetlany jako procent lub ułamek (X/Y)
- **Tooltip** z nazwą kategorii przy najechaniu

## Obliczanie wyników

### System punktowy

**Końcowy wynik = Wynik punktowy + Wynik plecaka**

- **Wynik punktowy**: Suma wartości wszystkich zebranych punktów z kategorii punktowych
- **Wynik plecaka**: Wartość przedmiotów znajdujących się w plecaku drużyny

### Sortowanie i ranking

**Główne kryterium**: Drużyny sortowane według końcowego wyniku (najwyższy pierwszy)

**Rozstrzyganie remisów**: Gdy drużyny mają równy wynik końcowy:
- Porównywany jest czas zebrania ostatniego punktu
- Wyżej klasyfikowana jest drużyna, która wcześniej osiągnęła ten sam wynik

## Uprawnienia i ograniczenia

### Role użytkowników

- **Administrator/Twórca wydarzenia**: Może przeglądać szczegóły wszystkich drużyn
- **Członkowie drużyny**: Mogą przeglądać szczegółowe wyniki tylko swojej drużyny
- **Pozostałe drużyny**: Widzą ograniczone informacje o innych drużynach (sam wynik całkowity i pozycję w rankingu)

## Aktualizacja w czasie rzeczywistym

Tabela wyników aktualizuje się automatycznie co minutę:
- **Nowe zebrane punkty** są widoczne w rankingu po aktualizacji
- **Zmiany w plecaku** wpływają na wynik końcowy
- **Postęp gry** jest przeliczany dynamicznie
- **Ranking** jest automatycznie sortowany po każdej zmianie wyniku
