# Zadania punktów

Zadania zastępują dotychczasowe pole hasła i opcję zbierania przez GPS w formularzu punktu. Zamiast jednego hasła organizator może poprosić drużynę o podanie liczby, wpisanie kodu jak w kłódce, wybór odpowiedzi z listy, ułożenie elementów w kolejności, uzupełnienie luk w zdaniu albo rozwiązanie kilku zadań naraz. Do zadania można dodać limit prób, karę za błędną odpowiedź, przerwę między próbami oraz płatne podpowiedzi.

Sekcja **Zadanie** jest dostępna w formularzu punktu zarówno w aplikacji, jak i w panelu administratora. Nowy punkt zbierany z dowolnego miejsca domyślnie dostaje zadanie typu **Hasło** — jeśli zostawisz je puste, hasło zostanie wygenerowane automatycznie, tak jak dotychczas.

## Skąd drużyna może zebrać punkt?

Pierwsza decyzja w sekcji **Zadanie** formularza punktu to sposób dostępu do punktu:

| Opcja | Co musi zrobić drużyna | Jak działa |
|-------|------------------------|------------|
| **Z dowolnego miejsca** | zadanie (wymagane) | Drużyna odpowiada na zadanie z dowolnego miejsca, nie musi być przy punkcie |
| **Tylko w pobliżu punktu** | **Nic: zbiera dotknięciem w pobliżu punktu** | Drużyna zbiera punkt dotknięciem, gdy jest w zasięgu (zbieranie przez GPS) |
| **Tylko w pobliżu punktu** | zadanie | Pytanie jest widoczne i można na nie odpowiedzieć dopiero w zasięgu punktu — wcześniej drużyna widzi komunikat „Podejdź bliżej, aby zobaczyć pytanie” |

Opcja **Tylko w pobliżu punktu** jest dostępna, gdy ustawienia wydarzenia pozwalają zbierać punkty przez GPS. Ustawienie **Zbieranie punktów przez geolokalizację** decyduje też, która opcja jest domyślna dla nowego punktu: **Domyślnie** → „Tylko w pobliżu punktu”, **Opcjonalnie** → „Z dowolnego miejsca”.

Istniejące punkty zostały przeniesione automatycznie:
- punkt zbierany przez GPS → **Tylko w pobliżu punktu**, zbierany dotknięciem (bez hasła),
- punkt zbierany hasłem → **Z dowolnego miejsca** z zadaniem typu **Hasło** (dotychczasowe hasło jest odpowiedzią).

> Zasięg punktu wynika z ustawień GPS wydarzenia. Jeśli drużyna wyjdzie poza zasięg w trakcie odpowiadania na punkt „tylko w pobliżu”, wpisana odpowiedź zostaje — wystarczy wrócić.

## Rodzaje zadań

Pole **Co musi zrobić drużyna** określa rodzaj zadania:

| Rodzaj | Co robi drużyna | Co ustawia organizator |
|--------|-----------------|------------------------|
| **Hasło** | Wpisuje słowo, frazę albo kod | Główną odpowiedź i inne pisownie (łącznie do 20), dozwolone znaki oraz opcjonalnie kratki jak w kłódce. Puste hasło zostanie wygenerowane automatycznie |
| **Liczba** | Podaje liczbę | Dokładną wartość z tolerancją (±) albo przedział (od–do) |
| **Wybór z listy** | Wybiera jedną lub zaznacza kilka odpowiedzi z listy | Rodzaj wyboru (jednokrotny / wielokrotny), od 2 do 8 odpowiedzi i poprawne odpowiedzi |
| **Uzupełnij luki** | Uzupełnia brakujące słowa w zdaniu, wpisując je lub wybierając z puli słów | Zdanie z lukami, opcjonalnie pulę słów i słowa-zmyłki |
| **Kolejność** | Układa elementy we właściwej kolejności (przeciągając lub strzałkami) | Elementy w poprawnej kolejności — każda drużyna zobaczy je wymieszane |
| **Kilka zadań** | Rozwiązuje kilka zadań różnych rodzajów i wysyła odpowiedzi razem | Od 2 do 5 zadań, każde z własnym rodzajem i pytaniem |

