# Metody Inżynierii Wiedzy

## Zadanie 1

1. Pobierz z repozytorium UCI następujące zbiory danych:
  * Australian
  * Credit Approval
  * Breast Cancer Wisconsin
2. Zaproponuj sposób przechowywania danych w programie (skorzystaj z wbudowanych typów danych lub stwórz własne). Zwróć uwagę, na rodzaj danych (numeryczne, symboliczne).
3. Napisz program, który w oparciu o zaproponowane rozwiązanie z punktu 2, wczyta dane z pobranych wcześniej zbiorów danych.
4. Stwórz mechanizm normalizujący dane.
5. Zaimplementuj kilka sposobów (minimum 3) zapisu wczytanych danych, które będą różniły się od formatu, w którym aktualnie znajduje się repozytorium.
6. Na podstawie zebranych doświadczeń stwórz plik konfiguracyjny do wymienionych wcześniej zbiorów danych. Plik powinien zawierać wszystkie ustawienia i parametry opisujące dane repozytorium, np. typ, liczba, zakres atrybutu, itp. Na podstawie pliku konfiguracyjnego program powinien sprawdzić poprawność wczytanych dany i poinformować użytkownika o ewentualnych  niezgodnościach.
7. Dla chętnych. Spróbuj napisać mechanizm tworzący plik konfiguracyjny. System miałby wykrywać niektóre parametry zbioru danych, aby tworzenie pliku konfiguracyjnego było szybsze.

## Zadanie 2

Napisz program, który sklasyfikuje jeden podany przez użytkownika obiekt (próbka testowa). Klasyfikację należy wybrać w dwóch wariantach na podstawie datasetów z poprzednich zajęć.
* Sprawdzenie czy podane k jest dozwolone
* mierzyć odległości za pomocą metryki między dwoma obiektami

Co jest potrzebne żeby sklasyfikować jeden obiekt (próbkę testową)?
1. próbka testowa (obiekt) - lista
3. próbki wzorcowe
4. parametr k
5. metryka

## Zadanie 3

1. Wygenerować odpowiednią ilosc losowych danych z zadanego zakresu na podstawie struktury, np.: `3 - 2 - 2`, `4 - 3 - 2 - 3 - 10`
  * Dane zapisac w taki sposób, aby nie stracić informacji o strukturze.
  * Odczytac dane z pliku.
2. Funkcjonalności z zadania 1b
  * generowanie wag dla wskazanej struktury
  * zapisywanie wag do pliku (z podaniem nazwy, aby można było zapisać więcej niż jeden plik)
  * odczytanie wag z plików wcześniej zapisanych
3. Możliwość zadawania pytań do sieci
  * bezpośrednio w interfejsie użytkownika
  * po przez plik
4. Podawanie próbek uczących próbka ucząca, to zestaw wejść i wyjść liczebnie zależny od struktury). Proponuje podawać je w pliku, gdyż próbek uczących w zależności od struktury sieci może być bardzo dużo.
  * próbki uczące do uczenia się muszą być podawane w sposób losowy
5. Ustawianie parametrów uczenia się
  * B - beta (można na sztywno)
  * mi - współczynnik uczenia się (można na sztywno)
6. Warunki stopu uczenia się przez propagację wsteczną (oba muszą być zaimplementowane, użytkownik wybiera, którego chce użyć)
  * Zatrzymanie uczenia, po przekroczeniu założonej liczby iteracji (ile razy powtarzamy propagację wsteczną)
  * Zatrzymanie uczenia, po osiągnięciu błędu sieci mniejszego niż założony (błąd powinien być liczony jako średnia z ostatnich wyników, najlepiej liczba wyników jako parametr do ustalenia)
  * Możliwość zapisu wag po procesie uczenia
