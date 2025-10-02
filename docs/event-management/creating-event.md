# Tworzenie wydarzenia
Autor: **Dominik Betka**

Strona dotyczący tworzenia wydarzeń w aplikacji - platformie do organizowania dynamicznych gier miejskich i terenowych takich jak poszukiwanie skarbów, rajdy czy aktywności terenowe.

## Przegląd

Tworzenie wydarzenia w Let's Map to prosty proces, który pozwala na zorganizowanie gier dla uczestników z możliwością konfiguracji zaawansowanych ustawień gry. Każde wydarzenie ma unikalne klucze dostępu dla różnych ról uczestników.

## Wymagania wstępne

Przed rozpoczęciem tworzenia wydarzenia upewnij się, że:
- Masz zainstalowaną aplikację Let's Map
- Posiadasz konto użytkownika w aplikacji
- Znasz lokalizację, gdzie będzie odbywać się wydarzenie

## Proces tworzenia wydarzenia

### 1. Rozpoczęcie tworzenia

Aby utworzyć nowe wydarzenie:
1. Otwórz aplikację Let's Map
2. Przejdź do listy wydarzeń
3. Wybierz opcję "Utwórz wydarzenie"

### 2. Podstawowe informacje o wydarzeniu

#### Wymagane pola:

**Nazwa wydarzenia**
- Długość: 3-45 znaków
- Wymaga podania unikalnej nazwy identyfikującej wydarzenie
- Przykład: "Rajd po Starym Mieście", "Poszukiwanie skarbów 2024"

**Data rozpoczęcia**
- Wybierz datę i godzinę rozpoczęcia wydarzenia
- Format: data i czas
- Musi być datą przyszłą

**Data zakończenia**
- Wybierz datę i godzinę zakończenia wydarzenia
- Musi być późniejsza niż data rozpoczęcia
- Format: data i czas

**Adres wydarzenia**
- Długość: 3-45 znaków
- Podaj główny adres lub lokalizację wydarzenia
- Przykład: "Rynek Główny 1, Kraków", "Park Łazienkowski, Warszawa"

**Nick organizatora**
- Długość: 1-45 znaków
- Nazwa wyświetlana jako organizator wydarzenia
- Widoczna dla wszystkich uczestników

### 3. Konfiguracja mapy

#### Obszar wydarzenia
- Użyj interaktywnej mapy do wyboru obszaru wydarzenia
- Mapa domyślnie wycentrowana na Polsce (52.69°N, 19.21°E)
- Możliwość przesuwania i zmiany pozycji poprzez interakcję z mapą
- Zoom można dostosować do wielkości obszaru wydarzenia
- Uczestnicy, którzy pierwszy raz otworzą wydarzenie zobaczą mapę pokazującą wybrany obszar

### 4. Zaawansowane ustawienia gry

Opcjonalna konfiguracja zasad gry dla zaawansowanych organizatorów:

#### Ustawienia mapy użytkownika:

**Dostępność geolokalizacji**
- Dostępna: Uczestnicy mogą używać GPS
- Zabroniona: Geolokalizacja wyłączona dla uczestników

**Wygląd zebranych punktów**
- Częściowo widoczne: Zebrane punkty są pokazane na mapie jako półprzeźroczyste
- Ukryte: Zebrane punkty są całkowicie ukryte

#### Ustawienia funkcji użytkownika:

**Zbieranie punktów przez geolokalizację**
- Jako domyślne: Standardowy sposób zbierania i tworzenia punktów
- Opcjonalne: Punkty można zbierać zarówno przez GPS, jak i za pomocą hasła do zebrania punktu
- Zabronione: Formularz tworzenia punktu ukrywa opcje zbierania punktów przez GPS

**Dokładność do zebrania geolokalizacją**
- Otwarta przestrzeń: Wymagana dokładność do 10 m do zebrania punktu GPS
- Teren miejski / leśny: (Domyślna) Wymagana dokładność do 20 m do zbierania punktu GPS
- Teren z przewyższeniami: Wymagana dokładność do 30 m do zbierania punktu GPS

