<h1 align= "center"> МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ РОССИЙСКОЙ ФЕДЕРАЦИИ ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ОБРАЗОВАНИЯ «САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»</h1>
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
<p align= "center">Лабораторная работа №7</p><br><br><br><br><br><br><br><br>
<p align= "right">Выполнил: Андреев Д.В.</p><br><br><br><br><br><br><br><br>
<p align="center">г. Южно-Сахалинск <br> 2023 год</p><br><br><br><br><br><br><br><br>
<h2 style="text-align: center">Введение</h2>
<p align="justify">JavaScript ("JS" для краткости) — это полноценный динамический язык программирования, который применяется к HTML документу, и может обеспечить динамическую интерактивность на веб-сайтах. Его разработал Brendan Eich, сооснователь проекта Mozilla, Mozilla Foundation и Mozilla Corporation. JavaScript сам по себе довольно компактный, но очень гибкий. Разработчиками написано большое количество инструментов поверх основного языка JavaScript, которые разблокируют огромное количество дополнительных функций с очень небольшим усилием. JavaScript невероятно универсален и дружелюбен к новичкам. Обладая большим опытом, вы сможете создавать игры, анимированную 2D и 3D графику, полномасштабные приложения с базами данных и многое другое!</p>
<h2 style="text-align: center">Цели и задачи</h2>
<ol align="justify"> <br>
<h2 align="center">Цели и задачи</h2>
Задачи:
1.	Сделайте alert по нажатию на кнопку.<br>
2.	Сделайте изменение текста в input по нажатию кнопки.<br>
3.	Сделайте вывод содержимого input по нажатию кнопки.<br>
4.	 Сделайте кнопку по нажатию на нее, она выводит alert содержимое input, возведенное в квадрат.<br>
5.	 Сделайте кнопку по нажатию, она осуществляет обмен содержимым между двумя input.<br>
6.	Сделайте кнопку по нажатию на нее поменяется ее текст.<br>
7.	Сделайте кнопку по нажатию на нее, она меняет цвет текста в input, используя свойства CSS.<br>
8.	Сделайте кнопки по нажатию на них, одна из них блокирует input с помощью атрибута disabled, а другая разблокирует.<br>
9.	Сделайте кнопку при наведении на нее появляется alert.<br>
10.	 Сделайте кнопку при двойном на нее появляется alert.<br>
11.	 Сделайте область с помощью div при наведении на нее появляется alert.<br>
12.	Сделайте кнопку и картинку, при нажатии кнопки картинка меняется.<br>
13.	Сделайте alert по нажатию на кнопку. Используя this.<br>
14.	Сделайте изменение текста в input по нажатию кнопки. Используя this.<br>
15.	Сделайте кнопку, при нажатии кнопки кнопка блокируется.<br>
16.	Сделайте кнопку, при нажатии кнопка считает количество нажатий на нее.<br>
17.	Сделайте кнопку, при нажатии курсор мышки должен измениться.<br>
18.	Используя JavaScript, сделайте так, чтобы при клике на кнопку исчезал элемент с id=&quot;hide&quot<br>
<!DOCTYPE HTML>
<html>
<head>
    <meta charset="utf-8">
</head>
<body>
    <input type="button" id="hider" value="Нажмите, чтобы спрятать текст"/>
    <div id="hide">Текст</div>
<script>
    /* ваш код */
</script>
</body>
</html>
19.	Создайте кнопку, при клике на которую, она будет скрывать сама себя.<br>
20.	Напишите простой калькулятор.<br>



