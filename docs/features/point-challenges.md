# Zadania punktów

Zadania zastępują dotychczasowe pole hasła i opcję zbierania przez GPS w formularzu punktu. Zamiast jednego hasła organizator może poprosić drużynę o podanie liczby, wpisanie kodu jak w kłódce, wybór odpowiedzi z listy, ułożenie elementów w kolejności czy uzupełnienie luk w zdaniu. Do zadania można dodać limit prób, karę za błędną odpowiedź, przerwę między próbami oraz płatne podpowiedzi.

Sekcja **Zadanie** jest dostępna w formularzu punktu zarówno w aplikacji, jak i w panelu administratora. Nowy punkt domyślnie dostaje zadanie typu **Hasło** — jeśli zostawisz je puste, hasło zostanie wygenerowane automatycznie, tak jak dotychczas.

## Skąd drużyna może zebrać punkt?

Pierwsza decyzja w sekcji **Zadanie** formularza punktu to sposób dostępu do punktu:

| Opcja | Zadanie | Jak działa |
|-------|---------|------------|
| **Z dowolnego miejsca** | wymagane | Drużyna odpowiada na zadanie z dowolnego miejsca, nie musi być przy punkcie |
| **Tylko w pobliżu punktu** | brak | Drużyna zbiera punkt dotknięciem, gdy jest w zasięgu (zbieranie przez GPS) |
| **Tylko w pobliżu punktu** | ustawione | Pytanie jest widoczne i można na nie odpowiedzieć dopiero w zasięgu punktu — wcześniej drużyna widzi komunikat „Podejdź bliżej, aby zobaczyć pytanie” |
| **W pobliżu punktu lub z dowolnego miejsca** | wymagane | W zasięgu drużyna zbiera punkt dotknięciem, poza zasięgiem — odpowiadając na zadanie |

Istniejące punkty zostały przeniesione automatycznie:
- punkt z hasłem i włączonym zbieraniem przez GPS → **W pobliżu punktu lub z dowolnego miejsca** z zadaniem typu **Hasło**,
- punkt z hasłem bez GPS → **Z dowolnego miejsca** z zadaniem typu **Hasło**.

> Zasięg punktu wynika z ustawień GPS wydarzenia. Jeśli drużyna wyjdzie poza zasięg w trakcie odpowiadania na punkt „tylko w pobliżu”, wpisana odpowiedź zostaje — wystarczy wrócić.

## Rodzaje zadań

Pole **Co musi zrobić drużyna** określa rodzaj zadania:

| Rodzaj | Co robi drużyna | Co ustawia organizator |
|--------|-----------------|------------------------|
| **Hasło** | Wpisuje słowo lub frazę | Główną odpowiedź i dowolną liczbę innych pisowni. Puste hasło zostanie wygenerowane automatycznie |
| **Tylko litery** | Jak hasło, ale pole przyjmuje wyłącznie litery i spacje | Odpowiedzi |
| **Liczba** | Podaje liczbę | Dokładną wartość z tolerancją (±) albo przedział (od–do) |
| **Kod o stałej długości** | Wpisuje kod znak po znaku, jak w kłódce szyfrowej | Kod oraz dozwolone znaki: cyfry, litery A–Z lub litery A–Z i cyfry (bez polskich znaków) |
| **Jednokrotny wybór** | Wybiera jedną odpowiedź z listy | Odpowiedzi do wyboru i dokładnie jedną poprawną |
| **Wielokrotny wybór** | Zaznacza wszystkie poprawne odpowiedzi — i tylko je | Odpowiedzi do wyboru i co najmniej jedną poprawną |
| **Uzupełnij luki** | Uzupełnia brakujące słowa w zdaniu, wpisując je lub wybierając z puli słów | Zdanie z lukami, opcjonalnie pulę słów i słowa-pułapki |
| **Kolejność** | Układa elementy we właściwej kolejności (przeciągając lub strzałkami) | Elementy w poprawnej kolejności — każda drużyna zobaczy je wymieszane |
| **Kilka haseł** | Podaje kilka haseł, każde w osobnym polu | Od 2 do 10 haseł i informację, czy ich kolejność ma znaczenie |

