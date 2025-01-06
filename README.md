# Zadanie egzaminacyjne

Wykonaj aplikację będącą prototypem części front-end do chata, wykorzystując pakiet XAMPP, edytor grafiki rastrowej
oraz edytor zaznaczający składnię.

Do zadania dołączono archiwum ZIP o nazwie pliki zabezpieczone hasłem: `ChaT_Ch@t`

Archiwum należy rozpakować. Na pulpicie należy utworzyć folder. Jako nazwy folderu należy użyć numeru zdającego (jest to Twój
numer PESEL). Rozpakowane pliki należy umieścić w tym folderze. Po skończonej pracy wszystkie wyniki należy zapisać w
tym folderze.

## Operacje na bazie danych

***Rys. 1: Baza danych***\
![Baza danych](https://ckziu2.edu.pl/programista/arkusze/inf-03/praktyczny-05/obraz1.jpg)

Za pomocą narzędzia phpMyAdmin wykonaj operacje na bazie danych:

1.  Utwórz bazę danych o nazwie `chat`, z zestawem polskich znaków (np. `utf8_unicode_ci`)
2.  Do bazy zaimportuj tabele z pliku baza.sql z rozpakowanego archiwum
3.  Wykonaj zrzut ekranu po imporcie. Zrzut zapisz w formacie `PNG` i nazwij `import`. Nie kadruj zrzutu.
    Powinien on obejmować cały ekran monitora, z widocznym paskiem zadań. Na zrzucie powinny być
    widoczne elementy wskazujące na poprawnie wykonany import tabel.
4.  Wykonaj zapytania SQL działające na bazie `chat`. Zapytania zapisz w pliku `kwerendy.txt`. Wykonaj
    zrzuty ekranu przedstawiające wyniki działania kwerend. Zrzuty zapisz w formacie `JPEG` i nadaj im
    nazwy `kw1`, `kw2`, `kw3`, `kw4`, `kw5`. Zrzuty powinny obejmować cały ekran monitora z widocznym paskiem zadań.
   - **Zapytanie 1:** wstawiające do tabeli logowanie nick `Jeremi` z hasłem `Jer123`. Wstawianemu wierszowi
   należy nadać identyfikator, odpowiadający wartości klucza obcego dla wiersza z danymi `Jeremi
   Kowalski` z tabeli uczestnicy
   - **Zapytanie 2:** obliczające średni rok urodzenia uczestników. Wybrana kolumna powinna mieć nazwę (alias)
       `Średni rok urodzenia`, a obliczony wynik powinien być zaokrąglony w dół do liczby całkowitej
   - **Zapytanie 3:** wybierające jedynie imię i nazwisko uczestnika oraz odpowiadające mu nick
     i hasło dla imion rozpoczynających się literą `J`. Należy posłużyć się relacją
   - **Zapytanie 4:** tworzące użytkownika `uczestnik` na `localhost` z hasłem `Ucz123&`
   - **Zapytanie 5:** nadające utworzonemu użytkownikowi prawa do wybierania i aktualizacji danych
     jedynie dla tabeli uczestnicy

***Rys. 2: Witryna internetowa. Stan początkowy***\
![Obraz 2](https://ckziu2.edu.pl/programista/arkusze/inf-03/praktyczny-05/obraz2.jpg)

## Cechy grafiki

1. Grafika `Jolka.jpg` przygotowana, podobnie jak `Krzysiek.jpg`. Grafikę `Jolka.jpg` należy wykadrować do
   kwadratu tak, aby była widoczna tylko cała twarz. Następnie należy przeskalować dokładnie do
   rozmiaru `70px` na `70px`.

## Cechy witryny

1. Składa się ze strony o nazwie `chat.html` zapisanej w języku `HTML5` 
2. Ustawiony język zawartości strony na polski 
3. Jawnie zastosowany właściwy standard kodowania polskich znaków
4. Tytuł strony widoczny na karcie przeglądarki: `Chat` 
5. Arkusz stylów w pliku o nazwie `styl.css` prawidłowo połączony z kodem strony 
6. Podział strony na baner i pod nim blok główny, obok obu bloków blok boczny oraz na dole stopka.
   Podział zrealizowany wyłącznie za pomocą semantycznych znaczników sekcji języka HTML5 tak, aby
   po uruchomieniu w przeglądarce wygląd układu bloków był zgodny z rysunkiem 2 
7. Zawartość banera: nagłówek drugiego stopnia o treści `Chat` 
8. Zawartość bloku bocznego:
   - Nagłówek trzeciego stopnia o treści `Chaty`
   - Lista punktowana z elementami: `Ogólny` , `Tematyczne`. Drugi element zagnieżdża listę
     numerowaną z elementami `Turystyczny`, `Żeglarski`, `Filatelistyczny`, `Hodowla zwierzątek
     domowych`
   - Nagłówek trzeciego stopnia o treści `Uczestnicy`
   - Paragraf (akapit) o treści `Jolanta Nowak`
   - Obraz `Jolka.jpg` z tekstem alternatywnym `Jolanta Nowak`
   - Paragraf o treści `Krzysztof Łukasiński`
   - Obraz `Krzysiek.jpg` z tekstem alternatywnym `Krzysztof Łukasiński`
9. Zawartość bloku głównego:
   - Blok chatu zawierający:
     - Jeden blok z wypowiedzią Jolanty: Obraz `Jolka.jpg` i paragraf: `Cześć idziesz jutro do
       kina?`
     - Jeden blok z wypowiedzią Krzysztofa: Obraz `Krzysiek.jpg` i paragraf: `Tak! A ty?`
   - Obok siebie: napis `Wpisz wiadomość:`, pole edycyjne, przycisk o treści `Wyślij`. Kliknięcie
     przycisku powoduje wywołanie funkcji skryptu
   - Poniżej: przycisk o treści: `Generuj losową odpowiedź`. Kliknięcie przycisku powoduje
     wywołanie funkcji skryptu
10. Zawartość stopki: nagłówek piątego stopnia o treści: `Chat wykonał: `, dalej wstawiony numer
    zdającego.

## Styl CSS witryny internetowej

Styl CSS zdefiniowany jest w całości w zewnętrznym pliku o nazwie `styl.css`. Cechy formatowania CSS,
działające na stronie:
1. Domyślne formatowanie wszystkich selektorów: krój czcionki `Garamond`
2. Dla banera: kolor tła `Tomato`, biały kolor czcionki, wyrównanie tekstu do środka, szerokość `80%`,
   wysokość `80px`
3. Dla bloku głównego: szerokość `80%`, wysokość `600px`
4. Dla bloku bocznego: kolor tła `Coral`, szerokość `20%`, wysokość `680px`
5. Dla stopki: kolor tła `Tomato`, biały kolor czcionki, wyrównanie tekstu do środka
6. Dla selektora obrazu: zaokrąglenie rogów `50%`, marginesy wewnętrzne lewy i prawy `10px`
7. Dla bloku chatu: obramowanie linią ciągłą o szerokości `1px` i kolorze `Tomato`, marginesy zewnętrzne
   `15px`, wysokość `470px`, paski przewijania zawsze widoczne na stronie
8. Wspólne dla bloków z wypowiedziami: zaokrąglenie rogów `5px`, szerokość `90%`, wysokość `70px`,
   marginesy zewnętrzne `2%`, marginesy wewnętrzne `3px`
9. Dodatkowo dla bloków z wypowiedziami Jolanty: kolor tła `#EEE`, obraz opływany tekstem z prawej
   strony (obraz po lewej stronie)
10. Dodatkowo dla bloków z wypowiedziami Krzysztofa: kolor tła `#CCC`, wyrównanie tekstu do prawej
    strony, obraz opływany tekstem z lewej strony (obraz po prawej stronie)
11. Dla obu przycisków: kolor tła `Tomato`, obramowanie linią ciągłą o szerokości `1px` i kolorze `DarkRed`,
    marginesy wewnętrzne `5px`, czcionka pogrubiona
12. Dla pola edycyjnego tekstowego: szerokość `500px`

>***Uwaga: styl CSS obrazu należy zdefiniować wyłącznie przy pomocy selektora znacznika obrazu. Jest to
uwarunkowane projektem późniejszej rozbudowy witryny.***

## Skrypt

Wymagania dotyczące skryptu:
1. Napisany w języku JavaScript
2. Należy stosować znaczące nazewnictwo wszystkich zmiennych i funkcji
3. Działanie funkcji wywoływanej po kliknięciu przycisku `Wyślij`:
   - Pobierany jest tekst z pola edycyjnego i umieszczany w oknie chatu jako ostatni
   - Tekst jest formatowany jako wypowiedź Jolanty, zgodnie z rysunkiem 3, czyli utworzony jest blok
     z wypowiedzią zawierający obraz `Jolka.jpg` i paragraf zgodny z tekstem wpisanym do pola
     edycyjnego
   - Jeśli blok chatu jest cały wypełniony, powinien być przewinięty do nowo wstawionej wypowiedzi

***Rys. 3: Działanie funkcji wywoływanej kliknięciem przycisku Wyślij***\
![Obraz 3](https://ckziu2.edu.pl/programista/arkusze/inf-03/praktyczny-05/obraz3.jpg)

4. Działanie funkcji wywoływanej po kliknięciu przycisku `Generuj losową odpowiedź`
   - Losowana jest wypowiedź Krzysztofa z wcześniej zadeklarowanej tablicy. Tablica zawiera 9
     elementów, którymi są wypowiedzi. Należy je skopiować z pliku pomocniczego `tekstyDoChatu.txt`
     rozpakowanego z archiwum
   - Losowana liczba z przedziału od `0` do `8` jest indeksem tablicy
   - Wypowiedź jest umieszczana w oknie chatu jako ostatnia
   - Tekst jest formatowany jako wypowiedź Krzysztofa, zgodnie z obrazem 4, czyli utworzony jest
     blok z wypowiedzią zawierający obraz `Krzysiek.jpg` i paragraf zgodny z wylosowanym tekstem
   - Jeśli blok chatu jest cały wypełniony, powinien być przewinięty do nowo wstawionej wypowiedzi

***Rys. 4: Działanie funkcji wywoływanej kliknięciem przycisku Generuj...***\
![Obraz 3](https://ckziu2.edu.pl/programista/arkusze/inf-03/praktyczny-05/obraz4.jpg)

>***UWAGA: po zakończeniu pracy utwórz plik tekstowy o nazwie przeglądarka.txt. Zapisz w nim nazwę
> przeglądarki internetowej, w której weryfikowana była poprawność działania witryny. Umieść go w folderze
> z numerem zdającego. Do oceny prześlij pliki: `chat.html`, `import.png`, `Jolka.jpg`, `Krzysiek.jpg`, `kw1.jpg`,
> `kw2.jpg`, `kw3.jpg`,`kw4.jpg`, `kw5.jpg`,`kwerendy.txt`, `przeglądarka.txt`, `styl.css`,
> ewentualnie inne przygotowane pliki.***

### Ocenie będzie podlegać 5 rezultatów:
1. operacje na bazie danych,
2. zawartość witryny internetowej,
3. działanie witryny internetowej,
4. styl CSS witryny internetowej,
5. skrypt.