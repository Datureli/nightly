---
id: #NFTSEARCH001
title: Sprawdź funkcjonalność paska wyszukiwania NFT
description: Testy funkcjonalności paska wyszukiwania NFT,  w tym poprawność wyników, wydajność i responsywność
test Scenario: Weryfikacja działania paska wyszukiwania NFT w różnych warunkach
Test Steps:
  - Wyszukiwanie NFT przy użyciu różnych zapytań
  - Testowanie wydajności przy dużej liczbie NFT
  - Testowanie na różnych przeglądarkach i urządzeniach
Prerequisites: Strona z listą NFT i paskiem wyszukiwania jest dostępna
Expected/Intended Results: Pasek wyszukiwania działa poprawnie, zwracając odpowiednie wyniki, i jest responsywny na różnych urządzeniach i przeglądarkach
---

## Przypadek: 1a: Sprawdź podstawowe wyszukiwanie NFT

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź popularne słowo kluczowe (np. `BEER`) w pasek wyszukiwania
- Kliknij przycisk wyszukiwania lub naciśnij Enter
- Sprawdź, czy wyniki wyszukiwania zawierają NFT związane z wprowadzonym słowem kluczowym

**Oczekiwany rezultat:** Pasek wyszukiwania zwraca wyniki odpowiadające wprowadzonej frazie

---

## Przypadek: 1b: Sprawdź wyszukiwanie z użyciem części słowa kluczowego

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź część słowa kluczowego (np. `BE`) w pasek wyszukiwania
- Kliknij przycisk wyszukiwania lub naciśnij Enter
- Sprawdź, czy wyniki wyszukiwania zawierają NFT, których pełna nazwa zawiera wprowadzone fragmenty

**Oczekiwany rezultat:** Pasek wyszukiwania zwraca wyniki odpowiadające części słowa kluczowego

---

## Przypadek: 1c: Sprawdź wyszukiwanie z użyciem znaków specjalnych

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź zapytanie zawierające znaki specjalne (np. `BEER?`) w pasek wyszukiwania
- Kliknij przycisk wyszukiwania lub naciśnij Enter
- Sprawdź, czy wyniki wyszukiwania zawierają NFT związane z wprowadzonym zapytaniem

**Oczekiwany rezultat:** Pasek wyszukiwania prawidłowo obsługuje znaki specjalne i zwraca odpowiednie wyniki

---

## Przypadek: 1d: Sprawdź reakcję na wprowadzenie pustego zapytania

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wyczyść pasek wyszukiwania
- Kliknij przycisk wyszukiwania lub naciśnij Enter bez wprowadzania żadnego zapytania
- Sprawdź, czy wyświetla się komunikat o braku wyników lub wszystkie dostępne NFT są wyświetlane

**Oczekiwany rezultat:** Pasek wyszukiwania obsługuje puste zapytanie i wyświetla odpowiedni komunikat lub pełną listę NFT

---

## Przypadek: 1e: Sprawdź wyszukiwanie przy dużej liczbie NFT

**Kroki testowe:**

- Otwórz stronę z dużą liczbą NFT (np. 1000 NFT)
- Wprowadź popularne słowo kluczowe w pasek wyszukiwania
- Kliknij przycisk wyszukiwania lub naciśnij Enter
- Sprawdź czas ładowania wyników i ich dokładność

**Oczekiwany rezultat:** Pasek wyszukiwania działa poprawnie i efektywnie nawet przy dużej liczbie NFT, a wyniki są zwracane w rozsądnym czasie

---

## Przypadek: 1f: Sprawdź działanie paska wyszukiwania na różnych przeglądarkach

**Kroki testowe:**

- Otwórz stronę z listą NFT w przeglądarkach Chrome, Firefox, Safari i Edge
- Wprowadź zapytanie w pasek wyszukiwania
- Kliknij przycisk wyszukiwania lub naciśnij Enter
- Sprawdź, czy wyniki wyszukiwania są poprawnie wyświetlane we wszystkich przeglądarkach

