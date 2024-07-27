---
id: #NFTLIST001
title: Sprawdź wyświetlanie komunikatu "Nie znaleziono żadnego NFT..."
description: Testy wyświetlania komunikatu, gdy brak jest NFT spełniających kryteria wyszukiwania oraz czas reakcji systemu
test Scenario: Weryfikacja wyświetlania komunikatu o braku wyników i czasu reakcji systemu
Test Steps:
  - Wyszukiwanie NFT z zapytaniem, które nie zwraca żadnych wyników
  - Sprawdzenie czasu, jaki zajmuje wyświetlenie komunikatu "Nie znaleziono żadnego NFT..."
Prerequisites: Strona z listą NFT i paskiem wyszukiwania jest dostępna
Expected/Intended Results: Komunikat o braku wyników wyświetla się w rozsądnym czasie, a użytkownik nie musi długo czekać
---

## Przypadek: 1a: Sprawdź wyświetlanie komunikatu "Nie znaleziono żadnego NFT..."

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź zapytanie, które na pewno nie zwróci żadnych wyników (np. "NonExistentNFT")
- Kliknij przycisk wyszukiwania lub naciśnij Enter
- Sprawdź, czy komunikat "Nie znaleziono żadnego NFT..." jest wyświetlany

**Oczekiwany rezultat:** Komunikat "Nie znaleziono żadnego NFT..." jest wyświetlany, gdy nie ma żadnych wyników wyszukiwania

## Przypadek: 1b: Sprawdź czas wyświetlania komunikatu "Nie znaleziono żadnego NFT..."

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź zapytanie, które na pewno nie zwróci żadnych wyników (np. "NonExistentNFT")
- Kliknij przycisk wyszukiwania lub naciśnij Enter
- Zmierz czas, jaki upływa od momentu wysłania zapytania do momentu wyświetlenia komunikatu "Nie znaleziono żadnego NFT..."

**Oczekiwany rezultat:** Komunikat "Nie znaleziono żadnego NFT..." wyświetla się w rozsądnym czasie, nie przekraczając 2-3 sekund

## Przypadek: 1c: Sprawdź, czy użytkownik nie musi długo czekać na wyświetlenie komunikatu

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź zapytanie, które na pewno nie zwróci żadnych wyników (np. "NonExistentNFT")
- Kliknij przycisk wyszukiwania lub naciśnij Enter
- Obserwuj czas reakcji systemu i odczucie użytkownika

**Oczekiwany rezultat:** Użytkownik nie musi długo czekać na wyświetlenie komunikatu o braku wyników, a reakcja systemu jest szybka

---

id: #NFTSIZE001
title: Sprawdź wybór rozmiaru wyświetlania NFT
description: Testy wyboru rozmiaru wyświetlania NFT z użyciem ikony trzech kropek (1, 4 kwadraty, 9 kwadratów)
test Scenario: Weryfikacja poprawności działania wyboru rozmiaru wyświetlania NFT
Test Steps:
  - Wybór różnych rozmiarów wyświetlania NFT
  - Sprawdzenie poprawności układu i reakcji na zmianę rozmiaru
Prerequisites: Strona z listą NFT i ikoną trzech kropek do wyboru rozmiaru jest dostępna
Expected/Intended Results: Wybór rozmiaru wyświetlania NFT działa poprawnie, a układ NFT jest zgodny z wybranym rozmiarem
---

## Przypadek: 2a: Sprawdź wybór rozmiaru 1 kwadrat

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Kliknij ikonę trzech kropek i wybierz opcję wyświetlania jako 1 kwadrat
- Sprawdź, czy NFT są wyświetlane w układzie 1x1 (jeden duży kwadrat)

**Oczekiwany rezultat:** NFT są wyświetlane w układzie 1x1, a widok jest odpowiednio dostosowany

## Przypadek: 2b: Sprawdź wybór rozmiaru 4 kwadraty

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Kliknij ikonę trzech kropek i wybierz opcję wyświetlania jako 4 kwadraty
- Sprawdź, czy NFT są wyświetlane w układzie 2x2 (cztery mniejsze kwadraty)

**Oczekiwany rezultat:** NFT są wyświetlane w układzie 2x2, a widok jest odpowiednio dostosowany

## Przypadek: 2c: Sprawdź wybór rozmiaru 9 kwadratów

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Kliknij ikonę trzech kropek i wybierz opcję wyświetlania jako 9 kwadratów
- Sprawdź, czy NFT są wyświetlane w układzie 3x3 (dziewięć małych kwadratów)

**Oczekiwany rezultat:** NFT są wyświetlane w układzie 3x3, a widok jest odpowiednio dostosowany

