---
id: #SENDTOKEN001
title: Sprawdź poprawność działania pola input "Send to"
description: Testy funkcji wysyłania tokenu dla pola input "Send to"
test Scenario: Weryfikacja działania pola input "Send to"
Test Steps:
  - Sprawdź, czy rozwija się dropdown z listą możliwych odbiorców
  - Sprawdź, czy pole input "Send to" przyjmuje tylko wartości typu string
  - Sprawdź, czy pole input "Send to" przyjmuje znaki specjalne
  - Sprawdź, czy pole input "Send to" akceptuje minimalną liczbę znaków
  - Sprawdź, czy pole input "Send to" akceptuje maksymalną liczbę znaków
  - Sprawdź, czy poprawnie wyświetla się komunikat o pustym polu
  - Sprawdź, czy poprawnie wyświetla się komunikat o przekroczeniu maksymalnej liczby znaków

Prerequisites: Strona z polem input "Send to" jest dostępna
Expected/Intended Results: Dropdown rozwija się poprawnie, pole input przyjmuje tylko stringi i obsługuje znaki specjalne
---

## Warunki wstępne
Strona z polem input "Send to" jest dostępna.

## Przypadek: 1b: Sprawdź, czy pole input "Send to" przyjmuje tylko wartości typu string

**Kroki testowe:**

- Wpisz wartość typu string (np. "NIGHTLY1") w pole input "Send to"
- Sprawdź, czy wartość jest zaakceptowana
- Wpisz wartość typu number (np. 12345) w pole input "Send to"
- Sprawdź, czy wartość jest odrzucona
- Wpisz wartość boolean (np. `true`) w pole input "Send to"
- Sprawdź, czy wartość jest odrzucona

**Oczekiwany rezultat:**
Pole input "Send to" akceptuje tylko wartości typu string, wartości typu number i boolean są odrzucane

## Przypadek: 1c: Sprawdź, czy pole input "Send to" przyjmuje znaki specjalne

**Kroki testowe:**

- Wpisz wartość zawierającą znaki specjalne (np. "Nightly_mm!@#") w pole input "Send to"
- Sprawdź, czy wartość jest zaakceptowana i poprawnie wyświetlona

**Oczekiwany rezultat:**
Pole input "Send to" akceptuje wartości zawierające znaki specjalne

## Przypadek: 2a: Sprawdź minimalną liczbę znaków w polu input "Send to"

**Kroki testowe:**

- Wpisz minimalną liczbę znaków (np. 1 znak) w pole input "Send to"
- Sprawdź, czy wartość jest zaakceptowana
- Wpisz wartość krótszą niż minimalna liczba znaków (np. 0 znaków) i sprawdź, czy jest odrzucona

**Oczekiwany rezultat:**
Pole input "Send to" akceptuje minimalną liczbę znaków, a wpisanie mniej niż minimalna liczba znaków powoduje wyświetlenie komunikatu o błędzie

## Przypadek: 2b: Sprawdź maksymalną liczbę znaków w polu input "Send to"

**Kroki testowe:**

- Wpisz maksymalną liczbę znaków (np. 255 znaków) w pole input "Send to"
- Sprawdź, czy wartość jest zaakceptowana
- Wpisz wartość dłuższą niż maksymalna liczba znaków (np. 256 znaków) i sprawdź, czy jest odrzucona

**Oczekiwany rezultat:**
Pole input "Send to" akceptuje maksymalną liczbę znaków, a wpisanie więcej niż maksymalna liczba znaków powoduje wyświetlenie komunikatu o błędzie

## Przypadek: 2c: Sprawdź komunikat o pustym polu

**Kroki testowe:**

- Pozostaw pole input "Send to" puste
- Spróbuj wysłać formularz lub przejść dalej
- Sprawdź, czy wyświetla się komunikat o błędzie "zły adres"

**Oczekiwany rezultat:**
Wyświetla się komunikat "zły adres"

## Przypadek: 2d: Sprawdź komunikat o przekroczeniu maksymalnej liczby znaków

**Kroki testowe:**

- Wpisz wartość dłuższą niż maksymalna liczba znaków (np. 256 znaków) w pole input "Send to"
- Spróbuj wysłać formularz lub przejść dalej
- Sprawdź, czy wyświetla się komunikat o błędzie informujący, że pole przekroczyło maksymalną liczbę znaków

**Oczekiwany rezultat:**
Wyświetla się komunikat informujący, że pole przekroczyło maksymalną liczbę znaków
