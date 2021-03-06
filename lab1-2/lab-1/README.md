Упражнение 1
=========

###Разгледани теми

- Организационни въпроси
- Процедурна, обектно-ориентирана, функционална, логическа парадигма, прилики и разлики между тях, добри и лоши страни на отделните парадигми.
- На какво ще пишем на упражнения (език и среда)
- Синтаксис на езика, на който ще пишем, неговите примитиви, средства за абстракция и комбинация, ще покажем и подкраме няколко примера
- задачи

###Организационни въпроси
- 2 контролни работи върху задачи за освобождаване от изпит
- за освобождаване - домашни работи; планът е след всяко упражнение да има по 1 домашно - трудност подобна на задачите в час
- предаване на задачите - по имейл.
- в края на семестъра - защита
- срокове за предаване - преди 2те контролни

###Процедурна парадигма
- позната от часовете по УП
- програма = множество от процедури, една начална/входна и множество извиквания помежду им, евентуално разделени в отделни файлове
- може да има процедури със странични ефекти
- императивен стил на програмиране
- примери за езици, в които е застъпена - С

###Обектно-ориентирана парадигма
- позната от часовете по УП / ООП
 основната програмна единица е класа. Класовете моделират някакви обекти от реалния свят или  домейна на проблема, който решаваме.
- всеки обект има поведение (множество от методи, които притежава) и състояние (множество от неговите полета)
- може да имаме методи със странични ефекти
- императивен стил на програмиране
- примери за езици, в които е застъпена - Java, C++, Python, Ruby, други

###Логическа парадигма
- ще се запознаете с нея на упражненията по Логическо Програмиране
 програмите са минималистични и представляват съвкупност от правила и факти
- фактите са някакви изначални твърдения, които е видимо, че са истина (дъно на рекурсия)
- правилата определят как от едно вярно твърдение да получим други верни твърдения (разгъване на рекурсията)
- декларативен стил на програмиране
- примери за езици, в които е застъпена - Prolog

###Функционална парадигма
- програмите са минималистични
- декларативен стил на програмиране
- програма = съвкупност от функции, в математическия смисъл на понятието
- всяка функция връща резултат и няма странични ефекти (чисто функционални езици)
- примери за езици, в които е застъпена - диалекти на Lisp - Scheme, Common Lisp; Haskell. Елементи в Javascript, Ruby, Python, други езици (ламбда изрази в Java 8, C#, F#)

###Функционална парадигма - специфики
- липса на странични ефекти; води до няколко неща:
    - от една страна неоптималност на изчисленията - многократни пресмятания на едни и същи функции, поради невъзможност за запазване на резултата
    - голяма полза при разработване на многонишкови приложения - решава основния проблем при разработка на такива приложения - необходимост от синхронизация при достъп до споделено състояние. Имаме липса на състояние (странични ефекти) => липса на необходимост от синхронизация
- обикновено във (чисто) функционалните езици няма оператори за цикъл - симулира се чрез рекурсия
- липсата на странични ефекти и декларативния стил ни карат да разбиваме задачата, която решаваме на подзадачи, за които да пишем отделни функции - добър код.

###Scheme / Racket
- на упражненията ще пишем на Racket и по-точно на неговата имплементация на R5RS стандарта на езика Scheme (диалект на Lisp)
- малко история на Scheme, R5RS, R7RS

###Примитивни типове и функции / процедури
- примитивни типове - числа, низове, символи, булеви стойности (атоми)
- примитивни процедури - вградени  езика - +, -, *, /, remainder, quotient, >, <, >=, <=, =, други
- s-изрази - атоми или точкови двойки от атоми (ще се запознаем по-натам)

###Средства за абстракция
- досадно (и признак за лошо качество на кода) е да пишем едно и също нещо няколко пъти
- специална форма define - дава ни начин за абстракция - може да дефинираме константи и функции, които ни дават общност

###Логически оператори
- if и cond - общ вид и пример с имплементация на (abs x);
- стойности, които се оценяват като истина и лъжа в Racket/Scheme, предикати

###Задачи
- да се проверят оценките на следните изрази: 3, 5, +, \*, (\* 5 5), (* 6 6), (+ 1 2 3 4 5 6), (/ 3 5)
- да се дефинират константи със зададени стойности
- да се напише функция пресмятаща |x| посредством if и cond
- да се напише функция пресмятаща x <sup>2</sup>
- да се напише функция пресмятаща x <sup>3</sup>
- да се напишат функции min(x,y) и max(x,y) като се използва:
    - if
    - формулата min(x,y) = (x + y - |x - y| ) / 2 ; max(x,y) = (x + y + |x - y|) / 2
- да се напишат предикати, проверяващи дали едно число е четно или нечетно, положително или отрицателно