Код на HTML
```html

<!DOCTYPE html>
<html>
 <head>
  <script src="lab6.js"></script>
  <title>Лабораторная №6</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
 
 </head>
 <body>
  
  <h1>Лабораторная №6</h1>
  <!-- Задание 1 -->
  <p>
    <button onclick="func1()">1 Задание</button>
</p>


  <!-- Задание 2 -->
  <p>
  
    <button onclick="func2()">2 Задание</button>
    <input type="text" id="myInput" value="ЕНОТ">
</p>

<!-- Задание 3 -->
<p>
  <button onclick="func3()">3 Задание</button>
  <input type="text" id="myyInput" value="БИБА">
</p>


<!-- Задание 4 -->
<p>
  <button onclick="func4()">4 Задание</button>
  <input type="number" id="myyInputt" value="3">
</p>


<!-- Задание 5 -->
<p>
  <button onclick="func5()">5 Задание</button>
  <input type="text" id="input51" value="БИБА">
  <input type="text" id="input52" value="БОБА">
</p>

<!-- Задание 6 -->
<p>
  <button onclick="this.innerHTML = 'Текст поменялся'">6 Задание</button>
</p>

<!-- Задание 7-->
<p>
  <button onclick="func7()">7 Задание</button>
  <input type="text" id="Inputs" value="asdadssadasdт">
</p>
<!-- Задание 8-->
<p>
  <button onclick="func8()">8 Задание</button>
  <button onclick="func88()">8 Задание</button>
  <input type="text" id="Innput" value="sddsasddas">
</p>

<!-- Задание 9-->
<p>
  <button onmouseover="alert('Вы навелись на кнопку')">9 Задание</button>
</p>

<!-- Задание 10-->
<p>
  <button ondblclick="alert('двойное нажатие')">10 Задание</button>
</p>
<style>
  .a {
   border: 2px double green; 
   background-color: rgb(98, 196, 69);
   width:130px;
  }
 </style>
<!-- Задание 11-->
<p>
  <div class="a" onmouseover="alert('Наведение ')">11 ЗАДАНИЕ</div>

</p>

<!-- Задание 12-->
<p>
  <button onclick="func12()">12 Задание</button><br>
  <img id="myImage" src="suzuki.jpeg" width="200" height="200">
</p>

<!-- Задание 13-->
<p>
  <button onclick="alert(this.innerHTML)">13 Задание</button>
</p>
<!-- Задание 14-->
<p>
  <input type="text" id="Inputqq" value="sdadadsa">
  <button onclick="this.previousElementSibling.value = 'Изменён'">14 Задание</button>
 
</p>
<!-- Задание 15-->
<p>
  <button onclick="this.disabled = true;">15 Задание</button>
</p>
<!-- Задание 16-->
<p>
  <button onclick="func16()">16 Задание</button>
<p id="clickCount">Количество нажатий: 0</p>
</p>

<!-- Задание 17-->
<p>
  <button onclick="this.style.cursor = 'pointer'">17 Задание</button>
</p>
<!-- Задание 18-->
<p>
 
  <button onclick="func18()">18 Задание</button>
  <p id="hide">id=hide</p>
</p>
<!-- Задание 19-->
<p>
 
  <button onclick="this.style.display = 'none'">19 Задание</button>
</p>

<!-- Задание 20-->
<p>
  <button onclick="func20()">20 Задание</button>
</p>

</body>
</html>
```
Код на JS
```JavaScript
function func1() {
  alert("Кнопка была нажата!");
}

function func2() {
  var input = document.getElementById('myInput');
  input.value = "Новый текст!";
}

function func3() {
  var input = document.getElementById('myyInput').value;
  alert(input);
}

function func4() {
  alert(Math.pow(document.getElementById('myyInputt').value, 2))
}

function func5() {
  var temp = document.getElementById('input51').value; 
  document.getElementById('input51').value = document.getElementById('input52').value; 
  document.getElementById('input52').value = temp;
}

function func6() {
  this.innerHTML = 'Текст кнопки поменялся';
}


function func7() {
  document.getElementById('Inputs').style.color = 'green'
}

function func8() {
  document.getElementById('Innput').disabled = true;
    }
    function func88() {
      document.getElementById('Innput').disabled = false;
        }


function func9() {
   
}


function func10() {
    
}


function func11() {
  
    }

    function func12() {
      document.getElementById('myImage').src = 'suz.jpg'
    }
    
    function func13() {
      
       }


function func14() {

}

function func15() {

}  
var clickCount = 0;
function func16() {

  clickCount++;
  document.getElementById("clickCount").innerHTML = "Количество нажатий: " + clickCount;
  }
  
    
function func17() {

}

function func18() {
  
    document.getElementById('hide').style.display = 'none';

}
function func19() {
const massive = [10, 5, 20, 8, 15, 30, 25, 12];

let minel = massive[0];
let maxel = massive[0];
let indexmin = 0;
let indexmax = 0;

for (let i = 1; i < massive.length; i++) {
  if (massive[i] < minel) {
    minel = massive[i];
    indexmin = i;
  }
  if (massive[i] > maxel) {
    maxel = massive[i];
    indexmax = i;
  }
}

const sumindex = indexmin + indexmax;

alert('Сумма номеров минимального и максимального элементов: ' + sumindex);
}

function func20() {
  
  function calculate(num1, operator, num2) {
    switch (operator) {
      case '+':
        return num1 + num2;
      case '-':
        return num1 - num2;
      case '*':
        return num1 * num2;
      case '/':
        if (num2 !== 0) {
          return num1 / num2;
        } else {
          return 'Ошибка: Деление на ноль невозможно!';
        }
      default:
        return 'Ошибка: Неверный оператор!';
    }
  }
  
  
  const number1 = parseFloat(prompt('Введите первое число:'));
  const operator = prompt('Введите оператор (+, -, *, /):');
  const number2 = parseFloat(prompt('Введите второе число:'));
  
  const result = calculate(number1, operator, number2);
  
  alert(`Результат: ${result}`);
}

function func21() {


}

function func22() {

}
```
  <h2 style="text-align: center">ВЫВОД</h2>
  JavaScript – это язык программирования, который добавляет интерактивность на ваш веб-сайт (например: игры, отклик при нажатии кнопок или при вводе данных в формы, динамические стили, анимация). 
 Разработчиками написано большое количество инструментов поверх основного языка JavaScript, которые разблокируют огромное количество дополнительных функций с очень небольшим усилием. JavaScript невероятно универсален и дружелюбен к новичкам. Обладая большим опытом, вы сможете создавать игры, анимированную 2D и 3D графику, полномасштабные приложения с базами данных и многое другое!
