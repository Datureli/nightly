---
id: #SENDTOKEN005
title: Sprawdź funkcjonalność przycisku "Next"
description: Testy przycisku "Next" przechodzącego do następnego etapu po wypełnieniu pól input "Send to" i "amount"
test Scenario: Weryfikacja działania przycisku "Next"
Test Steps:
  - Wypełnij pole "Send to"
  - Wypełnij pole "amount"
  - Kliknij przycisk "Next"
  - Sprawdź, czy użytkownik został przeniesiony do następnego etapu
Prerequisites: Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna
Expected/Intended Results: Po wypełnieniu pól i kliknięciu przycisku "Next" użytkownik zostaje przeniesiony do następnego etapu
---

## Przypadek: 5a: Sprawdź działanie przycisku "Next" przy poprawnym wypełnieniu pól

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź poprawne dane w pole "Send to" (np. recipient@example.com)
- Wprowadź poprawne dane w pole "amount" (np. 100)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik został przeniesiony do następnego etapu

**Oczekiwany rezultat:** Użytkownik zostaje przeniesiony do następnego etapu po kliknięciu przycisku "Next"

## Przypadek: 5b: Sprawdź działanie przycisku "Next" przy niepełnym wypełnieniu pól

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź poprawne dane w pole "Send to" (np. recipient@example.com)
- Pozostaw pole "amount" puste
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik nie został przeniesiony do następnego etapu i pojawia się komunikat o błędzie

**Oczekiwany rezultat:** Użytkownik nie zostaje przeniesiony do następnego etapu, pojawia się komunikat o konieczności wypełnienia wszystkich pól

## Przypadek: 5c: Sprawdź działanie przycisku "Next" przy wypełnieniu pól niepoprawnymi danymi

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź niepoprawne dane w pole "Send to" (np. invalid-email)
- Wprowadź poprawne dane w pole "amount" (np. 100)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik nie został przeniesiony do następnego etapu i pojawia się komunikat o błędzie

**Oczekiwany rezultat:** Użytkownik nie zostaje przeniesiony do następnego etapu, pojawia się komunikat o błędnych danych

## Przypadek: 5d: Sprawdź działanie przycisku "Next" przy wypełnieniu pola "Send to" znakami specjalnymi

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź dane w pole "Send to" zawierające znaki specjalne (np. recipient@ex@mple.com)
- Wprowadź poprawne dane w pole "amount" (np. 100)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik nie został przeniesiony do następnego etapu i pojawia się komunikat o błędzie

**Oczekiwany rezultat:** Użytkownik nie zostaje przeniesiony do następnego etapu, pojawia się komunikat o błędnych danych

## Przypadek: 5e: Sprawdź działanie przycisku "Next" przy wypełnieniu pola "amount" wartością ujemną

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź poprawne dane w pole "Send to" (np. recipient@example.com)
- Wprowadź wartość ujemną w pole "amount" (np. -100)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik nie został przeniesiony do następnego etapu i pojawia się komunikat o błędzie

**Oczekiwany rezultat:** Użytkownik nie zostaje przeniesiony do następnego etapu, pojawia się komunikat o błędnych danych

## Przypadek: 5f: Sprawdź działanie przycisku "Next" przy wypełnieniu pola "amount" wartością zmiennoprzecinkową

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź poprawne dane w pole "Send to" (np. recipient@example.com)
- Wprowadź wartość zmiennoprzecinkową w pole "amount" (np. 100.50)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik został przeniesiony do następnego etapu

**Oczekiwany rezultat:** Użytkownik zostaje przeniesiony do następnego etapu po kliknięciu przycisku "Next"

## Przypadek: 5g: Sprawdź działanie przycisku "Next" po usunięciu wprowadzonych danych

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź poprawne dane w pole "Send to" (np. recipient@example.com)
- Wprowadź poprawne dane w pole "amount" (np. 100)
- Usuń dane z pola "Send to" i "amount"
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik nie został przeniesiony do następnego etapu i pojawia się komunikat o błędzie

**Oczekiwany rezultat:** Użytkownik nie zostaje przeniesiony do następnego etapu, pojawia się komunikat o konieczności wypełnienia wszystkich pól

## Przypadek: 5h: Sprawdź działanie przycisku "Next" przy wypełnieniu pól z maksymalną ilością danych

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź dane w pole "Send to" z maksymalną ilością znaków (np. 255 znaków)
- Wprowadź dane w pole "amount" z maksymalną ilością cyfr (np. 9999999999)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik został przeniesiony do następnego etapu

**Oczekiwany rezultat:** Użytkownik zostaje przeniesiony do następnego etapu po kliknięciu przycisku "Next"

## Przypadek: 5i: Sprawdź działanie przycisku "Next" przy wypełnieniu pól z minimalną ilością danych

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź dane w pole "Send to" z minimalną ilością znaków (np. a@b.c)
- Wprowadź dane w pole "amount" z minimalną ilością cyfr (np. 1)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik został przeniesiony do następnego etapu

**Oczekiwany rezultat:** Użytkownik zostaje przeniesiony do następnego etapu po kliknięciu przycisku "Next"

## Przypadek: 5j: Sprawdź działanie przycisku "Next" przy wypełnieniu pól z danymi mieszanymi

**Warunek wstępny:** Strona z polami input "Send to" i "amount" oraz przyciskiem "Next" jest dostępna

**Kroki testowe:**

- Wprowadź dane w pole "Send to" z mieszanymi znakami (np. Recipient+Test@example.com)
- Wprowadź dane w pole "amount" z mieszanymi znakami (np. 100.00)
- Kliknij przycisk "Next"
- Sprawdź, czy użytkownik został przeniesiony do następnego etapu

**Oczekiwany rezultat:** Użytkownik zostaje przeniesiony do następnego etapu po kliknięciu przycisku "Next"