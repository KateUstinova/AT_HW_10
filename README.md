# Домашнее задание к занятию «Заключительная лекция»

## План тестирования (Устинова Екатерина QA-40) 

### Переход на страницу записи на обучение профессии «Тестировщик ПО»

#### Способ № 1

1) Перейти на страницу сайта [Нетологии](https://netology.ru/)
2) В шапке сайта кликнуть на кнопку **"Каталог курсов"**
3) В левом меню выбрать **"Программирование"**, затем в **"Списке для начинающих"** выбрать профессию **"Тестировщик ПО"**

#### Способ № 2

1) Перейти на страницу сайта [Нетологии](https://netology.ru/)
2) В разделе **"Направления обучения"** выбрать **"355 курсов всех направлений"**
3) На появившейся странице выбрать профессию **"Тестировщик ПО"** или воспользоваться строкой поиска **"Чему вы хотите научиться"**, вписав в данную строку слово **"Тестировщик"** и затем выбрав профессию **"Тестировщик ПО"**

#### Способ № 3

1) Перейти на страницу сайта [Нетологии](https://netology.ru/)
2) На главной странице "Нетологии" долистать до раздела **"Выберите вектор развития"** и выбрать **"Выбрать курс ->"**
3) На появившейся странице выбрать профессию **"Тестировщик ПО"** или воспользоваться строкой поиска **"Чему вы хотите научиться"**, вписав в данную строку слово **"Тестировщик"** и затем выбрав профессию **"Тестировщик ПО"**

#### Способ № 4

1) Перейти на страницу сайта [Нетологии](https://netology.ru/)
2) В разделе **"Направления обучения"** выбрать **"Программирование"**
3) На появившейся странице выбрать профессию **"Тестировщик ПО"** или воспользоваться строкой поиска **"Чему вы хотите научиться"**, вписав в данную строку слово **"Тестировщик"** и затем выбрав профессию **"Тестировщик ПО"**

#### Способ № 5

1) Перейти на страницу сайта [Нетологии](https://netology.ru/)
2) На главной странице "Нетологии" опуститься до **"подвала"** (блока в нижней части страницы)
3) В разделе **"Обучение"** выбрать **"Каталог курсов"**
4) На появившейся странице выбрать профессию **"Тестировщик ПО"** или воспользоваться строкой поиска **"Чему вы хотите научиться"**, вписав в данную строку слово **"Тестировщик"** и затем выбрав профессию **"Тестировщик ПО"**

### 1.Перечень автоматизируемых сценариев

#### Сценарий № 1 (валидные значения)
1) Поле "Имя" заполнено валидным значением (например, Екатерина)
2) Поле "Номер телефона" запонено валидным значением (например, +7 999 999 99 99)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@mail.ru)
4) После нажатия на кнопку "Записаться" заявка усшено отправлена

#### Сценарий № 2 (невалидное имя)
1) Поле "Имя" заполнено **НЕ**валидным значением (например, 9999)
2) Поле "Номер телефона" запонено валидным значением (например, +7 999 999 99 99)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@mail.ru)
4) После нажатия на кнопку "Записаться" под полем "Имя" появляется надпись **"Должно состоять из букв"**

#### Сценарий № 3 (невалидный телефон)
1) Поле "Имя" заполнено валидным значением (например, Екатерина)
2) Поле "Номер телефона" запонено **НЕ**валидным значением (например, Екатерина)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@mail.ru)
4) После нажатия на кнопку "Записаться" под полем "Номер телефона" появляется надпись **"Номер в формате +9 (999) 999-99-99"**

#### Сценарий № 4 (номер телефона не российский)
1) Поле "Имя" заполнено валидным значением (например, Екатерина)
2) Поле "Номер телефона" запонено валидным значением (например, +375 999 999 99 99)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@mail.ru)
4) После нажатия на кнопку "Записаться" заявка усшено отправлена

