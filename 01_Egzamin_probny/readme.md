![Coders-Lab-1920px-no-background](https://user-images.githubusercontent.com/152855/73064373-5ed69780-3ea1-11ea-8a71-3d370a5e7dd8.png)

# Kilka ważnych informacji

Przed przystąpieniem do rozwiązywania zadań przeczytaj poniższe wskazówki

## Jak zacząć?

1. Stwórz [*fork*](https://guides.github.com/activities/forking/) repozytorium z zadaniami.
2. Sklonuj repozytorium na swój komputer. Użyj do tego komendy `git clone adres_repozytorium`
Adres repozytorium możesz znaleźć na stronie repozytorium po naciśnięciu w guzik "Clone or download".
3. Rozwiąż zadania i skomituj zmiany do swojego repozytorium. Użyj do tego komend `git add nazwa_pliku`.
Jeżeli chcesz dodać wszystkie zmienione pliki użyj `git add .` 
Pamiętaj że kropka na końcu jest ważna!
Następnie skommituj zmiany komendą `git commit -m "nazwa_commita"`
4. Wypchnij zmiany do swojego repozytorium na GitHubie.  Użyj do tego komendy `git push origin master`
5. Stwórz [*pull request*](https://help.github.com/articles/creating-a-pull-request) do oryginalnego repozytorium, gdy skończysz wszystkie zadania.

Poszczególne zadania rozwiązuj w odpowiednich plikach.

# Poniżej znajdziesz wytyczne do zadań

## Zadanie 1

Napisz funkcję o nazwie ```getSqrt(n)```, która przyjmuje jako parametr jedną liczbę. Niech funkcja ta zwraca pierwiastek tej liczby. 

Przykład:

```JavaScript
getSqrt(4); // zwróci 2
getSqrt(16); // zwróci 4
```


## Zadanie 2

Napisz funkcję o nazwie ```mergeArrays(array1, array2)```, która przyjmuje jako parametry dwie tablice. Niech funkcja ta zwraca nową tablicę będącą połączeniem tych dwóch.

Przykład:

```JavaScript
mergeArrays([1,3], [3,5]); // zwróci [1, 3, 3, 5]
```


## Zadanie 3

Napisz funkcję ```biggestSumOfTwoElements(array)```, która przyjmuje tablicę z liczbami i **zwraca** sumę dwóch największych elementów z tej tablicy.
Dla uproszczenia możemy założyć, że przekazana tablica zawiera wyłącznie liczby.

* Jeżeli tablica zawiera tylko jeden element, funkcja powinna zwrócić wartość tego elementu.
* Jeżeli tablica zawiera zero elementów, funkcja powinna zwrócić wartość logiczną```false```.

Przykład:
```Javascript
biggestSumOfTwoElements([1,2,3,4]); // => 7
biggestSumOfTwoElements([]); // => false
biggestSumOfTwoElements([76]); // => 76
biggestSumOfTwoElements([23,45,17,12]); // => 68
```


## Zadanie 4
  
> Do każdego podpunktu stwórz odpowiednią funkcję o nazwie podanej w treści zadania.  
> Każda funkcja niech **zwraca** tablicę wypełnioną odpowiednimi elementami.


Wykonaj następujące polecenia:

### 1. Szukanie nazw tagów
- znajdź wszystkie elementy o **klasie** ```sample_class```,
- stwórz funkcję ```getTag(elements)``` do której przekaż jako argument znalezione elementy,
- stwórz w funkcji tablicę i wypełnij ją nazwami tagów. Pobierz je z elementów przekazanych jako argument.
- zwróć tablicę.

> Tablica powinna składać się z 10 elementów: "DIV", "LI", "P", "DIV", "LI", "LI", "ARTICLE", "H2", "H2", "DIV"


### 2. Szukanie nazw klas
- Znajdź element o **id** ```sample_id```.
- stwórz funkcję ```getClass(element)``` do której przekaż jako argument znaleziony element.
- stwórz w funkcji tablicę (nie pseuodotablice!) i wypełnij ją nazwami klas. Pobierz klasy z przekazanego jako argument elementu.
- zwróć tablicę.

> Tablica powinna składać się z 2 elementów: "sample_class", "sample_class_3"


### 3. Szukanie tekstu
- Znajdź wszystkie elementy __listy__ znajdujące się w elemencie o **klasie** ```sample_class_2```,
- stwórz funkcję ```getInnerText(elements)```, do której przekaż jako argument znalezione elementy.
- stwórz w funkcji tablicę i wypełnij ją tekstami pobranymi z elementów przekazanych jako argument.
- zwróć tablicę.

> Tablica powinna składać się z 4 elementów: "Test 3", "Marshmallow pastry gummies powder. Cake sweet roll sweet. Tart sweet lemon drops donut croissant.", "Lorem ipsum dolor sit amet, consectetur adipisicin…aspernatur enim harum nihil ratione voluptatibus.", "Test 2"


### 4. Szukanie adresów linków
- Znajdź wszystkie linki,
- stwórz funkcję ```getAddress(elements)```, do której przekaż jako argument znalezione elementy.
- stwórz w funkcji tablicę i wypełnij ją adresami pobranymi z elementów przekazanych jako argument.
- zwróć tablicę.

> Tablica powinna składać się z 4 elementów: "https://google.com/", "https://yahoo.com/", "https://onet.com/", "https://coderslab.pl/"


### 5. Szukanie tagów dzieci
- Znajdź wszystkie bezpośrednie dzieci elementu o **klasie** ```sample_class_3```,
- do funkcji, która wyszukuje tagi elementów, przekaż jako argument, znalezione dzieci.
  
> Tablica powinna składać się z 5 elementów: "DIV", "DIV", "UL", "ARTICLE", "DIV"
## Zadanie 5

Do wszystkich przycisków znajdujących się na stronie dopisz event tak, aby po naciśnięciu któregokolwiek przycisku  w  **divie** o klasie `.alert` pojawił się tekst trzymany w `data-text` danego przycisku.
## Zadanie 6

Na stronie znajduje się lista zakupów. Popatrz na HTML i zobacz jak lista jest zbudowana. Dopisz odpowiednią obsługę eventów tak, aby:

- Po kliknięciu przycisku pierwszego do listy został dopisany nowy produkt - ```Chleb```.

- Po kliknięciu przycisku drugiego z listy był usuwany ostatni element. Jeżeli nie ma czego usunąć (lista jest pusta) powinna pojawić się taka informacja w konsoli: "Lista jest pusta".

- Po kliknięciu przycisku trzeciego na końcu listy był dodawany nowy produkt, który jest klonem drugiego produktu. Jeżeli na liście jest tylko jeden lub mniej produktów, w konsoli powinna pojawić się informacja: "Lista zawiera jeden lub mniej produktów".
---

Repozytorium z ćwiczeniami zostanie usunięte 2 tygodnie po zakończeniu kursu. Spowoduje to też usunięcie wszystkich forków, które są zrobione z tego repozytorium.