Odpowiedź jest oceniana w całości — jest albo w pełni poprawna, albo błędna (nie ma punktów częściowych).

### Wskazówki do poszczególnych rodzajów

- **Hasło**
  - **Dozwolone znaki**: Dowolne, Tylko litery, Tylko cyfry lub Litery i cyfry. Drużyna widzi przy polu odpowiedzi, jakie znaki są dozwolone, a odpowiedź z innymi znakami nie jest liczona jako próba.
  - **Kod o stałej długości (kratki)** — drużyna wpisuje kod znak po znaku, jak w kłódce szyfrowej. Kod ma od 1 do 12 znaków, bez spacji i bez innych pisowni; liczba kratek wynika z długości odpowiedzi.
- **Wybór z listy** — przy jednokrotnym wyborze zaznacz dokładnie jedną poprawną odpowiedź, przy wielokrotnym co najmniej jedną; drużyna musi zaznaczyć wszystkie poprawne odpowiedzi — i tylko je. Odpowiedzi są zawsze wymieszane, inaczej dla każdej drużyny, więc kolejność wpisania nie ma znaczenia (możesz śmiało wpisać poprawną odpowiedź jako pierwszą).
- **Uzupełnij luki** — lukę zapisuje się w zdaniu jako `[[odpowiedź]]`, a inne poprawne odpowiedzi oddziela się znakiem `|`, np. `Stolicą Małopolski jest [[Kraków|Krakow]].` Można też zaznaczyć słowo i użyć przycisku **Zamień zaznaczenie w lukę**. Zdanie może mieć do 20 luk. Po włączeniu **puli słów** drużyna widzi do wyboru odpowiedzi z luk oraz do 10 słów-zmyłek.
- **Kilka zadań** — każde zadanie ma własne pytanie i może być dowolnego rodzaju (poza kolejnym „Kilka zadań”). Drużyna zdobywa punkt, gdy wszystkie odpowiedzi są poprawne. Limit prób, kara i podpowiedzi dotyczą całego punktu, nie pojedynczych zadań.

## Treść zadania

- **Pytanie (opcjonalne)** — obsługuje to samo formatowanie i multimedia co opis punktu. Przy punkcie zbieranym tylko w pobliżu drużyna zobaczy pytanie dopiero po podejściu.
- Pod formularzem widać podgląd **Tak zobaczy to drużyna**, a błędy do poprawienia są zebrane w sekcji **Popraw przed zapisaniem**.

## Ustawienia zaawansowane

Sekcja **Ustawienia zaawansowane** jest domyślnie zwinięta i otwiera się sama, jeśli punkt już korzysta z któregoś ustawienia.

- **Limit prób** (przełącznik **Ogranicz liczbę prób**) — od 1 do 999 prób. Po wyczerpaniu prób drużyna nie może już odpowiadać, dopóki organizator nie odblokuje punktu.
- **Przerwa (sekundy)** — czas, który musi minąć po błędnej odpowiedzi przed kolejną próbą (maksymalnie 24 godziny). 0 = bez przerwy.
- **Kara (PZ)** — liczba punktów odejmowana od wyniku drużyny za każdą błędną odpowiedź. 0 = bez kary.
- **Komunikat po błędzie** — własny tekst pokazywany drużynie po pomyłce.
- **Podpowiedzi** (przełącznik **Dodaj podpowiedzi**) — do 10 podpowiedzi, każda z własnym kosztem w PZ (może być darmowa). Szczegóły niżej.
- **Przy porównywaniu odpowiedzi pomijaj polskie znaki** (ą = a, ł = l) — domyślnie włączone. Wielkość liter i nadmiarowe spacje są pomijane zawsze.

