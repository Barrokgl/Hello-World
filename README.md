При помощи цикла for выведите чётные числа от 2 до 10.

```javascript
for (var i = 2; i <= 10; i++){
	if (i % 2== 0){
	alert (i);
	}
}
```
------
Напишите if..else, соответствующий следующему switch:

switch (browser) {
  case 'IE':
    alert( 'О, да у вас IE!' );
    break;

  case 'Chrome':
  case 'Firefox':
  case 'Safari':
  case 'Opera':
    alert( 'Да, и эти браузеры мы поддерживаем' );
    break;

  default:
    alert( 'Мы надеемся, что и в вашем браузере все ок!' );
}



if(browser == "IE") {
	alert ("о,у вас IE!");
} else if (browser == "Chrome")
|| browser == 'Fierfox'
|| browser == 'Safari'
|| browser == 'Opera'){
	alerrt('да,мы поддерживаем и их');
} else {
	alert("мы надеемся что у вас все ок!")
}

-----------

Следующая функция возвращает true, если параметр age больше 18. В ином случае она задаёт вопрос confirm и возвращает его результат.

function checkAge(age) {
  if (age > 18) {
    return true;
  } else {
    return confirm('Родители разрешили?');
  }
}
Перепишите функцию, чтобы она делала то же самое, но без if, в одну строку. Сделайте два варианта функции checkAge:

Используя оператор '?'
Используя оператор ||



function checkAge(age) {
  return (age > 18) ? true : confirm('Родители разрешили?');
}



function checkAge(age) {
	return (age > 18) || confirm("Родители разрешили?");
}


----------
Задача «Hello World» для функций :)

Напишите функцию min(a,b), которая возвращает меньшее из чисел a,b.

Пример вызовов:

min(2, 5) == 2
min(3, -1) == -1
min(1, 1) == 1


function min(a, b) {
  if (a < b) {
    return a;
  } else {
    return b;
  }
}


с использованием "?"

function min(a, b) {
  return a < b ? a : b;
}


-----------
  Напишите функцию pow(x,n), которая возвращает x в степени n. Иначе говоря, умножает x на себя n раз и возвращает результат.

pow(3, 2) = 3 * 3 = 9
pow(3, 3) = 3 * 3 * 3 = 27
pow(1, 100) = 1 * 1 * ...*1 = 1
Создайте страницу, которая запрашивает x и n, а затем выводит результат pow(x,n).


function pow(x, n) {
  var result = x;
     for(var i = 1;i<n ; i++) {
     result *=x;
     }

     return  result;
     }
     var x = prompt("x?", '');
var n = prompt("n?", '');

if (n <= 1) {
  alert('Степень ' + n +
    'не поддерживается, введите целую степень, большую 1'
  );
} else {
  alert( pow(x, n) );
}
--------------



Создайте функцию isEmpty(obj), которая возвращает true, если в объекте нет свойств и false – если хоть одно свойство есть.

Работать должно так:

function isEmpty(obj) {
  /* ваш код */
}

var schedule = {};

alert( isEmpty(schedule) ); // true

schedule["8:30"] = "подъём";

alert( isEmpty(schedule) ); // false





function isEmpty(obj){
	for(var key in obj){
	return false;
	}
	return true;
}

var schedule = {;
alert( isEmpty(schedule) );
schedule["8:30"] = "подъём";
alert( isEmpty(schedule) );
