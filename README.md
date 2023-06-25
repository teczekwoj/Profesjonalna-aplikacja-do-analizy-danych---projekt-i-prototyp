# Specyfikacja aplikacji do analizy danych uderzeń meteorytów w Ziemię.  

## 1. Wymagania biznesowe
1.1 **Opis projektu**
Celem projektu jest stworzenie aplikacji webowej do analizy danych uderzeń wszytkich zidentyfikowanych przez NASA obiektów w Ziemię. Aplilacja ma w czytelny, przystępny i nowoczesny sposób prezentować dane na temat obiektów, pokazywać statystyki i wizualizacje na podstawie zbioru danych dostarczonego przez organizacje NASA.

1.2 **Najważniejsze cele projektu**  
- Interaktywna aplikacja webowa w formie panelu (dashboardu)
- Dane źródłowe w formacie .csv
- Aplikacja w jasny i czytelny sposób ma przedstawiać statystyki i wizualizacje na temat uderzeń obiektów w Ziemię
- Celem analizy jest zauważenie zależności lub trendu wśród meteorytów
- Podstawowe metody statystyczne wykorzystane w projekcie to: średnia, mediana, liczba elementów zbioru, warości max i min, dominanta, wariancja, odchylenie standardowe, histogram, wykresy słupkowe, wykresy kołowe itp.

1.3 **Źródła danych**  
Źródłem danych jest portal organizacji kosmicznej NASA's Open Data Portal (https://data.nasa.gov/Space-Science/Meteorite-Landings/gh4g-9sfh).
Dane pozyskane z tego portalu są kompletne, sprawdzone i ogólnodostępne co czyni je gotowymi do analizy.

1.4 **Harmonogram projektu**  
Analiza wymagań - 2 tygodnie  
Projektowanie systemu - 4 tygodnie  
Implementacja systemu - 12 tygodni  
Testowanie i wdrożenie - 4 tygodnie  
Utrzymanie i aktualizacja - stały proces  

## 2. Wymagania dotyczące danych i ich jakości  
2.1 **Źródła danych**  
- Dane są przechowywane w pliku .csv  
- Stan danych  jest aktualizowany co parę miesięcy i zależy on od wolonaryjnej chęci pracowników NASA  
- Jakość tych danych jest sprawdzona, dane są prawidłowo zmodelowane i ustrukturyzowane  
- Organizajcą odpowiedzialną za poprawność tych danych jest NASA Open Data Portal, dane są udostępnianie publicznie na postawie licencji Open Source
- Aktualnie zestaw danych ma 47,7 tyś. unikalnych wierszy i 10 kolumn. Każdy z wierszy to pojedyńcze uderzenie obiektu w Ziemię.
- Dane te z czasem będą się powiększać, ponieważ obiekty ciągle uderzeją w Ziemie.  

2.2 **Oczyszczanie danych**
Dane źródłowe bedą miały jednolity charakter i formę. Będą podzielone na 10 kolumn o różnych typach danych:
- name (text) 
- id (text)
- nametype (text)
- recclass (text)
- mass g (num)
- fall (text)
- year (DateTime)
- reclat (text)
- reclong (text)
- GeoLocation (location)
