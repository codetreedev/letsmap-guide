# Gry publiczne dla autorów

Gra publiczna to gotowa gra, którą każdy zalogowany użytkownik znajdzie w aplikacji, w katalogu **Gry publiczne**, i do której dołączy sam, bez kodu zaproszenia. Nikt nie prowadzi jej na żywo: autor przygotowuje ją wcześniej, a każda drużyna gra we własnym tempie, kiedy chce. Gra może być dostępna miesiącami, a kolejne drużyny dołączają w dowolnym momencie.

Ta strona jest dla autorów, czyli osób, które chcą pokazać swoje wydarzenie innym. Jak grać w gry publiczne, opisuje strona [Gry publiczne](features/public-events.md#gry-publiczne).

## Czym gra publiczna różni się od zwykłego wydarzenia?

| | Zwykłe wydarzenie | Gra publiczna |
|---|---|---|
| **Dołączanie** | Kodem zaproszenia od organizatora (także kodem QR) | Z katalogu **Gry publiczne**, bez kodu. Każdy dołączający zakłada własną drużynę i zostaje jej liderem |
| **Czas gry** | Wspólny dla wszystkich: od początku do końca wydarzenia | Własny dla każdej drużyny: liczy się od chwili dołączenia i nie ma limitu |
| **Inne drużyny** | Widoczne zgodnie z ustawieniami wydarzenia | Niewidoczne. Każda drużyna widzi tylko siebie |
| **Tabela wyników** | Zgodnie z ustawieniami wydarzenia | Brak. Drużyny grają w różnym czasie, więc nie ma ich jak porównać |
| **Organizator** | Prowadzi grę na żywo | Nikt nie prowadzi gry. Wszystko jest w opisie gry i w opisach punktów |
| **Zmiany w grze** | Organizator edytuje wydarzenie | Autor wysyła aktualizację, którą sprawdza zespół Let's Map |
| **Gra od nowa** | Po zresetowaniu wydarzenia przez organizatora | Gracz sam zaczyna nowe podejście, z nową drużyną i pustymi postępami |

Gry publiczne są bezpłatne dla graczy.

## Jak wydarzenie staje się grą publiczną?

Grą publiczną może zostać każde Twoje wydarzenie:

1. Przygotowujesz wydarzenie i zgłaszasz je do katalogu.
2. Zespół Let's Map sprawdza zgłoszenie.
3. Po zatwierdzeniu do katalogu trafia **kopia** wydarzenia. Twoje wydarzenie zostaje u Ciebie jako wersja robocza: możesz je dalej zmieniać, a zmiany przenosić do gry aktualizacją.
4. W opublikowanej grze masz rolę obserwatora i śledzisz jej statystyki.

Zgłoszenia wysyłasz w [panelu organizatora](admin-panel.md#panel-organizatora).

## Przygotuj wydarzenie

Gra publiczna nie przyjmie elementów, które działają tylko przy wspólnym czasie gry albo wyczerpują się po pierwszej drużynie. Przed zgłoszeniem popraw:

| Co blokuje zgłoszenie | Dlaczego | Jak poprawić |
|---|---|---|
| Okno czasowe punktu lub oferty ustawione na **konkretną datę** | Drużyny grają w odstępie miesięcy | Usuń okno czasowe |
| Okno czasowe liczone **od początku lub końca wydarzenia** | Drużyny zaczynają w różnym czasie | Usuń okno czasowe |
| **Punkt jednorazowy** | Zebrałaby go tylko pierwsza drużyna | Zmień rodzaj punktu |
| **Nagroda jednorazowa** punktu | Dostałaby ją tylko pierwsza drużyna, która zbierze punkt | Ustaw nagrodę dla każdej drużyny |
| Oferta z **pulą wspólną dla wszystkich drużyn** | Wyczerpałaby ją pierwsza drużyna | Usuń limit puli w ofercie |

Formularz zgłoszenia sam pokaże listę elementów do poprawienia, więc nie musisz szukać ich ręcznie.

Warto też pamiętać, że:

- **nikt nie prowadzi gry na żywo.** Opisy punktów i [zadania](features/point-challenges.md#zadania-punktów) muszą wystarczyć graczom. Limit prób bez możliwości odblokowania punktu może zatrzymać drużynę na dobre,
- **tabela wyników i śledzenie drużyn są zawsze wyłączone**, niezależnie od ustawień Twojego wydarzenia,
- pozostałe ustawienia, w tym drużyny wieloosobowe i eksploracja mapy, gra przejmuje z Twojego wydarzenia,
- do gry trafiają kategorie, punkty, przedmioty, oferty i [aktualności](features/notifications.md#aktualności-w-wydarzeniu). Drużyny, uczestnicy i organizatorzy nie są kopiowani.

> **Wskazówka:** przejdź grę w [widoku gracza](features/player-view.md#widok-gracza), zanim ją zgłosisz. Zobaczysz ją tak, jak zobaczą ją gracze.

## Zgłoś wydarzenie

1. W panelu organizatora otwórz **Wydarzenia**.
2. W wierszu swojego wydarzenia otwórz menu **Więcej akcji** i wybierz **Zgłoś jako grę publiczną**. Opcję widzi tylko twórca wydarzenia.
3. Wypełnij formularz:

   | Pole | Co wpisać |
   |---|---|
   | **Nazwa gry** | Nazwa widoczna w katalogu. Domyślnie taka jak nazwa wydarzenia |
   | **W katalogu od / do** | Okres, w którym nowe drużyny mogą dołączać. Puste pola oznaczają: od teraz i bez końca |
   | **Krótki opis** | Tekst na karcie gry, do 300 znaków |
   | **Strona „O grze”** | Pełny opis: gdzie się gra, co zabrać, jak zacząć. Obok widzisz podgląd |
   | **Adres obrazka okładki** | Link do obrazka na karcie i stronie gry. Pole opcjonalne |
   | **Przewidywany czas gry jednej drużyny** | W godzinach. Gracze widzą go w katalogu jako podpowiedź |

4. Zaakceptuj regulamin i wybierz **Wyślij do sprawdzenia**.

Strona „O grze” przyjmuje prosty HTML: akapity (`p`), nagłówki (`h1`–`h6`), listy (`ul`, `ol`, `li`), pogrubienie (`strong`), kursywę (`em`) i linki (`a href`). Inne znaczniki zostaną pominięte.

## Co dzieje się po zgłoszeniu?

Zgłoszenie sprawdza zespół Let's Map. Jego stan widzisz w tym samym oknie, w którym je wysłano:

| Stan | Co oznacza |
|---|---|
| **Zgłoszenie czeka na sprawdzenie** | Możesz je jeszcze wycofać przyciskiem **Wycofaj zgłoszenie** |
| **Gra została opublikowana** | Kopia wydarzenia jest w katalogu |
| **Zgłoszenie zostało odrzucone** | Zobaczysz uwagi osoby sprawdzającej. Popraw wydarzenie i wybierz **Zgłoś ponownie** |

O decyzji dostaniesz też wiadomość e-mail. Jedno wydarzenie może mieć naraz jedno oczekujące zgłoszenie.

Po publikacji:

- właścicielem gry jest konto techniczne Let's Map, a Ty masz w niej rolę **obserwatora**: widzisz grę i jej statystyki, ale jej nie edytujesz,
- gracze widzą Cię jako autora gry, pod pseudonimem z Twojego wydarzenia,
- Twoje wydarzenie działa jak dotąd i możesz je dalej zmieniać.

## Statystyki Twojej gry

W panelu organizatora otwórz **Moje gry publiczne**. Zobaczysz listę swoich opublikowanych gier:

- **Status** – W katalogu, Poza oknem (nowe drużyny nie mogą dołączać), Ukryta lub Zarchiwizowana
- **Aktywne drużyny**, **Zakończone podejścia** i **Gracze**
- **Przewidywany czas**, **Ostatnie zebranie** punktu, daty publikacji i ostatniej aktualizacji

Kliknij nazwę gry, aby otworzyć **Podejścia drużyn**. To lista wszystkich drużyn, także tych, które już skończyły:

- start drużyny, liczba członków i zebranych punktów,
- **Czas gry** od startu do ostatniego zebranego punktu i jego stosunek do czasu przewidywanego,
- numer podejścia, gdy drużyna zaczynała od nowa.

Nad tabelą widzisz podsumowanie, w tym **medianę czasu gry** i liczbę podejść **ponad przewidywany czas**.

> **Wskazówka:** jeśli mediana czasu gry wyraźnie odbiega od czasu przewidywanego, popraw go w aktualizacji. Gracze planują wyjście według tej liczby.

## Aktualizacja opublikowanej gry

Opublikowanej gry nie edytujesz bezpośrednio. Zmieniasz swoje wydarzenie, a potem wysyłasz aktualizację:

1. Wprowadź zmiany w swoim wydarzeniu.
2. W panelu organizatora, w menu **Więcej akcji** w wierszu wydarzenia, otwórz to samo okno co przy zgłoszeniu i wybierz **Wyślij aktualizację**.
3. W razie potrzeby popraw okno katalogu i opis gry, a potem wybierz **Wyślij aktualizację do sprawdzenia**.

Aktualizację sprawdza zespół Let's Map, tak jak pierwsze zgłoszenie. Po zatwierdzeniu działa od razu, także dla drużyn, które właśnie grają.

**Drużyny zachowują postępy.** Zmienione elementy są aktualizowane w miejscu, nowe są dodawane, a usunięte znikają, chyba że któraś drużyna już w nie grała. Taki element zostaje w grze, dopóki ma czyjeś postępy.

Niektóre zmiany wpływają na drużyny, które już grają:

| Zmiana | Skutek dla drużyn |
|---|---|
| Wartość kategorii | Zmienia się wynik każdej drużyny, także za punkty zebrane wcześniej |
| Wartość przedmiotu | Zmieniają się wyniki drużyn, które go mają |
| Przeniesienie punktu do innej kategorii | Zmienia się jego wartość dla drużyn, które go zebrały |
| Położenie punktu | Drużyny idące do punktu zobaczą nowe miejsce po odświeżeniu |
| Zadanie punktu | Drużyny zachowują wykorzystane próby i kary |
| Sposób zbierania punktu | Punkt może dać się zebrać w inny sposób niż dotąd |

## Ukrycie i usunięcie gry

Grę z katalogu może ukryć lub usunąć zespół Let's Map:

- **ukryta** gra znika z katalogu i nie przyjmuje nowych drużyn, ale drużyny, które już grają, grają dalej,
- **usunięta** gra jest archiwizowana i znika dla graczy. Jej drużyny i statystyki zostają.

Jeśli chcesz wycofać swoją grę z katalogu, napisz do nas.

## Najczęstsze pytania autorów

**Nie widzę opcji „Zgłoś jako grę publiczną”.**
Opcja jest dostępna tylko dla twórcy wydarzenia i tylko w panelu organizatora.

**Formularz pokazuje listę „Popraw w wydarzeniu źródłowym”.**
To elementy, które blokują zgłoszenie. Popraw je zgodnie z tabelą w sekcji [Przygotuj wydarzenie](#przygotuj-wydarzenie) i wyślij zgłoszenie ponownie.

**Zmieniłem wydarzenie, a w grze nic się nie zmieniło.**
Gra jest osobną kopią. Zmiany trafią do niej dopiero po zatwierdzeniu aktualizacji.

**Czy mogę zgłosić to samo wydarzenie drugi raz?**
Nie. Opublikowane wydarzenie ma jedną grę, a kolejne zmiany wysyłasz jako aktualizacje.

**Czy mogę zaprosić do gry innych organizatorów?**
Nie. W grze publicznej nie ma organizatorów. Kodem zaproszenia można zaprosić tylko obserwatora albo członka drużyny.
