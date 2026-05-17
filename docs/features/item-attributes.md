# Atrybuty przedmiotów
Autor: **Paweł Bednarczyk**

Atrybuty przedmiotów to dodatkowe efekty, które można przypisać do przedmiotów w plecaku drużyny. Dzięki nim przedmioty mogą nie tylko dawać punkty, ale też aktywnie wpływać na rozgrywkę — zmieniać zasięg GPS, poszerzać widoczność na mapie czy modyfikować punktację za wybrane kategorie.

## Zarządzanie atrybutami (administrator)

Atrybuty są częścią formularza tworzenia i edycji przedmiotu. W sekcji **Atrybuty** administrator może:

- Dodać jeden lub więcej atrybutów do przedmiotu przyciskiem **Dodaj atrybut**
- Edytować istniejący atrybut klikając na niego
- Usunąć atrybut z przedmiotu

Każdy atrybut ma swój typ i zestaw parametrów do uzupełnienia. Efekt atrybutu jest oznaczony kolorem:
- **Zielony** — efekt pozytywny (zwiększenie możliwości)
- **Czerwony** — efekt negatywny (zmniejszenie możliwości)
- **Szary** — efekt neutralny

## Dostępne atrybuty

### Zasięg zbierania GPS

Modyfikuje odległość wymaganą do zebrania punktu przez GPS.

**Parametr**: Bonus (metry) — wartość dodatnia zwiększa zasięg, ujemna go zmniejsza.

**Ograniczenia**:
- Ostateczny zasięg zawsze mieści się w zakresie **10–60 metrów**, niezależnie od sumy bonusów
- Na przedmiot można dodać **tylko jeden** atrybut tego typu
- Posiadając wiele sztuk przedmiotu, efekt jest mnożony przez ilość

**Przykład**: Przedmiot z bonusem `+15 m`, posiadany w 2 egzemplarzach, daje łącznie `+30 m` zasięgu.

---

### Promień widoczności

Modyfikuje promień odkrytego obszaru na mapie w trybie ciemności (Darkness Mode).

**Parametr**: Bonus (metry) — wartość dodatnia zwiększa widoczny obszar, ujemna go zmniejsza.

**Ograniczenia**:
- Na przedmiot można dodać **tylko jeden** atrybut tego typu
- Posiadając wiele sztuk przedmiotu, efekt jest mnożony przez ilość

**Przykład**: Przedmiot z bonusem `+20 m` sprawia, że drużyna widzi szerszy krąg mapy wokół swojej lokalizacji.

---

### Punkty zwycięstwa za kategorie

Przyznaje dodatkowe punkty zwycięstwa za każdy zebrany punkt należący do wybranej kategorii.

**Parametry**:
- **Kategoria** — kategoria punktów, której dotyczy atrybut
- **Punkty zwycięstwa za zebranie** — liczba dodatkowych punktów za każdy zebrany punkt tej kategorii (może być ujemna)

**Ograniczenia**:
- Dla jednej kategorii można dodać **tylko jeden** atrybut tego typu na przedmiot
- Można dodać wiele atrybutów tego samego typu, ale każdy musi dotyczyć **innej kategorii**
- Posiadając wiele sztuk przedmiotu, efekt jest mnożony przez ilość

**Przykład**: Przedmiot z parametrem `+5 pts` dla kategorii "Zagadki", posiadany w 3 egzemplarzach, daje `+15 pts` za każdy zebrany punkt z tej kategorii.

---

### Bonus za próg kategorii

Przyznaje jednorazowy bonus punktów zwycięstwa za każde zebrane X punktów z wybranej kategorii.

**Parametry**:
- **Kategoria** — kategoria punktów, której dotyczy atrybut
- **Bonus punktów zwycięstwa** — liczba punktów przyznawana za osiągnięcie progu
- **Co ile zebranych** — co ile zebranych punktów z tej kategorii bonus jest przyznawany

**Ograniczenia**:
- Dla jednej kategorii można dodać **tylko jeden** atrybut tego typu na przedmiot
- Można dodać wiele atrybutów tego samego typu, ale każdy musi dotyczyć **innej kategorii**
- Posiadając wiele sztuk przedmiotu, efekt jest mnożony przez ilość

**Przykład**: Atrybut z bonusem `+50 pts` i progiem `5` dla kategorii "Tajne" oznacza, że za każde 5 zebranych punktów tej kategorii drużyna dostaje +50 punktów. Przy 12 zebranych punktach bonus wynosi `+100 pts` (2 × 50, bo `floor(12/5) = 2`).
