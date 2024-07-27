---
id: #EMAILDROP001
title: Sprawdź działanie rozwijanej listy adresów po kliknięciu w ikonkę "@" w polu input "Wysłać do"
description: Testy dotyczące działania rozwijanej listy adresów, otwierania i zamykania dropdowna, komunikatu o braku zapisanych adresów oraz poprawności nazw i komunikatów w różnych językach
test Scenario: Weryfikacja działania rozwijanej listy adresów, otwierania/zamykania dropdowna oraz komunikatów o braku zapisanych adresów
Test Steps:
  - Kliknij ikonę „@” w polu input „Wysłać do” i sprawdź działanie rozwijanej listy
  - Sprawdź, czy dropdown zamyka się po kliknięciu poza dropdownem
  - Sprawdź, czy wyświetlane są zapisane adresy
  - Sprawdź, czy wyświetlany jest komunikat „Brak zapisanych adresów” gdy lista jest pusta
  - Sprawdź poprawność nazw i komunikatów w różnych językach

Prerequisites: Strona z polem input „Wysłać do” i ikoną „@” jest dostępna, lista zapisanych adresów istnieje
Expected/Intended Results: Dropdown działa poprawnie, komunikat o braku zapisanych adresów jest wyświetlany w przypadku pustej listy, a komunikaty są poprawne w różnych językach
---

## Warunki wstępne
Strona z polem input „Wysłać do” i ikoną „@” jest dostępna, lista zapisanych adresów istnieje.

## Przypadek: 1a: Sprawdź otwieranie i zamykanie rozwijanej listy adresów

**Kroki testowe:**

- Otwórz stronę z polem input „Wysłać do”
- Kliknij ikonę „@” w tym polu
- Sprawdź, czy rozwijana lista adresów (dropdown) się otwiera
- Kliknij ikonę „@” ponownie
- Sprawdź, czy rozwijana lista adresów (dropdown) się zamyka

**Oczekiwany rezultat:**
Dropdown otwiera się po kliknięciu w ikonę „@” i zamyka się po ponownym kliknięciu.

## Przypadek: 1b: Sprawdź, czy dropdown zamyka się po kliknięciu poza dropdownem

**Kroki testowe:**

- Otwórz stronę z polem input „Wysłać do”
- Kliknij ikonę „@” w tym polu, aby otworzyć rozwijaną listę adresów
- Kliknij poza obszar rozwijanego dropdowna
- Sprawdź, czy dropdown się zamyka

**Oczekiwany rezultat:**
Dropdown zamyka się po kliknięciu poza jego obszar.

## Przypadek: 1c: Sprawdź wyświetlanie zapisanych adresów w dropdownie

**Kroki testowe:**

- Otwórz stronę z polem input „Wysłać do”
- Upewnij się, że istnieją zapisane adresy w systemie
- Kliknij ikonę „@” w polu input „Wysłać do”
- Sprawdź, czy zapisane adresy są poprawnie wyświetlane w rozwijanej liście

**Oczekiwany rezultat:**
Zapisane adresy są poprawnie wyświetlane w rozwijanej liście.

## Przypadek: 1d: Sprawdź komunikat „Brak zapisanych adresów” gdy lista jest pusta

**Kroki testowe:**

- Otwórz stronę z polem input „Wysłać do”
- Upewnij się, że nie ma zapisanych adresów w systemie
- Kliknij ikonę „@” w polu input „Wysłać do”
- Sprawdź, czy wyświetlany jest komunikat „Brak zapisanych adresów”

**Oczekiwany rezultat:**
Komunikat „Brak zapisanych adresów” jest wyświetlany, gdy lista adresów jest pusta.

## Przypadek: 1e: Sprawdź poprawność nazw i komunikatów w różnych językach

**Kroki testowe:**

- Otwórz stronę z polem input „Wysłać do”
- Ustaw język interfejsu na różne dostępne języki
- Kliknij ikonę „@” w polu input „Wysłać do”
- Sprawdź, czy nazwy adresów i komunikaty są poprawne w każdym języku

**Oczekiwany rezultat:**
Nazwy adresów i komunikaty są poprawne i zgodne z wybranym językiem interfejsu.
