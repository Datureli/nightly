---
id: #AMOUNTINPUT002
title: Sprawdź, czy pole input "amount" akceptuje wartości liczbowe i obsługuje komunikaty o niewystarczającym stanie konta
description: Testy funkcji wysyłania tokenu z uwagi na akceptację wartości liczbowych w polu input "amount" oraz obsługę komunikatu o niewystarczającym stanie konta
test Scenario: Weryfikacja akceptacji wartości liczbowych w polu input oraz obsługa sytuacji, gdy stan konta jest niewystarczający
Test Steps:
  - Wprowadź liczbę całkowitą
  - Wprowadź liczbę zmiennoprzecinkową
  - Wprowadź wartość ujemną
  - Wprowadź zero
  - Wprowadź wartość z maksymalną dozwoloną ilością cyfr
  - Sprawdź, czy komunikat o niewystarczającym stanie konta pojawia się, gdy wprowadzona kwota przekracza dostępne środki
Prerequisites: Strona z polem input "amount" i aktualnym stanem konta jest dostępna
Expected/Intended Results: System prawidłowo akceptuje wartości liczbowe w polu input, aktualizuje wartość "max amount", i wyświetla komunikat o niewystarczających środkach, gdy to konieczne
---

## Warunki wstępne
Strona z polem input "amount" jest dostępna, a wartość "max amount" jest wyświetlana

## Przypadek: 1a: Sprawdź akceptację liczb całkowitych
**Kroki testowe:**
- Wprowadź liczbę całkowitą (np. 100) w pole input "amount"
- Sprawdź, czy wartość została poprawnie zaakceptowana i przechowana
- Sprawdź, czy pojawia się komunikat o niewystarczającym stanie konta, gdy kwota przekracza dostępne środki

**Oczekiwany rezultat:**
Pole input akceptuje liczby całkowite i przechowuje je poprawnie. Komunikat o niewystarczającym stanie konta wyświetla się, jeśli wprowadzona kwota przekracza dostępne środki.

## Przypadek: 1b: Sprawdź akceptację liczb zmiennoprzecinkowych
**Kroki testowe:**
- Wprowadź liczbę zmiennoprzecinkową (np. 100.50) w pole input "amount"
- Sprawdź, czy wartość została poprawnie zaakceptowana i przechowana
- Sprawdź, czy pojawia się komunikat o niewystarczającym stanie konta, gdy kwota przekracza dostępne środki

**Oczekiwany rezultat:**
Pole input akceptuje liczby zmiennoprzecinkowe i przechowuje je poprawnie. Komunikat o niewystarczającym stanie konta wyświetla się, jeśli wprowadzona kwota przekracza dostępne środki.

## Przypadek: 1c: Sprawdź akceptację wartości ujemnych
**Kroki testowe:**
- Wprowadź wartość ujemną (np. -100) w pole input "amount"
- Sprawdź, czy wartość została poprawnie zaakceptowana i przechowana
- Sprawdź, czy pojawia się komunikat o niewystarczającym stanie konta, gdy kwota przekracza dostępne środki (powinna pojawić się informacja o błędzie, jeśli wartość ujemna jest nieakceptowalna)

**Oczekiwany rezultat:**
Pole input akceptuje wartości ujemne i przechowuje je poprawnie (jeśli są dozwolone). Komunikat o niewystarczającym stanie konta wyświetla się, jeśli kwota przekracza dostępne środki.

## Przypadek: 1d: Sprawdź akceptację wartości zero
**Kroki testowe:**
- Wprowadź wartość zero (0) w pole input "amount"
- Sprawdź, czy wartość została poprawnie zaakceptowana i przechowana
- Sprawdź, czy pojawia się komunikat o niewystarczającym stanie konta, gdy kwota przekracza dostępne środki (powinna pojawić się informacja, jeśli zero jest niedopuszczalne)

**Oczekiwany rezultat:**
Pole input akceptuje wartość zero i przechowuje ją poprawnie. Komunikat o niewystarczającym stanie konta wyświetla się, jeśli kwota przekracza dostępne środki.

## Przypadek: 1e: Sprawdź akceptację wartości z maksymalną ilością cyfr
**Kroki testowe:**
- Wprowadź wartość z maksymalną dozwoloną ilością cyfr (np. 9999999999) w pole input "amount"
- Sprawdź, czy wartość została poprawnie zaakceptowana i przechowana
- Sprawdź, czy pojawia się komunikat o niewystarczającym stanie konta, gdy kwota przekracza dostępne środki

**Oczekiwany rezultat:**
Pole input akceptuje wartości z maksymalną ilością cyfr i przechowuje je poprawnie. Komunikat o niewystarczającym stanie konta wyświetla się, jeśli wprowadzona kwota przekracza dostępne środki.

## Przypadek: 1f: Sprawdź akceptację wartości poza zakresem
**Kroki testowe:**
- Wprowadź wartość większą niż maksymalna dozwolona wartość (np. 10000000000)
- Wprowadź wartość mniejszą niż minimalna dozwolona wartość (np. -100)
- Sprawdź, czy pojawia się komunikat o błędzie informujący, że wartość jest poza zakresem

**Oczekiwany rezultat:**
Pole input wyświetla odpowiedni komunikat o błędzie dla wartości poza zakresem.

## Przypadek: 1g: Sprawdź komunikat walidacji dla pustego pola
**Kroki testowe:**
- Spróbuj wysłać formularz bez wprowadzania wartości w polu input "amount"
- Sprawdź, czy pojawia się komunikat o błędzie informujący, że pole nie może być puste

