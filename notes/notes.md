DEKLAROWANIE ZMIENNEJ:

```JavaScript
const myVariable = 10; // zadeklarowanie i przypisanie zmiennej na stałe
```

```JavaScript
let counter = 0; // zadeklarowanie, a potem ponowne przypisanie zmiennej (gdy zmienna ma się zmieniać)
counter = counter + 1; // alternatywnie counter++
```

```JavaScript
var myVariable = 10; // nie używamy, ponieważ jest to przestarzałe rozwiązanie. Redeklaracja nie będzie w żaden sposób oznaczona, co może doprowadzić do pomyłki!
```


Nie można tworzyć zmiennych zaczynających się od numeru, np:

```JavaScript
const 1fullstack = 20; // zmienna taka natychmiast skończy się SyntaxError-em
```


Najbardziej preferowany styleguide dla języka JavaScript to camelcase (pierwsza litera mała, kolejne słowa oddzielone dużą literą):

```JavaScript
const yourFirstVariable = 10;
```


Zmienne powinny mieć bardzo jasne nazwy odpowiadające temu, co deklarują:

```JavaScript
const q = 10; // słaba nazwa zmiennej, nie wiadomo, co oznacza
const taxRateForNetIncome = 0.08; // dobra nazwa, natomiast należy pamiętać, aby nazy nie były zbyt długie
```


Można zapisać zmienne w jednej linii i jest to jak najbardziej poprawne:

```JavaScript
const oneVariable = 20; const secondVariable = 30;
```


Prymitywne typy zmiennych:

```JavaScript
const variable1 = 10; // zmienna liczbowa
const variable2 = "some value"; // zmienna "string"
const variable3 = false; // zmienna boolean (prawda / fałsz)
typeof variable1; // sprawdzenie typu zmiennej
```


Działania na typach zmiennych:

```JavaScript
const variable1 = '10'; // zmienna typu "string"
const variable2 = 20; // zmienna typu number
variable1 + variable2; // wynikiem tego działania będzie '1020', ponieważ JS najpierw zmienił 20 na string, a następnie połączył obie zmienne
Number(variable1) + variable2; // wynikiem tego działania będzie 30, ponieważ funkcja "Number()" zmieniła typ zmiennej z literowej na liczbową
```


Zmienna typu "string"

```JavaScript
const stringValue = 'hello world'; // bardziej poprawna konwencja to użycie pojedynczego cudzysłowu
const stringValue = "hello world"; // podwójny cudzysłów też zadziała, ale nie jest zgodny z konwencją
```


Zmienna typu "number":
```JavaScript
const numberValue = 2000;
```


Zmienna typu boolean (prawda / fałsz):

```JavaScript
const boolValueTrue = true;
const boolValueFals = false;
```


Zmienna typu array (zbiór, szyk, lista):

```JavaScript
const firstArray = [10, 20, 30, 40]; // dane oddzielone zawsze przecinkiem
const secondArray = [10, 'a string', { prop: 'abcdef' }, [1, 2]] // lista może zawierać różne elementy, w tym kolejną listę, obiekt i całą resztę zmiennych
```


Listy są indeksowane tak jak w Pythonie, czyli zaczyna się od 0.

```JavaScript
const firstArray = [10, 20, 30, 40];
console.log(firstArray[0]); // drukowanie w konsoli konkretnego indeksu
```


Gdy w jednej liście zagnieżdżona jest druga lista, możemy w ten sposób pobrać indeks głównej, a następnie zagnieżdżonej listy:

```JavaScript
const secondArray = [1, 2, 3, [4, 5]];
console.log(secondArray[3][1]); // pierwsza cyfra to wskazanie zagnieżdżonej listy, a druga to konkretny indeks w tej liście
```



