---
id: #AMOUNTINPUT001  
title: Sprawdź działanie przycisku „Maks”  
description: Testy działania przycisku „Maks”, który powinien zwiększyć kwotę o maksymalną wartość dostępną na koncie  
test Scenario: Weryfikacja działania przycisku „Maks” w różnych scenariuszach związanych z saldem na koncie  
Test Steps:

- Sprawdzenie działania przycisku „Maks” przy różnych wartościach salda na koncie  
- Weryfikacja zachowania aplikacji w przypadku braku salda  

Prerequisites: Konto użytkownika jest aktywne i aplikacja jest zalogowana  
Expected/Intended Results: Przycisk „Maks” działa zgodnie z oczekiwaniami, a kwota jest ustawiana prawidłowo w zależności od salda na koncie  

---

## Warunki wstępne
Konto użytkownika jest aktywne, aplikacja jest zalogowana, a saldo na koncie jest ustawione na różne wartości w celu testowania funkcjonalności przycisku „Maks”.

## Przypadek: 1a: Sprawdź działanie przycisku „Maks” gdy saldo wynosi więcej niż 0

**Kroki testowe:**

- Zaloguj się do aplikacji  
- Ustaw saldo na koncie na wartość większą niż 0 (np. 1000 PLN)  
- Wprowadź jakąś wartość w polu kwoty  
- Kliknij przycisk „Maks”  
- Sprawdź, czy kwota w polu została ustawiona na wartość równą saldu na koncie (w tym przypadku 1000 PLN)  

**Oczekiwany rezultat:**
Kwota w polu powinna być równa maksymalnemu saldu na koncie (1000 PLN)

## Przypadek: 1b: Sprawdź działanie przycisku „Maks” gdy saldo wynosi 0

**Kroki testowe:**

- Zaloguj się do aplikacji  
- Ustaw saldo na koncie na 0 PLN  
- Wprowadź jakąś wartość w polu kwoty  
- Kliknij przycisk „Maks”  
- Sprawdź, czy kwota w polu pozostała taka sama, jak przed kliknięciem  

**Oczekiwany rezultat:**
Kwota w polu powinna pozostać taka sama, jak była przed kliknięciem

## Przypadek: 1c: Sprawdź działanie przycisku „Maks” gdy konto jest puste

**Kroki testowe:**

- Zaloguj się do aplikacji  
- Upewnij się, że saldo na koncie jest puste  
- Wprowadź jakąś wartość w polu kwoty  
- Kliknij przycisk „Maks”  
- Sprawdź, czy aplikacja wyświetla komunikat o braku salda lub zachowuje się w sposób oczekiwany  

**Oczekiwany rezultat:**
Kwota w polu powinna pozostać taka sama, jak była przed kliknięciem, a aplikacja powinna wyświetlić komunikat informujący o braku salda lub być gotowa na dalsze akcje użytkownika

## Przypadek: 1d: Sprawdź, jak zmiana salda wpływa na działanie przycisku „Maks”

**Kroki testowe:**

- Zaloguj się do aplikacji  
- Ustaw saldo na koncie na pewną wartość (np. 500 PLN)  
- Kliknij przycisk „Maks” i sprawdź, czy kwota w polu jest równa 500 PLN  
- Zmień saldo na koncie na inną wartość (np. 1000 PLN)  
- Kliknij przycisk „Maks” ponownie  
- Sprawdź, czy kwota w polu została zaktualizowana na nowe saldo (1000 PLN)  

**Oczekiwany rezultat:**
Kwota w polu powinna być równa nowemu maksymalnemu saldu na koncie (1000 PLN)
