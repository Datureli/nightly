---
id: #SENDTOKEN002
title: Sprawdź, czy pole input "Send to" obsługuje znaki z różnych języków
description: Testy funkcji wysyłania tokenu z uwagi na obsługę znaków z różnych języków i alfabetów w polu input "Send to"
test Scenario: Weryfikacja obsługi znaków z różnych języków
Test Steps:
  - Wprowadź tekst w cyrylicy (np. "тестовый текст") do pola input "Send to"
  - Wprowadź tekst w języku chińskim (np. "测试文本") do pola input "Send to"
  - Wprowadź tekst w innych językach i alfabetach (np. arabski, japoński) do pola input "Send to"

Prerequisites: Strona z polem input "Send to" jest dostępna
Expected/Intended Results: Pole input poprawnie akceptuje i wyświetla znaki z różnych języków
---

## Warunki wstępne
Strona z polem input "Send to" jest dostępna.

## Przypadek: 5a: Sprawdź obsługę tekstu w cyrylicy

**Kroki testowe:**

- Wprowadź tekst w cyrylicy (np. "тестовый текст") do pola input "Send to"
- Sprawdź, czy tekst jest poprawnie akceptowany i wyświetlany

**Oczekiwany rezultat:**
Tekst w cyrylicy jest poprawnie akceptowany i wyświetlany w polu input "Send to"

## Przypadek: 5b: Sprawdź obsługę tekstu w języku chińskim

**Kroki testowe:**

- Wprowadź tekst w języku chińskim (np. "测试文本") do pola input "Send to"
- Sprawdź, czy tekst jest poprawnie akceptowany i wyświetlany

**Oczekiwany rezultat:**
Tekst w języku chińskim jest poprawnie akceptowany i wyświetlany w polu input "Send to"

## Przypadek: 5c: Sprawdź obsługę tekstu w innych językach i alfabetach

**Kroki testowe:**

- Wprowadź tekst w języku arabskim (np. "نص تجريبي") do pola input "Send to"
- Sprawdź, czy tekst jest poprawnie akceptowany i wyświetlany
- Wprowadź tekst w języku japońskim (np. "テストテキスト") do pola input "Send to"
- Sprawdź, czy tekst jest poprawnie akceptowany i wyświetlany

**Oczekiwany rezultat:**
Tekst w innych językach i alfabetach (arabskim, japońskim itp.) jest poprawnie akceptowany i wyświetlany w polu input "Send to"
