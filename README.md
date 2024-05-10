[![Build status](https://ci.appveyor.com/api/projects/status/wi4fusp6c2f0wqfs?svg=true)](https://ci.appveyor.com/project/Nephedov/cardorder)

# «Тестирование веб-интерфейсов»

## Решение
* <a href="https://github.com/Nephedov/4.Automated-Testing/blob/main/src/test/java/ru/netology/CardOrderTest.java">CardOrderTest.java</a> - класс с функциональными тестами отправки формы, с использованием WebDriver и Selenium.
## Что было сделано
* Настроен <a href="https://github.com/Nephedov/4.Automated-Testing/blob/main/build.gradle">build.gradle</a> с зависимостями:
  * JunitJupier.
  * Selenide.
  * WebDriverManager.
* Подключен к проекту AppVeyor. Настроен <a href="https://github.com/Nephedov/4.Automated-Testing/blob/main/.appveyor.yml">appveyor.yml</a>. Добавлен бейдж в README.md, о статусе сборки при пуше.
* Реализованы функциональные автотесты формы заявки карты в классе
  <a href="https://github.com/Nephedov/4.Automated-Testing/blob/main/src/test/java/ru/netology/CardOrderTest.java">CardOrderTest.java</a>.

---
---


## Описание Задания №1: заказ карты

Вам необходимо автоматизировать тестирование формы заказа карты:

![](pic/order.png)

Требования к содержимому полей:
1. В поле фамилии и имени разрешены только русские буквы, дефисы и пробелы.
2. В поле телефона — только 11 цифр, символ + на первом месте.
3. Флажок согласия должен быть выставлен.

Тестируемая функциональность: отправка формы.

Условия: если все поля заполнены корректно, то вы получаете сообщение об успешно отправленной заявке:

![](pic/success.jpg)

## Описание Задания №2: проверка валидации (необязательная)

Тестируемая функциональность: валидация полей перед отправкой.

Условия: если какое-то поле не заполнено или заполнено неверно, то при нажатии на кнопку «Продолжить» должны появляться сообщения об ошибке. Будет подсвечено только первое неправильно заполненное поле:

![](pic/error.png)