## Przypadek: 2d: Sprawdź, czy zmiana rozmiaru wyświetlania działa płynnie

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Kliknij ikonę trzech kropek i wybierz opcję wyświetlania jako 1 kwadrat
- Zmieniając opcje, przełącz się na 4 kwadraty i 9 kwadratów
- Obserwuj, czy zmiana rozmiaru jest płynna i bez opóźnień

**Oczekiwany rezultat:** Zmiana rozmiaru wyświetlania NFT odbywa się płynnie, bez widocznych opóźnień

## Przypadek: 2e: Sprawdź, czy układ jest poprawny na różnych rozmiarach okna przeglądarki

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Kliknij ikonę trzech kropek i wybierz różne opcje wyświetlania
- Zmniejsz i powiększ rozmiar okna przeglądarki
- Sprawdź, czy układ NFT jest poprawnie dostosowany do rozmiaru okna

**Oczekiwany rezultat:** Układ NFT jest poprawnie dostosowany do rozmiaru okna przeglądarki, niezależnie od wybranej opcji wyświetlania

---

id: #NFTDISPLAY001
title: Sprawdź wyświetlanie nazw i liczby NFT na zdjęciach
description: Testy dotyczące wyświetlania nazw NFT oraz liczby NFT na zdjęciach, w tym obsługa długich nazw i dużych liczb
test Scenario: Weryfikacja poprawności wyświetlania nazw i liczby NFT oraz obsługi długich nazw i liczb
Test Steps:
  - Sprawdzenie wyświetlania nazw NFT i liczby obok nazw
  - Testowanie działania przy długich nazw i dużych liczbach
Prerequisites: Strona z listą NFT oraz zdjęciami NFT jest dostępna
Expected/Intended Results: Nazwy NFT i liczby są poprawnie wyświetlane, a długie nazwy i duże liczby są obsługiwane w sposób czytelny
---

## Przypadek: 3a: Sprawdź, czy na zdjęciach pojawia się nazwa NFT

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Sprawdź, czy pod każdym zdjęciem NFT wyświetla się nazwa NFT

**Oczekiwany rezultat:** Nazwa NFT jest poprawnie wyświetlana pod każdym zdjęciem NFT

## Przypadek: 3b: Sprawdź, czy na zdjęciach pojawia się liczba NFT obok nazwy

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Sprawdź, czy obok nazwy NFT wyświetlana jest liczba NFT

**Oczekiwany rezultat:** Liczba NFT jest poprawnie wyświetlana obok nazwy NFT na zdjęciach

## Przypadek: 3c: Sprawdź obsługę długich nazw NFT

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź NFT z bardzo długą nazwą (np. "Super Long NFT Name That Should Test The Layout")
- Sprawdź, czy długa nazwa NFT jest czytelna i nie zakrywa liczby NFT obok

**Oczekiwany rezultat:** Długa nazwa NFT jest wyświetlana w sposób czytelny, a liczba NFT obok nie jest zakrywana

## Przypadek: 3d: Sprawdź obsługę długich liczb NFT

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź NFT z dużą liczbą (np. 123456789)
- Sprawdź, czy duża liczba NFT jest poprawnie wyświetlana i nie wychodzi poza granice zdjęcia

**Oczekiwany rezultat:** Duża liczba NFT jest wyświetlana poprawnie, bez wychodzenia poza granice zdjęcia

## Przypadek: 3e: Sprawdź, co się stanie, gdy nazwa NFT jest zbyt długa

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź NFT z nazwą tak długą, że powinna wyjść poza widoczny obszar (np. "NFTNameThatIsExtremelyLongAndShouldOverflowTheContainer")
- Sprawdź, czy tekst nazwy NFT jest przycinany lub przewijany w sposób czytelny, a liczba NFT obok jest widoczna

**Oczekiwany rezultat:** Nazwa NFT jest przycinana lub przewijana w sposób czytelny, a liczba NFT obok jest widoczna

## Przypadek: 3f: Sprawdź, co się stanie, gdy liczba NFT jest zbyt duża

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź NFT z liczbą, która może być za duża (np. 999999999)
- Sprawdź, czy liczba NFT jest wyświetlana poprawnie, nie wychodząc poza granice zdjęcia

**Oczekiwany rezultat:** Liczba NFT jest wyświetlana poprawnie, bez wychodzenia poza granice zdjęcia

## Przypadek: 3g: Sprawdź wyświetlanie nazw i liczby NFT na różnych rozmiarach okna przeglądarki

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Zmieniaj rozmiar okna przeglądarki
- Sprawdź, czy nazwy NFT i liczby są poprawnie wyświetlane na różnych rozmiarach okna

**Oczekiwany rezultat:** Nazwy NFT i liczby są poprawnie wyświetlane, a układ dostosowuje się do zmiany rozmiaru okna przeglądarki
