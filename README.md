# C.N.B.P
Czyszczenie i normalizacja bazy produktów

## Cel
Ujednolicenie „brudnych” danych produktowych pochodzących z wielu źródeł (różne działy, różne formaty, skróty, błędy w nazwach).

## Problem
- nazwy zawierają gramatury, skróty, literówki
- te same produkty występują pod różnymi wariantami
- dane są w wielu arkuszach i nie trzymają jednego standardu

## Rozwiązanie (koncept)
Pipeline ETL w Pythonie:
1. import danych (CSV/XLSX)
2. czyszczenie tekstu (spacje, znaki, skróty)
3. ekstrakcja gramatur / jednostek
4. normalizacja nazw i kategorii
5. walidacja + raport błędów
6. zapis do PostgreSQL / pliku wynikowego

## Technologie
- Python
- Pandas
- (docelowo) PostgreSQL
- (opcjonalnie) reguły normalizacji + słowniki

## Efekt biznesowy
- mniej błędów w promocjach i opisach
- szybsza praca marketingu i działu danych
- jedno źródło prawdy dla produktu

## Status
W trakcie rozwoju — repo zawiera koncepcję i strukturę projektu.