**Oczekiwany rezultat:**
Pojawia się odpowiedni komunikat o błędzie informujący, że pole nie może być puste.

## Przypadek: 1h: Sprawdź komunikat walidacji dla zbyt długiej wartości
**Kroki testowe:**
- Wprowadź wartość przekraczającą maksymalną ilość dozwolonych cyfr
- Sprawdź, czy pojawia się komunikat o błędzie informujący, że wartość jest zbyt długa

**Oczekiwany rezultat:**
Pojawia się odpowiedni komunikat o błędzie informujący, że wartość jest zbyt długa.

## Przypadek: 1i: Sprawdź funkcję kopiowania i wklejania
**Kroki testowe:**
- Skopiuj wartość z pola input "amount"
- Wklej wartość do innego pola input
- Sprawdź, czy wartość została poprawnie skopiowana i wklejona

**Oczekiwany rezultat:**
Pole input poprawnie obsługuje kopiowanie i wklejanie wartości.

## Przypadek: 2a: Sprawdź zmianę wartości "max amount" po wprowadzeniu liczby całkowitej
**Kroki testowe:**
- Wprowadź liczbę całkowitą (np. 100) w pole input "amount"
- Sprawdź, czy wartość "max amount" została zaktualizowana
- Sprawdź, czy pojawia się komunikat o niewystarczającym stanie konta, gdy kwota przekracza dostępne środki

**Oczekiwany rezultat:**
Wartość "max amount" jest poprawnie zaktualizowana po wprowadzeniu liczby całkowitej. Komunikat o niewystarczającym stanie konta wyświetla się, jeśli wprowadzona kwota przekracza dostępne środki.

## Przypadek: 2b: Sprawdź zmianę wartości "max amount" po wprowadzeniu liczby zmiennoprzecinkowej
**Kroki testowe:**
- Wprowadź liczbę zmiennoprzecinkową (np. 100.50) w pole input "amount"
- Sprawdź, czy wartość "max amount" została zaktualizowana
- Sprawdź, czy pojawia się komunikat o niewystarczającym stanie konta, gdy kwota przekracza dostępne środki

**Oczekiwany rezultat:**
Wartość "max amount" jest poprawnie zaktualizowana po wprowadzeniu liczby zmiennoprzecinkowej. Komunikat o niewystarczającym stanie konta wyświetla się, jeśli wprowadzona kwota przekracza dostępne środki.

## Przypadek: 2c: Sprawdź zmianę wartości "max amount" po wprowadzeniu wartości ujemnej
**Kroki testowe:**
- Wprowadź wartość ujemną (np. -100) w pole input "amount"
- Sprawdź, czy wartość "max amount" została zaktualizowana
- Sprawdź, czy pojawia się komunikat o niewystarczającym stanie konta, gdy kwota przekracza dostępne środki

**Oczekiwany rezultat:**
Wartość "max amount" jest poprawnie zaktualizowana po wprowadzeniu wartości ujemnej (jeśli dozwolone). Komunikat o niewystarczającym stanie konta wyświetla się, jeśli kwota przekracza dostępne środki.

## Przypadek: 2d: Sprawdź zmianę wartości "max amount" po wprowadzeniu zera
**Kroki testowe:**
- Wprowadź wartość zero (0) w pole input "amount"
- Sprawdź, czy wartość "max amount" została zaktualizowana
- Sprawdź, czy pojawia się komunikat o niewystarczającym stanie konta, gdy kwota przekracza dostępne środki

**Oczekiwany rezultat:**
Wartość "max amount" jest poprawnie zaktualizowana po wprowadzeniu wartości zero. Komunikat o niewystarczającym stanie konta wyświetla się, jeśli kwota przekracza dostępne środki.

## Przypadek: 2g: Sprawdź zmianę wartości "max amount" po pustym polu
**Kroki testowe:**
- Spróbuj wysłać formularz bez wprowadzania wartości w polu input "amount"
- Sprawdź, czy wartość "max amount" została odpowiednio zaktualizowana
- Sprawdź, czy pojawia się komunikat o błędzie informujący, że pole nie może być puste

**Oczekiwany rezultat:**
Pojawia się odpowiedni komunikat o błędzie informujący, że pole nie może być puste, a wartość "max amount" jest aktualizowana zgodnie z tymi wymaganiami.

## Przypadek: 2h: Sprawdź zmianę wartości "max amount" po zbyt długiej wartości
**Kroki testowe:**
- Wprowadź wartość przekraczającą maksymalną ilość dozwolonych cyfr
- Sprawdź, czy wartość "max amount" została odpowiednio zaktualizowana
- Sprawdź, czy pojawia się komunikat o błędzie informujący, że wartość jest zbyt długa

**Oczekiwany rezultat:**
Pojawia się odpowiedni komunikat o błędzie informujący, że wartość jest zbyt długa, a wartość "max amount" jest aktualizowana zgodnie z dozwolonym zakresem.

## Przypadek: 2i: Sprawdź zmianę wartości "max amount" po kopiowaniu i wklejaniu
**Kroki testowe:**
- Skopiuj wartość z pola input "amount"
- Wklej wartość do innego pola input
- Sprawdź, czy wartość "max amount" została odpowiednio zaktualizowana

**Oczekiwany rezultat:**
Pole input poprawnie obsługuje kopiowanie i wklejanie wartości, a wartość "max amount" jest aktualizowana poprawnie.