**Dostępność plecaka**
- Dostępny: Uczestnicy i organizatorzy mogą korzystać z plecaka i przedmiotów w aplikacji
- Zabroniony: Funkcja plecaka i przedmiotów jest wyłączona – po naciśnięciu ikony plecaka pojawia się komunikat, że funkcja jest niedostępna

**Dostępność wieloosobowych drużyn**
- Dostępne: Możliwość zapraszania członków drużyny
- Zabronione: Liderzy drużyn nie mogą zapraszać członków

**Dostępność sklepu**
- Dostępny: Uczestnicy i organizatorzy mogą korzystać z funkcji sklepu
- Zabroniony: Funkcjonalność sklepu jest wyłączona – po naciśnięciu ikony sklepu pojawia się komunikat, że funkcja jest niedostępna

**Dostępność tablicy wyników**
- Dostępna: Uczestnicy i organizatorzy widzą ranking
- Zabroniona: Tablica wyników ukryta dla wszystkich – po naciśnięciu ikony rankingu pojawia się komunikat, że funkcja jest niedostępna

### 5. Czas odświeżania mapy

- **Odświeżanie co**: 60 sekund
- Określa jak często mapa jest aktualizowana dla uczestników i organizatorów podczas wydarzenia
- Mapa jest dodatkowo aktualizowana przy każdym otwarciu aplikacji i konkretnych akcjach (np. zebranie punktu, wysłanie aktualności, zakupienie oferty ze sklepu itp.)

## Finalizowanie wydarzenia

#### Walidacja danych

Przed zapisaniem sprawdzana jest poprawność:
- Wszystkie wymagane pola są wypełnione
- Nazwa wydarzenia ma odpowiednią długość
- Data zakończenia jest późniejsza niż rozpoczęcia
- Adres ma odpowiednią długość
- Nick organizatora jest poprawny

#### Zapisanie wydarzenia

Po wypełnieniu wszystkich wymaganych pól:
1. Kliknij "Zapisz"
2. System waliduje wprowadzone dane
3. W przypadku błędów, popraw wskazane pola
4. Po pomyślnym utworzeniu otrzymasz potwierdzenie

## System kluczy dostępu

[Dowiedz się więcej o systemie kluczy dostępu i zarządzaniu uczestnikami](inviting-participants-organizers.md)

## Rozwiązywanie problemów

### Typowe problemy:

**Błąd walidacji**
- Sprawdź czy wszystkie wymagane pola są wypełnione
- Upewnij się, że długość tekstu mieści się w limitach
- Zweryfikuj poprawność dat

**Problemy z mapą**
- Upewnij się, że masz połączenie z internetem
- Spróbuj odświeżyć pozycję na mapie
- Sprawdź czy geolokalizacja jest włączona

**Błędy zapisu**
- Sprawdź połączenie z internetem
- Zweryfikuj poprawność wszystkich danych
- Spróbuj ponownie za chwilę

## Wskazówki i najlepsze praktyki

### Planowanie wydarzenia:
- Wybierz opisową i unikalną nazwę
- Ustaw realistyczne ramy czasowe
- Przemyśl lokalizację względem dostępności dla uczestników
- Skonfiguruj ustawienia odpowiednio do typu gry

### Ustawienia gry:
- Dostosuj ustawienia do charakteru wydarzenia
- Rozważ ograniczenia techniczne uczestników
- Przetestuj ustawienia przed głównym wydarzeniem
- Załóż dodatkowe konto i dołącz do wydarzenia jako uczestnik, aby przetestować jego działanie (potem możesz je zresetować i usunąć swoje testowe konto)

## Następne kroki

Po utworzeniu wydarzenia możesz:
1. [Zarządzaj punktami na mapie](event-management/managing-points.md)
2. [Konfiguruj kategorie punktów](event-management/managing-point-categories.md)
3. [Zapraszaj uczestników i organizatorów](event-management/inviting-participants-organizers.md)
4. [Zarządzaj drużynami](event-management/managing-teams.md)
5. [Monitoruj postępy uczestników](event-management/scoreboard.md)