> Odpowiedź w złym formacie (np. pusta) nie liczy się jako próba i nie nalicza kary.

## Podpowiedzi

- Drużyna odkrywa podpowiedzi **po kolei** — nie można pominąć pierwszej i od razu kupić drugiej.
- Przed odkryciem płatnej podpowiedzi aplikacja prosi o potwierdzenie („Podpowiedź odejmie drużynie N PZ. Pokazać ją?”).
- Koszt jest odejmowany od wyniku drużyny raz — nawet jeśli dwie osoby z drużyny klikną jednocześnie.
- Odkryte podpowiedzi widzą wszyscy członkowie drużyny, a odkryć je może ta sama osoba, która może odpowiadać (zob. [Kto odpowiada na zadanie?](#kto-odpowiada-na-zadanie)).
- Podpowiedzi nie można odkryć po zakończeniu wydarzenia, po zebraniu punktu ani gdy drużyna wykorzystała wszystkie próby.

> Nie zmieniaj kolejności ani nie usuwaj podpowiedzi w trakcie gry — drużyny, które już je odkryły, zobaczą teksty z nowych pozycji (zapłacony koszt się nie zmienia).

## Jak to wygląda dla drużyny?

Po otwarciu punktu drużyna widzi panel zadania z pytaniem, polem odpowiedzi oraz informacjami o zasadach: liczbie pozostałych prób (lub „Bez limitu prób”), wysokości kary i czasie do następnej próby.

- Po poprawnej odpowiedzi punkt zostaje zebrany jak dotychczas (nagrody, wiadomość po zebraniu itd.).
- Po błędnej odpowiedzi drużyna widzi komunikat organizatora albo „Błędna odpowiedź” (z wysokością kary, jeśli jest ustawiona).
- Po wykorzystaniu wszystkich prób drużyna widzi komunikat z prośbą o kontakt z organizatorem.
- Po zakończeniu wydarzenia nie można już odpowiadać na zadania.
- Starsze wersje aplikacji mogą nie obsługiwać nowych rodzajów zadań — wtedy drużyna zobaczy prośbę o aktualizację aplikacji.

### Kto odpowiada na zadanie?

Zależy to od ustawienia wydarzenia **Kto zbiera punkty**:

- **Tylko lider drużyny** (domyślnie, także w wydarzeniach utworzonych przed wprowadzeniem tego ustawienia) — odpowiedź wysyła i podpowiedzi odkrywa lider drużyny. Pozostali członkowie widzą zadanie w trybie podglądu („Tylko lider drużyny może wysłać odpowiedź”). Przy punkcie **Tylko w pobliżu punktu** pytanie pokazuje się dopiero liderowi, gdy podejdzie bliżej — pozostali członkowie widzą informację, że pytanie zobaczy lider przy punkcie.
- **Wszyscy członkowie drużyny** — odpowiedź wysyła i podpowiedzi odkrywa każdy członek drużyny; przy punkcie **Tylko w pobliżu punktu** pytanie zobaczy każdy członek, który podejdzie bliżej. Punkt zebrany przez jedną osobę liczy się całej drużynie, a limit prób, kary i odkryte podpowiedzi są wspólne dla całej drużyny.

## Wpływ na wynik

Kary za błędne odpowiedzi i koszty podpowiedzi są odejmowane od wyniku drużyny i widoczne osobno w szczegółach wyniku w tabeli wyników. W podglądzie historii wydarzenia w panelu administratora pojawia się pozycja „zadania: −N”.

## Narzędzia organizatora

### Zakładka „Zadanie” w szczegółach punktu (aplikacja)

Organizator, który może edytować punkt, widzi w szczegółach punktu na mapie dodatkową zakładkę **Zadanie** z podsumowaniem: rodzajem zadania, pytaniem, poprawnymi odpowiedziami i ustawieniami (limit prób, kara, przerwa, podpowiedzi). Dzięki temu w trakcie gry można szybko sprawdzić odpowiedź bez otwierania formularza edycji.

### Drużyny i próby (panel administratora)

W formularzu punktu z zadaniem panel **Drużyny i próby** pokazuje dla każdej drużyny: liczbę prób (i limit), naliczone kary, wykorzystane podpowiedzi, trwającą przerwę, ostatnie błędne odpowiedzi oraz status (zebrany / zablokowany).

Przycisk **Odblokuj** zeruje licznik prób drużyny i kończy przerwę. Naliczone wcześniej kary i koszty podpowiedzi **nie są zwracane**.

### Edycja zbiorcza

W edycji zbiorczej punktów opcja **Ustawienia zadania** ustawia jednocześnie limit prób, przerwę i karę we wszystkich zaznaczonych punktach z zadaniem. Punkty zbierane dotknięciem są pomijane. Tabela punktów ma też kolumny **Skąd zebrać** i **Zadanie**.

### Statystyki zadań

Widok **Zadania punktów** w menu panelu administratora pokazuje, jak drużyny radzą sobie z zadaniami — najtrudniejsze punkty są na górze. Dla każdego punktu widać m.in.: ile drużyn próbowało, ile odpowiedziało dobrze, liczbę odpowiedzi, odsetek błędnych, sumę kar i podpowiedzi oraz **najczęstsze błędne odpowiedzi** wraz z drużynami, które je podały. To dobre miejsce, żeby w trakcie gry wyłapać pytania za trudne albo niejednoznaczne (np. brakującą pisownię hasła). Widok jest dostępny dla twórcy, administratorów i obserwatorów wydarzenia.

### Historia wydarzenia

W podglądzie historii wydarzenia szczegóły punktu na mapie pokazują też rodzaj jego zadania.

## Kopiowanie i resetowanie wydarzenia

- Przy kopiowaniu wydarzenia zadania punktów są kopiowane razem z punktami.
- Duplikat punktu z hasłem dostaje nowe, wygenerowane hasło (inne pisownie nie są kopiowane).
- Reset wydarzenia czyści próby, kary i odkryte podpowiedzi wszystkich drużyn.

## Najczęstsze problemy

- **„Punkt zbierany z dowolnego miejsca wymaga zadania”** — opcja „Z dowolnego miejsca” wymaga ustawienia zadania. Jeśli drużyna ma tylko dotrzeć na miejsce, wybierz „Tylko w pobliżu punktu” i „Nic: zbiera dotknięciem w pobliżu punktu”.
- **Drużyna nie widzi pytania** — punkt ma ustawiony dostęp „Tylko w pobliżu punktu”, więc pytanie pojawi się dopiero w zasięgu. Jeśli ustawienie wydarzenia **Kto zbiera punkty** ma wartość „Tylko lider drużyny”, pytanie zobaczy wyłącznie lider — pozostali członkowie nie zobaczą go nawet przy punkcie.
- **Członek drużyny nie może odpowiedzieć** — jeśli ustawienie wydarzenia **Kto zbiera punkty** ma wartość „Tylko lider drużyny”, odpowiada tylko lider; aby odpowiadać mógł każdy członek, zmień je na „Wszyscy członkowie drużyny”.
- **Drużyna nie może odpowiedzieć** — sprawdź, czy drużyna nie wykorzystała limitu prób, czy nie trwa przerwa po błędnej odpowiedzi i czy wydarzenie się nie zakończyło.
- **„Hasło w kratkach ma jedną odpowiedź, bez innych pisowni”** — kod w kratkach przyjmuje tylko jedną odpowiedź; usuń inne pisownie albo wyłącz kratki.
- **„Zaktualizuj aplikację, aby odpowiedzieć na ten punkt”** — drużyna korzysta ze starszej wersji aplikacji.
