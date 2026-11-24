# Kody QR

Od wersji 7.0.0 kody QR przydają się w dwóch miejscach: przy **zbieraniu punktów** i przy **dołączaniu do wydarzenia**. Kod drukujesz albo pokazujesz na ekranie, a gracze skanują go aparatem.

## Zbieranie punktu kodem QR

Przy punkcie wieszasz wydrukowany kod. Drużyna otwiera punkt w aplikacji, wybiera **Zeskanuj kod QR** i kieruje aparat na kartkę. Gdy skan nie działa (słabe światło, zniszczona kartka), drużyna wpisuje znaki wydrukowane pod kodem.

Kod QR sprawdza się tam, gdzie GPS zawodzi, np. w budynku albo w gęstym lesie: drużyna musi dotrzeć do kartki, żeby zebrać punkt.

### Jak ustawić?

1. W formularzu punktu, w sekcji **Zadanie**, wybierz rodzaj **Kod QR**.
2. Kod tworzy się sam. Możesz go zmienić przyciskiem **Wygeneruj nowy kod**, ale wcześniej wydrukowana kartka tego punktu przestanie wtedy działać.
3. Kod QR może być też jednym z zadań w punkcie z rodzajem **Kilka zadań** (najwyżej jeden kod na punkt). Masz wtedy dwie możliwości:
   - kod jest **jednym z zadań**: drużyna musi go zeskanować, żeby zdobyć punkt,
   - kod **odsłania pozostałe zadania**: drużyna zobaczy pytania dopiero po zeskanowaniu. Uwaga: w tym trybie kod tylko odsłania zadania i nie jest dowodem, że drużyna była przy punkcie.

Więcej o rodzajach zadań: [Zadania punktów](features/point-challenges.md#rodzaje-zadań).

### Jak wydrukować?

Kody do wydruku przygotujesz w aplikacji (ekran **Lista punktów**) albo w [panelu organizatora](admin-panel.md#panel-organizatora) (lista punktów), przyciskiem **Generuj kody QR**. Możesz wygenerować kody wszystkich punktów albo tylko zaznaczonych. Punkty bez zadania „Kod QR” zostaną pominięte.

Do wyboru masz:

- **rozmiar kodu**: plakat (widać go z daleka), duże, średnie albo małe (do schowania w terenie, skan z bliska),
- **wygląd karty**: prosta, rozbudowana albo własna; na karcie mogą być m.in. nazwa wydarzenia, nazwa punktu, kod do wpisania, własny tekst i prośba o niezdejmowanie kartki do końca wydarzenia,
- **kolory**: kolorowa albo czarno-biała.

Gotowy plik PDF ma strony A4, na życzenie z liniami cięcia. Jeśli wolisz drukować po swojemu (np. naklejki), pobierz plik CSV i zrób z niego kody w Excelu albo w programie do etykiet.

> **Dobrze wiedzieć:** zduplikowany punkt dostaje nowy kod, więc jedna kartka nigdy nie zbierze dwóch punktów.

## Dołączanie do wydarzenia kodem QR

Każdy kod zaproszenia możesz pokazać jako kod QR. Otwórz **Udostępnij wydarzenie** (lider drużyny: **Zaproszenie do drużyny**), wybierz rolę i stuknij **Wyślij zaproszenie**. Kod QR możesz pokazać na ekranie, zapisać jako PDF albo wydrukować, np. na plakat przy starcie.

Gracz skanuje kod:

- **aparatem telefonu**: otwiera się dołączanie do wydarzenia w aplikacji albo w przeglądarce,
- **w aplikacji**: na ekranie **Dołącz do wydarzenia** wybiera skanowanie kodu QR zaproszenia.

### Szybkie dołączenie

Przy zaproszeniu dla lidera drużyny i do drużyny możesz włączyć **Szybkie dołączenie**. Kto zeskanuje taki kod, od razu gra:

- z kodu dla lidera powstaje nowa drużyna, a jej nazwę, kolor i nick gracza losujemy,
- z kodu do drużyny gracz trafia do tej drużyny, a nick losujemy,
- gracz podaje tylko adres e-mail.

To dobre rozwiązanie na duże wydarzenia, gdzie nie ma czasu na zakładanie drużyn przy stoliku.

> **Uwaga:** po zresetowaniu kodu zaproszenia przestają działać także wydrukowane kody QR z tym zaproszeniem.

Więcej o zaproszeniach: [Zapraszanie uczestników i organizatorów](event-management/inviting-participants-organizers.md#zapraszanie-uczestników-i-organizatorów).