**Oczekiwany rezultat:** Pasek wyszukiwania działa poprawnie w różnych przeglądarkach, zwracając odpowiednie wyniki

---

## Przypadek: 1g: Sprawdź działanie paska wyszukiwania na różnych urządzeniach

**Kroki testowe:**

- Otwórz stronę z listą NFT na komputerze, tablecie i telefonie
- Wprowadź zapytanie w pasek wyszukiwania
- Kliknij przycisk wyszukiwania lub naciśnij Enter
- Sprawdź, czy wyniki wyszukiwania są poprawnie wyświetlane na wszystkich urządzeniach

**Oczekiwany rezultat:** Pasek wyszukiwania działa poprawnie na wszystkich testowanych urządzeniach, zwracając odpowiednie wyniki

---

## Przypadek: 1h: Sprawdź wyszukiwanie z różnymi językami i alfabetami

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź zapytanie w różnych językach i alfabetach (np. chińskie znaki, cyrylica)
- Kliknij przycisk wyszukiwania lub naciśnij Enter
- Sprawdź, czy wyniki wyszukiwania odpowiadają wprowadzonym zapytaniom

**Oczekiwany rezultat:** Pasek wyszukiwania prawidłowo obsługuje różne języki i alfabety, zwracając odpowiednie wyniki

---

## Przypadek: 1i: Sprawdź działanie ikony lupki (search)

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź zapytanie w pasek wyszukiwania
- Kliknij ikonę lupki (search)
- Sprawdź, czy wyniki wyszukiwania odpowiadają wprowadzonej frazie

**Oczekiwany rezultat:** Kliknięcie w ikonę lupki (search) powoduje poprawne wyświetlenie wyników wyszukiwania odpowiadających wprowadzonej frazie

---

## Przypadek: 1j: Sprawdź wyszukiwanie za pomocą klawisza Enter

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź zapytanie w pasek wyszukiwania
- Naciśnij klawisz Enter
- Sprawdź, czy wyniki wyszukiwania odpowiadają wprowadzonej frazie

**Oczekiwany rezultat:** Naciśnięcie klawisza Enter powoduje poprawne wyświetlenie wyników wyszukiwania odpowiadających wprowadzonej frazie

---

## Przypadek: 1k: Sprawdź, czy wyszukiwanie jest reaktywne

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź zapytanie w pasek wyszukiwania
- Obserwuj wyniki wyszukiwania podczas wpisywania zapytania bez naciśnięcia Enter lub kliknięcia przycisku wyszukiwania

**Oczekiwany rezultat:** Wyniki wyszukiwania aktualizują się na bieżąco podczas wpisywania zapytania w pasek wyszukiwania

---

## Przypadek: 1l: Sprawdź, czy wyniki wyszukiwania są takie same po kliknięciu ikony lupki i naciśnięciu klawisza Enter

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź zapytanie w pasek wyszukiwania
- Kliknij ikonę lupki (search) i zanotuj wyniki
- Wprowadź to samo zapytanie ponownie i naciśnij klawisz Enter
- Zanotuj wyniki
- Porównaj wyniki uzyskane poprzez kliknięcie ikony lupki i naciśnięcie klawisza Enter

**Oczekiwany rezultat:** Wyniki wyszukiwania uzyskane przez kliknięcie ikony lupki (search) i naciśnięcie klawisza Enter są identyczne

---

## Przypadek: 1m: Sprawdź, czy wyszukiwanie jest reaktywne na bieżąco

**Kroki testowe:**

- Otwórz stronę z listą NFT
- Wprowadź zapytanie w pasek wyszukiwania
- Obserwuj wyniki wyszukiwania podczas wpisywania zapytania bez naciśnięcia Enter lub kliknięcia przycisku wyszukiwania

**Oczekiwany rezultat:** Wyniki wyszukiwania aktualizują się na bieżąco podczas wpisywania zapytania w pasek wyszukiwania
