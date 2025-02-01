# Projekt_PAD
Projekt zaliczeniowy przedmiotu PAD na PJATK

Opis struktury projektu:
Źródła danych:

Pliki csv, których źródłem są API (https://github.com/swar/nba_api) udostępniane przez NBA (National Basketball Association):
  - players,
  - playersinfo,
  - salaries,
  - stats_playoffs,
  - stats,
Plik csv tworzony ręcznie, przez export danych o kontraktach z https://www.espn.com/nba/salaries. Plik robots.txt - https://www.espn.com/robots.txt
  - salaries,
Plik csv, który https://github.com/gboogy/nba-injury-data-scraper:
  - injuries,
Plik csv tworzony ręcznie, przez różnice w imionach i nazwiskach pomiedzy źródłami
  - names_aliases.

Pliki ipynb:
  - nba_data_scraping - służy do tworzenia plików csv, zawierających dane z API !!!Uwaga na ponowny export danych z API NBA. Przez problemy z traffickiem, może on zająć pomiędzy 6h, a 30h.
  - data_cleaning - czyszczenie danych, analiza, modelowanie i dashboard. Wszystkie wnioski oraz operacje opisane w kodzie

Wersja pythona, na której pisany był kod: 3.11.9
Biblioteki:
time
pandas 2.2.2
numpy 1.26.4
re 2.2.1
requests 2.32.3
bs4
nba_api
os
datetime
openpyxl 3.1.5
matplotlib
wordcloud
seaborn 0.13.2
scipy
