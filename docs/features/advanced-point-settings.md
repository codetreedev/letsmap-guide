# Zaawansowane ustawienia punktu
Autor: **Paweł Bednarczyk**

Punkty rozmieszczane na mapie są najważniejszymi elementami aplikacji, dlatego chcemy udostępnić dużą ilość możliwość konfiguracji a z drugiej strony zachować prostotę, żeby początkujący administratorzy nie zatonęli w morzu opcji.

Formularz tworzenia punktów składa się z pięciu sekcji:
1. Informacje ogólne:
   - Nazwa punktu – Nazwa punktu widoczna dla uczestników 
   - Hasło do zebrania punktu – Składające się z przynajmniej trzech znaków hasło, które po wpisaniu do aplikacji umożliwi drużynom zebranie punktu. 
   - Opis punktu – Opis punktu widoczny dla użytkowników, można zawrzeć w nim fabularną historię, zagadkę lub podpowiedzi gdzie dokładnie szukać karteczki z punktem
2. Typ punktu
   - Typ zbieralności punktu – punkty mogą być możliwe do zebrania tylko przez jedną drużynę lub dostępne do zebrania przez wszystkie drużyny
   - Kategoria punktu – Kategorie punktów tworzone są w osobnym formularzu i przy tworzeniu punktu należy go jedynie przypisać do odpowiedniej kategorii, określa ona wygląd punktu na mapie, jego wartość punktową a także opis kategorii jest dostępny przy każdym punkcie, który do niej należy
   - Możliwość zbierania punktu poprzez GPS – ta opcja działa jedynie jeśli ustawienie wydarzenie pozwalają zbierać punkty poprzez GPS. Jest to wartość prawa/fałsz
3. Ustawienia mapy
   - Możliwość, w którym miejscu znajduje się dany punkt
4. Typ widoczności punktu
   - Typ widoczności punktu – jest to nadrzędna cecha, która kontroluje dalsze opcje ustawienia
   - Punkt widoczny – bazowy punkt jest zawsze widoczny przez cały okres trwania wydarzenia
   - Punkt czasowy – punkt widoczny jest przez wybrany przed administratora przedział czasowy*
   - Punkt ukryty – punkt widoczny jest tylko dla drużyn, które spełniają odpowiednie kryteria np. posiadają odpowiedni przedmiot (mapę)
   - Punkt ukryty czasowy – połączenie punktów ii) i iii), punkt jest widoczny w przedziale czasowym tylko dla drużyn, które posiadają odpowiedni przedmiot
5. Akcje po zebraniu punktu
   - Wiadomość po zebraniu punktu
   - Przedmioty jakie w nagrodę dostanie drużyna zbierająca punkt

-------------------

Ustalanie przedziałów czasowych punktów możliwe polega na podaniu godziny pojawienia i zniknięcia punktu, przy czym ustalić jest można jako konkretną godzinę lub w sposób relatywny:
   - Data i godzina – ustawienie na konkretną godzinę – jest to najprostsza opcja, ale powoduje problemy jeśli czas wydarzenia miałby ulec zmianie
   Relatywne – Umożliwia ustawienie 6 markerów czasu i dodanie różnicy od nich w minutach
   - Przed startem wydarzenia – rzadko używane, ale może posłużyć jako oznaczenie punktu startowego jeśli użytkownicy zarejestrują się do aplikacji przed przybyciem na miejsce
   - Start wydarzenia – domyślna opcja dla pojawienia się punktu
   - Po stracie wydarzenia – można ustawić czas, kiedy punkt się pojawi relatywnie względem czasu rozpoczęcia wydarzenia (godzinę po rozpoczęciu np.)
   - Przed końcem wydarzenia – można ustawić czas, kiedy punkt zniknie relatywnie względem czasu zakończenia wydarzenia (godzinę przed zakończeniem np.)
   - Koniec wydarzenia – domyślna opcja dla wygaśnięcia punktu
   - Po końcu wydarzenia – rzadko używane, ale może posłużyć do ukrycia miejsca końcowej zbiórki (jako dodatkowe zadanie)