#### Сценарий № 5 (невалидная почта)
1) Поле "Имя" заполнено валидным значением (например, Екатерина)
2) Поле "Номер телефона" запонено валидным значением (например, +7 999 999 99 99)
3) Поле "Электронная почта" заполнено **НЕ**валидным значением (например, testerrr)
4) После нажатия на кнопку "Записаться" под полем "Электронная почта" появляется надпись **"Неверный email"**

#### Сценарий № 6 (поля не заполнены)
1) Поле "Имя" **НЕ**заполнено
2) Поле "Номер телефона" **НЕ**запонено
3) Поле "Электронная почта" **НЕ**заполнено
4) После нажатия на кнопку "Записаться" под полями "Имя", "Номер телефона", "Электронная почта" появляется надпись **"Обязательное поле"**

#### Сценарий № 7 (короткое имя)
1) Поле "Имя" заполнено **НЕ**валидным значением из одной буквы (Например, А)
2) Поле "Номер телефона" запонено валидным значением (например, +7 999 999 99 99)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@mail.ru)
4) После нажатия на кнопку "Записаться" под полем "Имя" появляется надпись **"Должно быть не короче 2 символов"**

#### Сценарий № 8 (длинное имя)
1) Поле "Имя" заполнено **НЕ**валидным значением из одной буквы (Например, Напу-Амо-Хала-Она-Она-Анека-Вехи-Вехи-Она-Хивеа-Нена-Вава-Кехо-Онка-Кахе-Хеа-Леке-Еа-Она-Ней-Нана-Ниа-Кеко-Оа-Ога-Ван-Ика-Ванао)
2) Поле "Номер телефона" запонено валидным значением (например, +7 999 999 99 99)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@mail.ru)
4) После нажатия на кнопку "Записаться" заявка усшено отправлена

#### Сценарий № 9 (длинный телефон)
1) Поле "Имя" заполнено валидным значением из одной буквы (например, Екатерина)
2) Поле "Номер телефона" запонено **НЕ**валидным значением состояшим из более чем 15 символов (например, +375 999 999 99 99 00)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@mail.ru)
4) После нажатия на кнопку "Записаться" под полем "Номер телефона" появляется надпись **"Номер в формате +9 (999) 999-99-99"**

#### Сценарий № 10 (короткий телефон)
1) Поле "Имя" заполнено валидным значением из одной буквы (например, Екатерина)
2) Поле "Номер телефона" запонено **НЕ**валидным значением состояшим из более чем 6 символов (например, +7 999 99)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@mail.ru)
4) После нажатия на кнопку "Записаться" под полем "Номер телефона" появляется надпись **"Номер в формате +9 (999) 999-99-99"**

#### Сценарий № 11 (валидная отправка на консультацию)
1) Поле "Имя" заполнено валидным значением (например, Екатерина)
2) Поле "Номер телефона" запонено валидным значением (например, +7 999 999 99 99)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@mail.ru)
4) После нажатия на кнопку "Получить консультацию" заявка на консультацию успешно направлена

#### Сценарий № 12 (невалидное имя)
1) Поле "Имя" заполнено **НЕ**валидным значением (например, 12345)
2) Поле "Номер телефона" запонено валидным значением (например, +7 999 999 99 99)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@mail.ru)
4) После нажатия на кнопку "Получить консультацию" под полем "Имя" появляется надпись **"Должно состоять из букв"**

#### Сценарий № 13 (невалидный телефон)
1) Поле "Имя" заполнено валидным значением (например, Екатерина)
2) Поле "Номер телефона" запонено **НЕ**валидным значением (например, Екатерина)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@mail.ru)
4) После нажатия на кнопку "Получить консультацию" под полем "Номер телефона" появляется надпись **"Номер в формате +9 (999) 999-99-99"**

#### Сценарий № 14 (невалидная почта)
1) Поле "Имя" заполнено валидным значением (например, Екатерина)
2) Поле "Номер телефона" запонено валидным значением (например, +7 999 999 99 99)
3) Поле "Электронная почта" заполнено **НЕ**валидным значением (например, Екатерина)
4) После нажатия на кнопку "Получить консультацию" под полем "Электронная почта" появляется надпись **"Неверный email"**

