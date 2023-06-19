Autor: Oskar Sroka
Data: 19.06.2023
Generator ASCIIGRAPHIC 

Prosty generator ASCIIGRAPHIC, który czyta plik konfiguracyjny zawierający informacje o rozmiarze płótna, nazwie pliku wynikowego oraz figurach do narysowania. Program obsługuje rysowanie prostokątów (w tym również kwadratów) i okręgów na płótnie.

Jak używać
- Pobierz kod źródłowy i przejdź do katalogu projektu.
- Skompiluj kod za pomocą komendy: g++ main.cpp -o ascii_art
- Utwórz plik konfiguracyjny o następującym formacie:

- <szerokość_płótna> <wysokość_płótna> <nazwa_pliku_wynikowego> <symbol_pustego_miejsca>
- <typ_figury> <dane_figury>
- <typ_figury> <dane_figury>
...


Opis konfiguracji

- <szerokość_płótna> i <wysokość_płótna> określają wymiary płótna w znakach.
- <nazwa_pliku_wynikowego> to nazwa pliku, w którym zostanie zapisany ASCII Art.
- <symbol_pustego_miejsca> to symbol używany do reprezentacji pustych miejsc na płótnie.
- <typ_figury> może być "Kwadrat", "Prostokąt" lub "Okrąg".
- <dane_figury> zależą od typu figury:
- Dla kwadratu: <x> <y> <rozmiar> <symbol> (współrzędne lewego górnego rogu, rozmiar i symbol)
- Dla prostokąta: <x> <y> <szerokość> <wysokość> <symbol> (współrzędne lewego górnego rogu, szerokość, wysokość i symbol)
- Dla okręgu: <środek_x> <środek_y> <promień> <symbol> (współrzędne środka, promień i symbol)
- Każda figura powinna być umieszczona w nowej linii.
- Uruchom program, podając ścieżkę do pliku konfiguracyjnego jako argument wiersza poleceń: ./ascii_art <plik_konfiguracyjny>
- <plik_konfiguracyjny> to ścieżka do pliku konfiguracyjnego utworzonego we wcześniejszym kroku.
- ASCII Art zostanie wygenerowany i zapisany w określonym pliku wynikowym. Program wyświetli wiadomość wskazującą lokalizację zapisanego pliku.