Odpowiedź jest oceniana w całości — jest albo w pełni poprawna, albo błędna (nie ma punktów częściowych).

### Wskazówki do poszczególnych rodzajów

- **Jednokrotny / wielokrotny wybór** — można włączyć opcję **Mieszaj odpowiedzi inaczej dla każdej drużyny**, żeby drużyny nie podpowiadały sobie „to trzecia odpowiedź”.
- **Uzupełnij luki** — lukę zapisuje się w zdaniu jako `[[odpowiedź]]`, a inne poprawne odpowiedzi oddziela się znakiem `|`, np. `Stolicą Małopolski jest [[Kraków|Krakow]].` Można też zaznaczyć słowo i użyć przycisku **Zamień zaznaczenie w lukę**. Zdanie może mieć do 20 luk. Po włączeniu **puli słów** drużyna widzi do wyboru odpowiedzi z luk oraz do 10 słów-pułapek.
- **Kilka haseł** — jeśli kolejność nie ma znaczenia, każde hasło można użyć tylko raz (podanie dwa razy tego samego hasła nie zaliczy dwóch pól).

## Treść zadania

- **Pytanie (opcjonalne)** — obsługuje to samo formatowanie i multimedia co opis punktu. Przy punkcie zbieranym tylko w pobliżu drużyna zobaczy pytanie dopiero po podejściu.
- Pod formularzem widać podgląd **Tak zobaczy to drużyna**.

## Ustawienia zaawansowane

Sekcja **Ustawienia zaawansowane** jest domyślnie zwinięta i otwiera się sama, jeśli punkt już korzysta z któregoś ustawienia.

- **Limit prób** (przełącznik **Ogranicz liczbę prób**) — od 1 do 999 prób. Po wyczerpaniu prób drużyna nie może już odpowiadać, dopóki organizator nie odblokuje punktu.
- **Przerwa (sekundy)** — czas, który musi minąć po błędnej odpowiedzi przed kolejną próbą (maksymalnie 24 godziny). 0 = bez przerwy.
- **Kara (PZ)** — liczba punktów odejmowana od wyniku drużyny za każdą błędną odpowiedź. 0 = bez kary.
- **Komunikat po błędnej odpowiedzi** — własny tekst pokazywany drużynie po pomyłce.
- **Podpowiedzi** (przełącznik **Dodaj podpowiedzi**) — do 10 podpowiedzi, każda z własnym kosztem w PZ (może być darmowa). Szczegóły niżej.
- **Przy porównywaniu odpowiedzi pomijaj** — wielkość liter, nadmiarowe spacje oraz polskie znaki (ą = a, ł = l). Dotyczy zadań tekstowych.

> Odpowiedź w złym formacie (np. pusta) nie liczy się jako próba i nie nalicza kary.

## Podpowiedzi

- Drużyna odkrywa podpowiedzi **po kolei** — nie można pominąć pierwszej i od razu kupić drugiej.
- Przed odkryciem płatnej podpowiedzi aplikacja prosi o potwierdzenie („Podpowiedź odejmie drużynie N PZ. Pokazać ją?”).
- Koszt jest odejmowany od wyniku drużyny raz — nawet jeśli dwie osoby z drużyny klikną jednocześnie.
- Odkryte podpowiedzi widzą wszyscy członkowie drużyny, ale odkryć je może tylko lider.
- Podpowiedzi nie można odkryć po zakończeniu wydarzenia ani po zebraniu punktu.

> Nie zmieniaj kolejności ani nie usuwaj podpowiedzi w trakcie gry — drużyny, które już je odkryły, zobaczą teksty z nowych pozycji (zapłacony koszt się nie zmienia).

## Jak to wygląda dla drużyny?