#### Сценарий № 15 (поля не заполнены)
1) Поле "Имя" **НЕ**заполнено
2) Поле "Номер телефона" **НЕ**запонено
3) Поле "Электронная почта" **НЕ**заполнено
4) После нажатия на кнопку "Получить консультацию" под полями "Имя", "Номер телефона", "Электронная почта" появляется надпись **"Обязательное поле"**

#### Сценарий № 16 (короткое имя)
1) Поле "Имя" заполнено **НЕ**валидным значением из одной буквы (Например, А)
2) Поле "Номер телефона" запонено валидным значением (например, +7 999 999 99 99)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@mail.ru)
4) После нажатия на кнопку "Получить консультацию" под полем "Имя" появляется надпись **"Должно быть не короче 2 символов"**

#### Сценарий № 17 (длинное имя)
1) Поле "Имя" заполнено **НЕ**валидным значением из одной буквы (Например, Напу-Амо-Хала-Она-Она-Анека-Вехи-Вехи-Она-Хивеа-Нена-Вава-Кехо-Онка-Кахе-Хеа-Леке-Еа-Она-Ней-Нана-Ниа-Кеко-Оа-Ога-Ван-Ика-Ванао)
2) Поле "Номер телефона" запонено валидным значением (например, +7 999 999 99 99)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@mail.ru)
4) После нажатия на кнопку "Получить консультацию" заявка на консультацию успешно направлена.

#### Сценарий № 18 (длинный телефон)
1) Поле "Имя" заполнено валидным значением из одной буквы (например, Екатерина)
2) Поле "Номер телефона" запонено **НЕ**валидным значением состояшим из более чем 15 символов (например, +375 999 999 99 99 00)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@mail.ru)
4) После нажатия на кнопку "Получить консультацию" под полем "Номер телефона" появляется надпись **"Номер в формате +9 (999) 999-99-99"**

#### Сценарий № 19 (короткий телефон)
1) Поле "Имя" заполнено валидным значением из одной буквы (например, Екатерина)
2) Поле "Номер телефона" запонено **НЕ**валидным значением состояшим из более чем 15 символов (например, +7 999 9)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@mail.ru)
4) После нажатия на кнопку "Получить консультацию" под полем "Номер телефона" появляется надпись **"Номер в формате +9 (999) 999-99-99"**

#### Сценарий № 20 (номер телефона не российский)
1) Поле "Имя" заполнено валидным значением (например, Екатерина)
2) Поле "Номер телефона" запонено валидным значением (например, +375 999 999 99 99)
3) Поле "Электронная почта" заполнено валидным значением (например, tester@хостер.бел)
4) После нажатия на кнопку "Получить консультацию" заявка на консультацию успешно направлена


### 2.Перечень используемых инструментов с обоснованием выбора.
1) **IntelliJ IDEA** - среда для разработки автотестов
2) **CI** - настройка проекта для непрерывной интеграции
3) **Gradle, maven** - инструменты для сборки проектов 
3) **JUnit, Selenide, Lombok, Faker** - библиотеки подключаемые в проекте
4) **Allure** фреймворк для создания отчетов после тестирования
5) **Jira, Git Issues** - система для заведения баг-репортов 

### 3.Перечень необходимых разрешений, данных и доступов.
1) Доступ на тестирование сайта Нетологии
2) JAR - файл, т.е. тестовое приложение для тестирования отправки формы
3) Тенническое задание

### 4.Перечень и описание возможных рисков при автоматизации.
1) Перегруженность сайта, т.к. при тестировании самого сайта будут отправляться реальные заявки.
2) Возможно обновление данных на сайте, тесты могут устареть.

### 5.Перечень необходимых специалистов для автоматизации.
1) Тестировщик со знанием автоматизации
2) Руководитель проекта, который предоставит разрешение на тестирование продуктивного стенда

### 6.Интервальная оценка с учётом рисков в часах.
1) Анализ требований и данных (1-2 часа)
2) Ручное тестирование 4-5 часов
3) Автоматизированное тестирование: 15-20 часов на начальных этапах, с опытом быстрее



