# Zarządzanie punktami
Autor: **Paweł Bednarczyk**

Punkty rozmieszczane na mapie są najważniejszymi elementami aplikacji, dlatego chcemy udostępnić dużą ilość możliwości konfiguracji a z drugiej strony zachować prostotę, żeby początkujący administratorzy nie zatonęli w morzu opcji.

## Przegląd

Formularz tworzenia punktów składa się z sześciu głównych sekcji, które pozwalają na pełną konfigurację punktów w wydarzeniu.

## Struktura formularza tworzenia punktów

### 1. Informacje ogólne

**Podstawowe dane punktu**:
- **Nazwa punktu**: Nazwa punktu widoczna dla uczestników
- **Opis punktu**: Opis punktu widoczny dla użytkowników, można zawrzeć w nim fabularną historię, zagadkę lub podpowiedzi gdzie dokładnie szukać karteczki z punktem

### 2. Typ punktu

**Konfiguracja zachowania punktu**:
- **Typ zbieralności punktu**: Punkty mogą być możliwe do zebrania tylko przez jedną drużynę lub dostępne do zebrania przez wszystkie drużyny
- **Kategoria punktu**: Kategorie punktów tworzone są w osobnym formularzu i przy tworzeniu punktu należy go jedynie przypisać do odpowiedniej kategorii, określa ona wygląd punktu na mapie, jego wartość punktową a także opis kategorii jest dostępny przy każdym punkcie, który do niej należy

### 3. Zadanie

**Jak drużyna zbiera punkt**:
- **Skąd drużyna może zebrać punkt**: **Z dowolnego miejsca** lub **Tylko w pobliżu punktu** (przez GPS). Opcja „Tylko w pobliżu punktu” jest dostępna tylko wtedy, gdy ustawienia wydarzenia pozwalają zbierać punkty poprzez GPS
- **Co musi zrobić drużyna**: Domyślnie jest to **Hasło** — jeśli zostawisz je puste, zostanie wygenerowane automatycznie. Zamiast hasła możesz wybrać inne zadanie: liczbę, wybór z listy, kolejność, luki w zdaniu lub kilka zadań naraz. Hasło może też być kodem wpisywanym w kratki jak w kłódce. Przy punkcie „Tylko w pobliżu punktu” możesz wybrać **Nic: zbiera dotknięciem w pobliżu punktu** — drużyna musi jedynie dotrzeć na miejsce
- **Ustawienia zaawansowane**: Limit prób, kara za błędną odpowiedź, przerwa między próbami i płatne podpowiedzi

Szczegóły w opisie funkcji [Zadania punktów](features/point-challenges.md#zadania-punktów).

### 4. Ustawienia mapy

**Lokalizacja punktu**:
- Określenie miejsca, w którym znajduje się dany punkt na mapie

### 5. Typ widoczności punktu

**Kontrola dostępności punktu**:
- **Typ widoczności punktu**: Jest to nadrzędna cecha, która kontroluje dalsze opcje ustawienia
  - **Punkt widoczny**: Bazowy punkt jest zawsze widoczny przez cały okres trwania wydarzenia
  - **Punkt czasowy**: Punkt widoczny jest przez wybrany przez administratora przedział czasowy
  - **Punkt ukryty**: Punkt widoczny jest tylko dla drużyn, które spełniają odpowiednie kryteria np. posiadają odpowiedni przedmiot (mapę)
  - **Punkt ukryty czasowy**: Połączenie punktów czasowych i ukrytych, punkt jest widoczny w przedziale czasowym tylko dla drużyn, które posiadają odpowiedni przedmiot

### 6. Akcje po zebraniu punktu

**Nagrody i komunikaty**:
- **Wiadomość po zebraniu punktu**: Komunikat wyświetlany drużynie po zebraniu punktu
- **Przedmioty**: Nagrody jakie dostanie drużyna zbierająca punkt

## Zaawansowane ustawienia punktu

### Ustawienia zaawansowane zadania
W zaawansowanych ustawieniach zadania możesz dodatkowo określić:
- **Limit prób**: Po wykorzystaniu wszystkich prób drużyna nie może już odpowiadać, dopóki organizator nie odblokuje punktu
- **Przerwa**: Czas w sekundach, jaki drużyna musi odczekać po błędnej odpowiedzi
- **Kara**: Liczba punktów zwycięstwa odejmowana drużynie za każdą błędną odpowiedź
- **Komunikat po błędzie**: Własna wiadomość wyświetlana po błędnej odpowiedzi
- **Podpowiedzi**: Drużyna odkrywa je po kolei. Każda podpowiedź może mieć koszt w punktach zwycięstwa odejmowany od wyniku drużyny – przed odkryciem drużyna widzi, ile zapłaci
- **Porównywanie odpowiedzi**: Możesz pominąć polskie znaki (ą = a, ł = l), aby odpowiedź bez nich też była uznana

W przypadku zadania „Kilka zadań” limit prób, kara i podpowiedzi dotyczą całego punktu.

### Ustalanie przedziałów czasowych
Ustalanie przedziałów czasowych punktów polega na podaniu godziny pojawienia i zniknięcia punktu. Można to zrobić na dwa sposoby:

#### Data i godzina (konkretny czas)
- **Zastosowanie**: Ustawienie na konkretną godzinę
- **Zalety**: Najprostsza opcja
- **Wady**: Powoduje problemy jeśli czas wydarzenia miałby ulec zmianie

#### Ustawienie relatywne
Umożliwia ustawienie 6 markerów czasu i dodanie różnicy od nich w minutach:  
**Dostępne markery czasu**:
- **Przed startem wydarzenia**: Rzadko używane, ale może posłużyć jako oznaczenie punktu startowego jeśli użytkownicy zarejestrują się do aplikacji przed przybyciem na miejsce
- **Start wydarzenia**: Domyślna opcja dla pojawienia się punktu
- **Po starcie wydarzenia**: Można ustawić czas, kiedy punkt się pojawi relatywnie względem czasu rozpoczęcia wydarzenia (godzinę po rozpoczęciu np.)
- **Przed końcem wydarzenia**: Można ustawić czas, kiedy punkt zniknie relatywnie względem czasu zakończenia wydarzenia (godzinę przed zakończeniem np.)
- **Koniec wydarzenia**: Domyślna opcja dla wygaśnięcia punktu
- **Po końcu wydarzenia**: Rzadko używane, ale może posłużyć do ukrycia miejsca końcowej zbiórki (jako dodatkowe zadanie)