Po otwarciu punktu drużyna widzi panel zadania z pytaniem, polem odpowiedzi oraz informacjami o zasadach: liczbie pozostałych prób (lub „Bez limitu prób”), wysokości kary i czasie do następnej próby.

- **Odpowiedź wysyła tylko lider drużyny** — pozostali członkowie widzą zadanie w trybie podglądu.
- Po poprawnej odpowiedzi punkt zostaje zebrany jak dotychczas (nagrody, wiadomość po zebraniu itd.).
- Po wykorzystaniu wszystkich prób drużyna widzi komunikat z prośbą o kontakt z organizatorem.
- Starsze wersje aplikacji mogą nie obsługiwać nowych rodzajów zadań — wtedy drużyna zobaczy prośbę o aktualizację aplikacji.

## Wpływ na wynik

Kary za błędne odpowiedzi i koszty podpowiedzi są odejmowane od wyniku drużyny. W szczegółach wyniku w tabeli wyników widoczna jest pozycja **Kary za błędne odpowiedzi**, a w podglądzie historii wydarzenia w panelu administratora — „zadania: −N”.

## Narzędzia organizatora (panel administratora)

### Drużyny i próby

W formularzu punktu z zadaniem panel **Drużyny i próby** pokazuje dla każdej drużyny: liczbę prób (i limit), naliczone kary, wykorzystane podpowiedzi, trwającą przerwę, ostatnie błędne odpowiedzi oraz status (zebrany / zablokowany).

Przycisk **Odblokuj** zeruje licznik prób drużyny i kończy przerwę. Naliczone wcześniej kary i koszty podpowiedzi **nie są zwracane**.

### Edycja zbiorcza

W edycji zbiorczej punktów opcja **Ustawienia zadania** ustawia jednocześnie limit prób, przerwę i karę we wszystkich zaznaczonych punktach z zadaniem. Punkty zbierane dotknięciem są pomijane. Tabela punktów ma też kolumny **Skąd zebrać** i **Zadanie**.

### Statystyki zadań

Widok **Zadania punktów** w menu panelu administratora pokazuje, jak drużyny radzą sobie z zadaniami — najtrudniejsze punkty są na górze. Dla każdego punktu widać m.in.: ile drużyn próbowało, ile odpowiedziało dobrze, liczbę odpowiedzi, odsetek błędnych, sumę kar i podpowiedzi oraz **najczęstsze błędne odpowiedzi** wraz z drużynami, które je podały. To dobre miejsce, żeby w trakcie gry wyłapać pytania za trudne albo niejednoznaczne (np. brakującą pisownię hasła). Widok jest dostępny dla twórcy, administratorów i obserwatorów wydarzenia.

## Kopiowanie i resetowanie wydarzenia

- Przy kopiowaniu wydarzenia zadania punktów są kopiowane razem z punktami.
- Duplikat punktu z hasłem dostaje nowe, wygenerowane hasło (inne pisownie nie są kopiowane).
- Reset wydarzenia czyści próby, kary i odkryte podpowiedzi wszystkich drużyn.

## Najczęstsze problemy

- **„Punkt zbierany z dowolnego miejsca wymaga zadania”** — opcje „Z dowolnego miejsca” oraz „W pobliżu punktu lub z dowolnego miejsca” wymagają ustawienia zadania. Bez zadania wybierz „Tylko w pobliżu punktu”.
- **Drużyna nie widzi pytania** — punkt ma ustawiony dostęp „Tylko w pobliżu punktu”, więc pytanie pojawi się dopiero w zasięgu.
- **Drużyna nie może odpowiedzieć** — odpowiedź może wysłać tylko lider drużyny; sprawdź też, czy drużyna nie wykorzystała limitu prób lub nie trwa przerwa po błędnej odpowiedzi.
- **„Zaktualizuj aplikację, aby odpowiedzieć na ten punkt”** — drużyna korzysta ze starszej wersji aplikacji.
