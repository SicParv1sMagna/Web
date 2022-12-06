# Разработка Интернет Приложений (РИП) 2022

## [Видеозаписи лекций в youtube](https://youtube.com/playlist?list=PLLELLTvDgUQ9cpB1XzSuZ0mNSBkbjVNJ_)
#### Образ виртуальной машины Linux [Ubuntu 20.04](https://github.com/iu5git/Standards/blob/main/Linux/Linux.md) для выполнения заданий курса 

## Лекции
### Бекенд
[Лекция 1. История Web, трехуровневая модель приложений, MVC](https://github.com/iu5git/web-2022/blob/main/lectures/web_intro.pdf) 

[Лекция 2. Методология Agile, состав команды. Диаграммы UML](https://github.com/iu5git/web-2022/blob/main/lectures/Lecture_2_Agile_UML.pdf)

[Лекция 3. Основы Web, шаблонизация, Django](https://github.com/iu5git/web-2022/blob/main/lectures/Lecture_3_Web_Django.pdf)

[Лекция 4. Базы данных, ER, PostgreSQL. ORM. Админка Django. Курсоры](https://github.com/iu5git/web-2022/blob/main/lectures/Lecture_4_Databases_Django_ORM.pdf)

[Лекция 5. Веб-сервис. Swagger. Микросервисы](https://github.com/iu5git/web-2022/blob/main/lectures/Lecture_5_Web_Service.pdf)

[Лекция 6. Работа в git. Примеры специализированных сервисов - S3, уведомления, очереди](https://github.com/iu5git/web-2022/blob/main/lectures/Lecture_6_Special_Services.pdf)

### Фронтенд
[Лекция 7. Введение в фронтенд и React](https://github.com/iu5git/web-2022/blob/main/lectures/Lecture_7_React_Introduction.pdf)

[Лекция 8. React, сборка, компоненты](/lectures/Lecture_8_React.pdf)

[Лекция 9. Redux, hooks](/lectures/Lecture_9_Redux.pdf)

[Лекция 10. Ajax, запросы на React. WebSocket](/lectures/Lecture_10_Ajax.pdf)

[Лекция 11. Авторизация, куки, хранилище сессий](/lectures/Lecture_11_Authorization.pdf) 

[Лекция 12. JWT. SSO](/lectures/Lecture_12_jwt.pdf) 

### Мобильные приложения

[Лекция 13. Общая лекция про мобильные приложения. PWA](/lectures/Lecture_13_PWA.pdf) 

Лекция 14. Конкретные кейсы с примерами кода. Сетевое взаимодействие. 

### Инфраструктура

Лекция 15. Деплой, DevOps, RE

## Лабораторные работы
У каждого своя предметная область на весь курс: бронирование отелей, билетов в театр/кинотеатр, онлайн-магазин

Основной вариант лаб по беку - это Django. Но есть ещё варианты на `Go`, `Java`, `C#` и `Node.js`

При защите необходимо продемонстрировать работу приложения, UML диаграмму, репозиторий github с кодом и ответить на вопросы.

#### Лабораторная работа №1
Базовая шаблонизация в Django для словаря. Создание базового интерфейса для просмотра списка (отели, товары, рейсы и тд) с ссылками и частью полей (цена, город) и при переходе по ссылке другая страница с более подробной информацией о товаре (описание, картинка и тд). 

В приложении должны быть использованы стили, для каждого элемента списка подгружается свое изображение. 

Добавить поле input для ограничения количества записей, отображаемых на странице (по умолчанию отображать все).

На выбор `Django`, `Go`, `Spring`, `Node.js`

Контрольные вопросы: MVC, Django, шаблонизация, HTTP, Web, HTML

* [Методические указания Django](/tutorials/lab1-py/lab1_tutorial.md)
* [Методические указания Golang](/tutorials/lab1-go/README.md)

#### Лабораторная работа №2
Создание базы данных `PostgreSQL`/`MySQL` (`SQLite` использовать нельзя), подключение к шаблонизатору. Создание админки.

Для карточек таблицы услуг добавить кнопку удаления услуги с помощью выполнения SQL запроса.

Таблицы: таблица услуг - словарь, таблица фактов - бронирования (с датами и статусом, три даты и менеджер), таблица пользователей

Статусы: введен, в работе, завершён, удалён

ER диаграмма: таблицы, связи, столбцы, типы столбцов и их длина, первичные, вторичные ключи

Контрольные вопросы: ORM, SQL, модель и миграции

* [Методические указания Django](/tutorials/lab2-py/lab2_tutorial.md)
* [Методические указания Golang](/tutorials/lab2-go/README.md)

#### Лабораторная работа №3
Создание веб-сервиса для получения/редактирования данных из вашей БД. Требуется разработать методы для основных (минимум трех) таблиц вашего приложения. Проверка в swagger/postman. 

Добавить метод для подсчета суммы (количества) покупок/бронирований за определенную дату через обращение к методам модели.

Диаграмма компонентов+классов: компонент сервиса, интерфейс, структура модели по классам

Контрольные вопросы: веб-сервис, микросервисы, REST, RPC

* [Методические указания DRF](/tutorials/lab3-py/lab3_tutorial.md)
* [Методические указания Golang](/tutorials/lab3-go/README.md)

#### Лабораторная работа №4
Базовая работа по фронтенду. Карточки элементов, навигация. Необходимо разработать страницы, аналогичные лабораторной работе №1 для просмотра услуг. Использовать компоненты `React-Bootstrap`. Без взаимодействия с сервисом, карточки наполняются через mock-объекты.

Навигация по двум страницам должна быть организована посредством Навигационной цепочки `Breadcrumbs`: [Магазин](/README.md) / [Название услуги](/README.md)

На выбор `React`, `Vue`, `Angular`

Deployment диаграмма: узлы фронтенда, веб-сервиса, базы данных, web-сервера со статикой

Контрольные вопросы: react, props, компонент, элемент, состояние, хуки, жизненный цикл компонента

* [Методические указания](/tutorials/lab4/lab4_tutorial.md)

#### Лабораторная работа №5
Подключение разработанного интерфейса фронтенда к веб-сервису из лабораторной №3. Ajax-запросы написать самостоятельно (через fetch например). 

Добавление менеджера состояний (`redux` или через хуки `useReducer`, `useContext`) для кеширования полученных по API данных и их использования в компонентах. 

На выбор `React`, `Vue`, `Angular`

Sequence диаграмма: получение `HTML` страницы, `AJAX` запросы

Контрольные вопросы: AJAX, json, XmlHttpRequest/fetch, redux, контекст

* [Методические указания](/tutorials/lab5/lab5_tutorial.md)

#### Лабораторная работа №6
Добавление страницы просмотра для таблицы бронирований (корзина товаров, бронирования) и кнопки бронирования услуги. Из корзины товар можно удалить. 

Для подключения к нужным сервисам/методам бэкенда желательно использовать автоматическую кодогенерацию через swagger (дополнительные баллы). На бэкенде должна быть доступна админская панель.

В приложении должно быть реализовано переключение между интерфейсом гостя и интерфейсом пользователя - без аутентификации, просто смена состояния.

Добавление фильтрации и поиска на странице услуг (сама фильтрация на стороне бэкенда):
1. По наименованию услуги
2. По диапазону значений (цене). Максимальное и минимальное значение запрашиваются с сервера

Activity диаграмма: описание основного алгоритма, разделение на дорожки по элементам системы или ролям пользователей 

Контрольные вопросы: AJAX, json, XmlHttpRequest/fetch, react, props, компонент, элемент, состояние, веб-сервис, микросервисы, REST, RPC

* [Методические указания](/tutorials/lab6/lab6_tutorial.md)

#### Лабораторная работа №7
Добавить модель таблицы пользователей, реализовать методы бэкенда и окна фронтенда для аутентификации и регистрации. Авторизация через хранение сессий (Redis - дополнительные баллы) и куки. Автозаполнение пользователя в таблице фактов при создании нового бронирования.

Диаграмма компонентов с детализацией бэкенда: все компоненты системы с интерфейсами, выделить сервисы и интерфейсы данных и авторизации

Контрольные вопросы: куки, сессия, redis, jwt, авторизация, аутентификация

* [Настройка Redis через WSL](tutorials/redis_wsl/redis.md))
* [Методические указания DRF Redis](https://github.com/iu5git/web-2022/blob/main/tutorials/lab7-py/lab7_tutorial.md)
* [Методические указания Golang JWT](https://github.com/iu5git/web-2022/tree/main/tutorials/lab7-go/README.md)

#### Лабораторная работа №8
Создание мобильного нативного приложения (дополнительные баллы) или `PWA` с адаптивной версткой для телефона. 

Требуется реализовать подключение к web-сервису. Просмотр услуг (товаров и тд), без бронирования и редактирования. 

Контрольные вопросы: PWA, service worker, manifest.json, media queries

* [iOS (Swift)](https://github.com/iu5git/web-2022/blob/main/tutorials/ios_tutorial/ios_tutorial.md)
* [Android (Java)](https://github.com/iu5git/web-2022/blob/main/tutorials/android_tutorial/android_tutorial.md)
* [React Native + Redux Toolkit](/tutorials/react-native/react_native.md)
* [Progressive Web App](/tutorials/pwa/PWA.md)

## Домашнее задание
Добавление роли пользователя-менеджера контента, доработка под эту роль фронтенда и веб-сервиса:
1. Редактирование таблицы услуг
2. Изменение статусов таблицы бронирования
3. Фильтрация записей таблицы бронирования по дате и статусу. Список статусов начитывается с сервера

Доработка ролевой модели - ограничение прав на интерфейс для пользователь-клиента. Добавление главного меню приложения.

Добавить ограничение на вызовы методов веб-сервиса. Без авторизации менеджера в Insomnia должно быть доступно только чтение-получение данных через API 

Контрольные вопросы: куки, сессия, AJAX, json, веб-сервис

* [Методические указания](/tutorials/homework/homework_tutorial.md)

#### Оформление единого отчёта 
Добавить диаграмму состояний для бронирований или услуг и диаграмму прецедентов.

Актуализировать все диаграммы из лабораторных, добавить краткое описание к диаграммам.

Пять разделов отчета: 
1. Введение (цель, задачи, актуальность)
2. Бизнес-процесс. Диаграмма прецедентов, диаграмма состояний
3. Архитектура. Диаграммы развертывания, ER с назначением таблиц и диаграмма компонентов с детализацией бекенда
4. Алгоритмы. Диаграмма последовательности и деятельности
5. Описание интерфейса. Перечень окон и их назначение

## Вопросы к экзамену
1. Шаблон MVC
2. Django
3. Шаблонизация
4. Протокол HTTP
5. Web
6. HTML
7. URI
8. ORM
9. SQL
10. Модель и миграции
11. Веб-сервис
12. Сервис-ориентированная архитектура
13. Микросервисная архитектура
14. REST
15. RPC
16. AJAX
17. JSON
18. XmlHttpRequest/fetch
19. Архитектура React приложения
20. Функциональные компоненты. React Hooks
21. Менеджер состояний Redux
22. Куки
23. Redis
24. JWT
25. Авторизация и аутентификация
26. Отличия Axios от fetch
