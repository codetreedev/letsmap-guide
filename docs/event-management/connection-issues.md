# Problemy związane z brakiem internetu lub lokalizacji GPS
Autor: **Emil Twardzik**

Podczas korzystania z aplikacji Let's Map, niektórzy użytkownicy mogą zauważyć, że ich lokalizacja na mapie nie aktualizuje się lub punkty zbierane na bazie lokalizacji użytkownika nie mogą być zebrane w danym momencie. Ten przewodnik wyjaśnia przyczyny tych problemów oraz przedstawia rozwiązania.

## Dlaczego lokalizacja może być niedokładna?

### 1. Warunki środowiskowe

Dokładność GPS zależy od wielu czynników zewnętrznych:

- **Zabudowania i budynki** – sygnał GPS odbija się od ścian budynków, co powoduje błędy w pomiarze (tzw. efekt multipath)
- **Gęsta roślinność** – drzewa i gęste zarośla osłabiają sygnał satelitarny
- **Wnętrza budynków** – GPS praktycznie nie działa w pomieszczeniach zamkniętych
- **Warunki pogodowe** – gęste chmury i burze mogą wpływać na dokładność
- **Wąwozy miejskie** – w wąskich ulicach między wysokimi budynkami sygnał jest mocno zniekształcony

### 2. Rodzaj urządzenia mobilnego i system operacyjny

**Aplikacja działa sprawniej na urządzeniach z iOS**. Problem może występować ze względu na brak udzielonych dostępów do systemu operacyjnego:

#### Na urządzeniach Android:
- Aplikacja nie ma przyznanych uprawnień do lokalizacji
- Lokalizacja jest włączona tylko podczas korzystania z aplikacji zamiast "cały czas"
- Oszczędzanie energii ogranicza dokładność GPS
- Tryb lokalizacji ustawiony na "oszczędzanie baterii" zamiast "wysoka dokładność"

#### Na urządzeniach iOS:
- Aplikacja nie ma przyznanych uprawnień do lokalizacji
- Lokalizacja ustawiona na "Podczas korzystania z aplikacji" zamiast "Zawsze"
- Wyłączona opcja "Dokładna lokalizacja"
- Ograniczenia związane z trybem niskiego zużycia energii

## Jakie funkcjonalności mogą nie działać w wyniku problemów z GPS lub internetem?

### 1. Zbieranie punktów za pomocą lokalizacji użytkownika

W aplikacji istnieje rodzaj punktu, który jest naniesiony tylko wirtualnie i zbierany jest za pomocą lokalizacji. W przypadku problemów z GPS możliwa będzie konieczność zebrania punktu jeszcze raz.

### 2. Aktualizacja i dokładność mapy

Zarówno w przypadku braku internetu, jak i problemów z GPS, mapa będąca centralnym elementem wydarzenia może nie działać poprawnie. Charakteryzuje się to:

- Brakiem przemieszczania się kółka użytkownika
- Zmianą koloru kółka na szary
- Zmniejszeniem się promienia oznaczającego dokładność GPS

### 3. Logowanie do aplikacji

Zalogowanie się do aplikacji jest niemożliwe bez dostępu do internetu.
