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

#### Ustawienia mapy użytkownika

**Ustawienia geolokalizacji**
- Dostępna: Uczestnicy mogą używać GPS i widzą swoją pozycję na mapie
- Zabroniona: Geolokalizacja wyłączona dla uczestników

**Wygląd zebranych punktów dla drużyny**
- Częściowo przeźroczysty: Zebrane punkty są pokazane na mapie jako przyciemnione
- Ukryty: Zebrane punkty są całkowicie ukryte na mapie

**Tryb ciemności na mapie** *(eksperymentalne)*
- Włączony: Mapa jest pokryta ciemnością — uczestnicy widzą tylko obszar wokół swojej pozycji GPS. Jako administrator możesz przetestować ten tryb zmieniając ustawienia mapy w prawym górnym rogu widoku mapy
- Wyłączony: Mapa jest w pełni widoczna

**Zasięg widoczności (dokładna lokalizacja)** *(eksperymentalne, widoczne gdy tryb ciemności włączony)*
- Określa promień widocznego obszaru gdy GPS ma wysoką dokładność: 10 / 20 / 30 / 50 / 100 / 300 / 500 / 1000 metrów
- Domyślnie: 30 metrów

**Zasięg widoczności (niedokładna lokalizacja)** *(eksperymentalne, widoczne gdy tryb ciemności włączony)*
- Określa promień widocznego obszaru gdy GPS ma niską dokładność: 5 / 10 / 20 / 30 / 50 metrów
- Domyślnie: 5 metrów

**Radar najbliższego punktu** *(eksperymentalne, widoczne gdy tryb ciemności włączony)*
- Włączony: Na krawędzi widocznego obszaru pojawia się wskaźnik kierunku i odległości do najbliższego niezebranego punktu
- Wyłączony: Radar jest ukryty

**Liczba radarów** *(eksperymentalne, widoczne gdy radar włączony)*
- Liczba punktów jednocześnie pokazywanych na radarze: 1 / 2 / 3 / 4 / 5

**Podgląd kategorii punktu na radarze** *(eksperymentalne, widoczne gdy radar włączony)*
- Włączony: Obok wskaźnika dystansu wyświetlana jest miniaturka punktu (kształt i kolor kategorii)
- Wyłączony: Na radarze wyświetlany jest tylko dystans

**Odkrywanie mapy (mgła wojny)** *(eksperymentalne, widoczne gdy tryb ciemności włączony)*
- Włączone: Odwiedzone obszary pozostają widoczne na mapie. Uwaga: aktualnie odkryta mapa nie jest synchronizowana między urządzeniami
- Wyłączone: Widoczny tylko obszar wokół bieżącej pozycji

**Czas wygasania odkrytych kafelków** *(eksperymentalne, widoczne gdy odkrywanie mapy włączone)*
- Określa po jakim czasie odkryte obszary znikają z mapy: 1 min / 3 min / 5 min / 10 min / 15 min / 30 min / 1 godzina / nie czyść (do wyczerpania limitu 10 000 lokalizacji)
- Domyślnie: 5 minut

#### Funkcje wydarzenia

**Zbieranie punktów przez geolokalizację**
- Domyślnie: Punkty można zbierać przez GPS — domyślna opcja przy tworzeniu punktu
- Opcjonalnie: Punkty można zbierać przez GPS, jednak domyślna opcja tworzenia to hasło
- Zabronione: Zbieranie punktów przez GPS jest wyłączone

**Dokładność do zebrania geolokalizacją**
- Otwarta przestrzeń: Wymagana dokładność do 10 m
- Teren miejski / leśny: Wymagana dokładność do 20 m
- Teren z przewyższeniami: Wymagana dokładność do 30 m

**Dostępność plecaka**
- Dostępny: Uczestnicy mogą korzystać z plecaka i przedmiotów
- Wyłączony: Funkcja plecaka jest niedostępna

**Dostępność wieloosobowych drużyn**
- Dostępne: Liderzy mogą zapraszać członków do swojej drużyny
- Wyłączone: Liderzy nie mogą zapraszać członków

**Dostępność sklepu**
- Dostępny: Uczestnicy mogą korzystać ze sklepu
- Wyłączony: Sklep jest niedostępny

**Dostępność tabeli wyników**
- Dostępna: Uczestnicy i organizatorzy widzą ranking
- Wyłączona: Tablica wyników jest ukryta dla wszystkich

#### Funkcje organizatora

**Śledzenie GPS drużyn**
- Włączone: Pozycje GPS liderów drużyn są zbierane co 60 sekund i wyświetlane na mapie dla organizatorów
- Wyłączone: Śledzenie GPS drużyn jest wyłączone
- Śledzenie uczestników odbywa się wyłącznie w trakcie trwania wydarzenia

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
