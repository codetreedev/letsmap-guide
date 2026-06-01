# Tryb ciemności
Autor: **Paweł Bednarczyk**

Tryb ciemności to zaawansowana funkcjonalność, która zmienia sposób, w jaki uczestnicy widzą mapę podczas gry. Zamiast pełnej widoczności, mapa jest zakryta ciemnością — widoczny jest tylko obszar wokół aktualnej pozycji GPS gracza. Dzięki temu uczestnicy muszą fizycznie eksplorować teren, żeby odkryć rozmieszczenie punktów.

Tryb ciemności jest funkcją **eksperymentalną** — działa stabilnie, ale może być rozwijany w kolejnych wersjach.

## Jak włączyć?

Tryb ciemności włącza się w zaawansowanych ustawieniach wydarzenia (**Tryb ciemności na mapie → Włączony**). Organizator może przetestować jego wygląd bezpośrednio z panelu admina, zmieniając ustawienia mapy w prawym górnym rogu widoku mapy.

## Warianty konfiguracji

### 1. Podstawowy tryb ciemności

Najprostsza konfiguracja — mapa jest zakryta, gracze widzą tylko obszar w wybranym promieniu wokół siebie.

**Ustawienia**:
- Tryb ciemności: **Włączony**
- Radar: **Wyłączony**
- Odkrywanie mapy: **Wyłączone**

**Efekt**: Uczestnicy nie wiedzą gdzie są punkty i muszą fizycznie przemierzać teren, żeby je znaleźć. Najtrudniejszy wariant — wymaga dobrej znajomości lub eksploracji terenu.

---

### 2. Tryb ciemności z radarem

Ciemność uzupełniona o wskaźnik kierunku i odległości do najbliższych niezebranych punktów. Radar pojawia się na krawędzi widocznego obszaru.

**Ustawienia**:
- Tryb ciemności: **Włączony**
- Radar: **Włączony**
- Liczba radarów: 1–5 (ile punktów jednocześnie jest wskazywanych)
- Podgląd kategorii na radarze: opcjonalnie

**Efekt**: Gracze wiedzą, w którym kierunku i jak daleko jest najbliższy punkt, ale nadal muszą do niego dojść. Balans między eksploracją a orientacją. Podgląd kategorii na radarze pozwala graczom zdecydować, czy dany punkt jest dla nich priorytetem.

---

### 3. Tryb mgły wojny (odkrywanie mapy)

Odwiedzone obszary pozostają widoczne na mapie — gracze stopniowo "odkrywają" mapę podczas gry. Odkryte kafelki mogą z czasem znikać, wymuszając ponowną eksplorację.

**Ustawienia**:
- Tryb ciemności: **Włączony**
- Odkrywanie mapy: **Włączone**
- Czas wygasania kafelków: od 1 minuty do braku wygasania

**Efekt**: Gracze budują widoczność mapy w miarę poruszania się. Z krótkim czasem wygasania (np. 5–15 minut) muszą cały czas być w ruchu, żeby zachować widoczność. Z wyłączonym wygasaniem mapa staje się coraz bardziej odkryta w miarę eksploracji.

> **Uwaga**: Odkryta mapa nie jest aktualnie synchronizowana między urządzeniami tej samej drużyny.

---

### 4. Tryb ciemności z modyfikacją przez przedmioty

Gracze mogą zdobywać przedmioty, które zmieniają ich promień widoczności. Atrybuty przedmiotów umożliwiają zarówno powiększenie jak i zmniejszenie widocznego obszaru.

**Ustawienia**:
- Tryb ciemności: **Włączony**
- Przedmioty z atrybutem **Promień widoczności** dodane do puli nagród

**Efekt**: Zebranie odpowiedniego przedmiotu rozszerza zasięg widzenia drużyny. Można zaprojektować grę, gdzie kluczowym zadaniem jest najpierw zdobycie "latarni" lub "mapy", żeby w ogóle móc eksplorować teren.

[Dowiedz się więcej o atrybutach przedmiotów](features/item-attributes.md)

---

## Zasięg widoczności a dokładność GPS

Tryb ciemności korzysta z dwóch osobnych ustawień zasięgu:

- **Dokładna lokalizacja** — gdy GPS działa dobrze (otwarta przestrzeń): od 10 do 1000 metrów
- **Niedokładna lokalizacja** — gdy GPS ma słaby sygnał (budynki, las): od 5 do 50 metrów

Dzięki temu gracze z gorszym sygnałem GPS nie są nadmiernie karani. Administrator powinien dobrać wartości do charakteru terenu, na którym odbywa się gra.

## Punkty a tryb ciemności

Punkty, które są niewidoczne dla drużyny z powodu ciemności (poza zasięgiem), **nie mogą być zebrane przez GPS**. Drużyna musi fizycznie podejść na tyle blisko, żeby punkt znalazł się w widocznym obszarze.
