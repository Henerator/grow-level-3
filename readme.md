**Table of contents**

[Software Development Methodologies](#software-development-methodologies)
- [Agile](#agile)
  - [Приниципы](#приниципы)
  - [Scrum](#scrum)
  - [Kanban](#kanban)
  - [Extreme Programming](#extreme-programming)
  - [Lean](#lean)
- [Waterfall](#waterfall)
- [RAD model](#rad-model)
- [Incremental model](#incremental-model)
  - [Advantages](#advantages)
  - [Disadvantages](#disadvantages)
- [Iterative model](#iterative-model)
- [Spiral model](#spiral-model)
- [V-model](#v-model)

[JS Engines](#js-engines)
- [V8](#v8)
  - [Threads](#threads)
  - [Hidden class](#hidden-class)
  - [Inline Caching](#inline-caching)
  - [Optimize your code](#optimize-your-code)

[Estimation](#estimation)
- [T-Shirt Size](#t-shirt-size)
- [Planning Poker](#planning-poker)
- [Bucket System](#bucket-system)
- [Dot-voting](#dot-voting)
- [Estimation by Analogy](#estimation-by-analogy)
- [Bottom-up Estimating](#bottom-up-estimating)
- [Up-bottom Estimating](#up-bottom-estimating)
- [PERT (Program Evaluation Review Technique)](#pert-program-evaluation-review-technique)
- [Bug Fixing Time Planning](#bug-fixing-time-planning)
- [Experts Estimations](#experts-estimations)

[Client server communication](#client-server-communication)
- [Long Pooling](#long-pooling)
- [Server Side Events](#server-side-events)
- [Web Sockets](#web-sockets)

[Code quiality](#code-quiality)
- [7 axes](#7-axes)
- [Metrics](#metrics)
- [How to Improve Code Quality](#how-to-improve-code-quality)

[Test pyramid](#test-pyramid)
- [Integration tests](#integration-tests)

[SonarQube](#sonar-qube)

[OWASP 10](#owasp-10)

[Design pattern](#design-pattern)
- [MVC](#mvc)
  - [Passive view](#passive-view)
- [MVP](#mvp)
  - [Passive View](#passive-view)
  - [Supervising Controller](#supervising-controller)
- [MVVM](#mvvm)

[Flux](#flux)
- [Redux](#redux)

[SOLID](#solid)

[Programming Principles](#programming-principles)
- [KISS](#kiss)
- [DRY](#dry)
- [YAGNI](#yagni)

# Software Development Methodologies

SDLC (Software Development Life Cycle)

фреймворк, описывающий способ управления процессом разработки продукта

Этапы:

1. **Анализ требований** отвечает на вопрос «Какие проблемы требуют решений?»
1. **Планирование** отвечает на вопрос «Что мы хотим сделать?»
1. **Проектирование и дизайн** отвечает на вопрос «Как мы добьемся наших целей?»
1. **Разработка ПО** регулирует процесс создания продукта.
1. **Тестирование** регулирует обеспечение качественной работы продукта.
1. **Развертывание** регулирует использование финального продукта.

- It offers a basis for project planning, scheduling, and estimating
- Provides a framework for a standard set of activities and deliverables
- It is a mechanism for project tracking and control
- Increases visibility of project planning to all involved stakeholders of the development process
- Increased and enhance development speed
- Improved client relations
- Helps you to decrease project risk and project management plan overhead

## Agile

итеративный подход к управлению проектами и разработке ПО, позволяющий командам ускорить доставку ценности клиентам. Agile-команда выполняет работу в рамках небольших, но удобных инкрементов. Требования, планы и результаты постоянно проходят проверку на актуальность, благодаря чему команды могут быстро реагировать на изменения.

### Приниципы

- **Люди и взаимодействие** важнее процессов и инструментов.
- **Работающий продукт важнее** исчерпывающей документации.
- **Сотрудничество с заказчиком** важнее согласования условий контракта.
- **Готовность к изменениям** важнее следования плану.

- incremental and iterative approach
- separates a project into sprints
- helps complete many small projects
- introduces a product mindset with a focus on customer satisfaction
- requirements are prepared everyday
- allows requirement changes at any time
- testing is performed concurrently with development
- test teams can take part in requirements change
- enables the entire team to manage the project without a dedicated project manager

### Scrum

минимально необходимый набор мероприятий, артефактов, ролей, на которых строится процесс SCRUM-разработки, позволяющий за фиксированные небольшие промежутки времени, называемые спринтами (sprints), предоставлять конечному пользователю работающий продукт с новыми бизнес-возможностями, для которых определен наибольший приоритет

- Регулярные спринты с фиксированной продолжительностью (например, 2 недели)
- Релиз в конце каждого спринта
- В ходе спринта команды не должны вносить изменения

#### Activities

- Работа с Бэклогом Продукта
- Планирование Спринта
- Daily Scrum
- Демонстрация
- Ретроспектива

#### Roles

- Scrum Master - следит за соблюдением scrum принципов всей командой и предлагает улучшение процессов
- Product owner - является связующим звеном между командой разработки и заказчиком
- Команда разработки

### Kanban

Канбан – это метод, инструмент с набором практик и принципов. Вы можете использовать все практики, часть практик или не использовать их вообще.

Скрам – это фреймворк с жесткими правилами и границами. Вы можете использовать разные инструменты и методологии внутри Скрама, но если вы отказались от чего-то обязательного в Скраме, он уже не может считаться Скрамом.

- Непрерывный процесс (отсутствуют спринты)
- Непрерывная поставка (релиз не ожидает окончания спринта)
- Изменение может произойти в любой момент

### Extreme Programming

применимо только в области разработки ПО. Не может быть использовано в другом бизнесе или повседневной жизни

цель методики XP — справиться с постоянно меняющимися требованиями к программному продукту и повысить качество разработки

#### Practicies

- **Итеративность** - разработка ведется короткими итерациями (2-3 недели) при наличии активной взаимосвязи. Отсутствие формализации описания входных данных проекта компенсируетс за счет активного включения в процесс разработки заказчика
- **Простота решений** - принимается первое простейшее рабочее решение. Экстремальность метода связана с высокой степенью риска решения. Реализуется минимальный набор главных функций системы на первой и каждой последующей итерации
- **Интенсивная разработка малыми группами** (не больше 10 человек)
- **Парное программирование** - парное программирование направлено на решение задачи стабилизации проекта. Один программист из пары может поддерживать код при уходе с проекта другого.
- **Обратная связь с заказчиком**
- **Рефакторинг**
- **40-часовая рабочая неделя**
- **Небольшие релизы**
- **Непрерывная интеграция**
- **Тестирование** - тесты пишутся до написания кода

### Lean

философия бережливого мышления. Подход, который позволяет экономить ресурсы и получать лучший результат.

В двух словах: избавляйтесь от всего, что не добавляет дополнительной ценности, и делайте только то, в чем вы абсолютно уверены, что это нужно делать в настоящий момент. Устраняйте бесполезные собрания, задачи и документацию, избавляйтесь от временных потерь в любых известных задачах, которые нужно будет сделать в будущем (все меняется и часто в итоге становится ненужным)

- использовать системный подход
- искать и устранять потери
- создавать поток (поток - непрерывный процесс создания продукта, который нужен потребителю)

#### Principles

- **Ликвидировать потери** - если действие не улучшает качество продукта, не приносит прибыли заказчику и не экономит время разработчика, то его нужно исключить.
- **Усиливать обучение** - чтобы создавать качественный продукт, команда должна постоянно совершенствовать свои знания и навыки. А руководитель ― обеспечивать команду временем и ресурсами.
- **Принимать важные решения в последний момент** - иногда запоздало принятое решение может испортить всю проделанную работу, но для Lean откладывать принятие решения до последнего ― это способ собрать как можно больше информации о вопросе. А значит, быть уверенным в его правильности и избежать ошибок.
- **Доставлять ценность как можно раньше** - чем раньше команда покажет свои наработки заказчику, тем быстрее получит от него обратную связь и смогут внести изменения при необходимости.
- **Объединять сотрудников** - когда команда работает сообща и понимает свою ценность, процесс идет быстрее и эффективнее. Поэтому важно доверять сотрудникам и ценить то, что они делают.
- **Создавать целостный продукт** - команда должна сфокусироваться на качестве, не допускать дефектов и всегда ставить в приоритет потребности заказчика.
- **Следить за общим процессом** - чтобы работа шла хорошо, каждый в команде должен понимать задачи и иметь возможность постоянно видеть весь процесс. Вся информация по проекту должна быть доступна в любое время. Для этих целей в гибких методологиях (Scrum, Kanban) используют доску, где отмечены цели, задачи и процесс их выполнения.


#### Principles

- прозрачность
- баланс
- сотрудничество
- клиентоориентированность
- поток
- лидерство
- понимание
- согласие
- уважение

#### Practicies

- визуализируйте (имеется ввиду визуализация процесса с помощью Канбан-доски)
- ограничивайте незавершенную работу
- управляйте потоком работы
- используйте явные правила
- вводите петли обратной связи (каденции)
- улучшайте и эволюционируйте

> Канденции - регулярные встречи, которые еще являются петлями обратной связи

## Waterfall

- linear and sequential approach
- divides a project into phases
- helps complete one single project
- introduces a project mindset with a focus on successful project delivery
- requirements are prepared once at the start
- avoids scope changes once the project starts
- testing phase comes only after the build phase
- test teams do not get involved in requirements change
- requires a project manager who plays an essential role in every phase

## RAD model

Rapid application development

## Incremental model

- system development is broken down into many mini development projects
- partial systems are successively built to produce a final total system
- highest priority requirement is tackled first
- once the requirement is developed, requirement for that increment are - frozen

### Advantages

- The software will be generated quickly during the software life cycle
- It is flexible and less expensive to change requirements and scope
- Throughout the development stages changes can be done
- This model is less costly compared to others
- A customer can respond to each building
- Errors are easy to be identified

### Disadvantages

- It requires a good planning designing
- Problems might cause due to system architecture as such not all requirements collected up front for the entire software lifecycle
- Each iteration phase is rigid and does not overlap each other
- Rectifying a problem in one unit requires correction in all the units and consumes a lot of time

## Iterative model

## Spiral model

## V-model

# JS Engines

- V8 - открытый исходный код, разработан компанией Google, написан на C++
- Rhino - управляемый Mozilla Foundation, открытый исходный код, разработан преимущественно на Java
- SpiderMonkey - первый движок JavaScript, который был ранее разработан Netscape Navigator, а сейчас над ним работает Firefox
- JavaScriptCore - открытый исходный код, продавался под именем Nitro и разрабатывался компанией Apple для Safari
- KJS - движок первоначально разработанный Harri Porten для KDE проекта - браузера Konqueror
- Chakra (JScript9) - в браузере Internet Explorer
- Chakra (JavaScript) - в браузере Microsoft Edge
- Nashorn - открытый исходный код как часть OpenJDK, написанный на Oracle Java Languages и Tool Group
- JerryScript - легковесный движок для Интернета вещей

## V8

используется внутри Google Chrome и для среды выполнения Node.js

V8 компилирует код JavaScript в машинный код во время исполнения путем реализации JIT (Just-In-Time) компилятора

> JIT-компиляция - технология увеличения производительности программных систем, использующих байт-код, путём компиляции байт-кода в машинный код или в другой формат непосредственно во время работы программы.

### Threads

- Основной поток - получает код, компилирует, выполняет
- Отдельный поток для компиляции - основной поток может продолжать выполняться, пока первый оптимизирует код
- Profiler - сообщает среде выполнения, на какие методы тратится много времени, чтобы Crankshaft мог их оптимизировать
- Несколько потоков для сборки мусора

### Hidden class

Использование словарей для поиска местоположения свойств объекта в памяти неэффективно, поэтому V8 использует другой метод: скрытые классы, которые работают аналогично схемам фиксированных объектов (классам), используемым в таких языках, как Java, за исключением того, что они создаются во время выполнения.

При создании экземпляра класса создается скрытый пустой класс. Добавление поля к экземпляру создает новый класс основанный на предыдущем.

### Inline Caching

Встроенное кэширование основано на наблюдении, что повторные вызовы одного и того же метода имеют тенденцию происходить на объектах одного типа.

V8 поддерживает кэш типа объектов, которые были переданы в качестве параметра в недавних вызовах методов, и использует эту информацию, чтобы сделать предположение о типе объекта, который будет передан в качестве параметра в будущем. После двух успешных вызовов одного и того же метода, к одному и тому же скрытому классу, V8 пропускает поиск скрытого класса и просто добавляет смещение свойства к самому указателю объекта.

### Optimize your code

- **Порядок свойств объекта**: всегда создавайте экземпляры свойств вашего объекта в одном и том же порядке, чтобы скрытые классы, и впоследствии оптимизированный код, могли совместно использоваться.
- **Динамические свойства**: добавление свойств к объекту, после создания экземпляра, вызовет изменение скрытого класса и замедлит все методы, которые были оптимизированы для предыдущего скрытого класса. Вместо этого назначьте все свойства объекта в его конструкторе.
- **Методы**: код, который выполняет один и тот же метод несколько раз, будет выполняться быстрее, чем код, который выполняет много разных методов только один раз (из-за встроенного кэширования).
- **Массивы**: избегайте разреженных массивов, где ключи не являются инкрементными числами. Разреженные массивы, в которых нет каждого элемента, являются хэш-таблицей. Элементы в таких массивах более дороги для доступа. Также старайтесь избегать предварительного выделения больших массивов. Не удаляйте элементы в массивах. Это делает ключи разреженными.
- **Помеченные значения**: V8 представляет объекты и числа с 32 битами. Он использует бит, чтобы узнать, является ли он объектом (flag = 1), или целым числом (flag = 0), называемым SMI (SMall Integer) из-за его 31 бита. Затем, если числовое значение больше 31 бита, V8 укажет число, превратив его в двойное и создав новый объект для помещения числа внутрь. Старайтесь по возможности использовать 31-разрядные числа со знаком, чтобы избежать дорогостоящей операции упаковки в объект JS.

# Estimation

## T-Shirt Size

XS, S, M, L, XL

Первые несколько задач оцениваются предварительно. Далее начинает вырисовываться картина о степени декомпозиции историй. В итоге находят самые мелкие относительно остальных задачи и они принимаются за XS. После этого остальные задачи оцениваются с точки зрения насколько они больше XS

## Planning Poker

одна из самых точных техник оценки, но подходит для сравнительно небольшого количества задач

## Bucket System

- Все истории выписываются на карточки
- Выстраивается последовательность из «ведерок» для задач различного размера
- Команда выбирает по очереди 3-5 произвольные карточки с задачами и оценивает их в ходе открытого обсуждения сравнивая и выстраивая их друг относительно друга
- Задачи помещаются в соответствующие «ведра», задавая общий масштаб и ориентиры для последующих оценок
- Все оставшиеся задачи поровну разделяются между всеми участниками и оцениваются ими самостоятельно, с учетом полученной шкалы измерений
- Если кто-то из членов команды затрудняется оценить какую-либо историю, то он передает ее другому

## Dot-voting

- Все оцениваемые Stories выписываются на отдельные карточки
- Каждый из участников получает одинаковое количество «точек», которые он распределяет между задачами
- Подсчитывается общее количество точек выставленных для каждой истории

## Estimation by Analogy

получение оценки текущего проекта, называемого целевым, на основе фактической стоимости одного или нескольких предыдущих проектов (аналогичных или исходных) близкого размера, сложности и содержания

## Bottom-up Estimating

Работа разбивается на более мелкие. Оценивается каждая из частей. Оценки  суммируются. Точность оценки "снизу вверх" определяется размером и сложностью работ, выделенных на более нижних уровнях

## Up-bottom Estimating

используется для оценки затрат на ранних стадиях проекта, когда информация о проекте еще очень ограниченна. Смысл такой укрупненной экспертной оценки в том, что она производится обобщенно и проект оценивается в целом по одному показателю. Оценка удобна тем, что не требует больших усилий и времени. Недостатком же является не такая высокая точность, какая могла бы быть при более детальной оценке

## PERT (Program Evaluation Review Technique)

Three-Point Estimates

предназначен для очень масштабных, единовременных, сложных, нерутинных проектов. Метод подразумевает наличие неопределённости, давая возможность разработать рабочий график проекта без точного знания деталей и необходимого времени для всех его составляющих

Сама идея метода крайне проста — для того, чтобы оценить время выполнения задачи или процесса, вам необходимо знать оптимистичную, пессимистичную и наиболее вероятную оценку продолжительности этой задачи

E = (O + 4*M + P)/6
E = (BestCase + 4*LikelyCase + WorstCase)/6

## Bug Fixing Time Planning

use Three-Point Estimation

## Experts Estimations

процесс получения оценки чего-либо, на основе мнения и опыта экспертов

# Client server communication

## Long Pooling

cамый простой способ получать новую информацию от сервера – периодический опрос

## Server Side Events

Спецификация Server-Sent Events описывает встроенный класс EventSource, который позволяет поддерживать соединение с сервером и получать от него события.

поддерживает автоматическое переподключение при потере соединения

### Restrictions

- Однонаправленность: данные посылает только сервер
- Только текст
- Протокол: Обычный HTTP

## Web Sockets

обеспечивает возможность обмена данными между браузером и сервером через постоянное соединение. Данные передаются по нему в обоих направлениях в виде «пакетов», без разрыва соединения и дополнительных HTTP-запросов.

- Двунаправленность: и сервер, и клиент могут обмениваться сообщениями
- Бинарные и текстовые данные
- Протокол: WebSocket

# Code quiality

- Does what it should
- Follows a consistent style
- It is easy to understand
- Has been well-documented
- It can be tested

## 7 axes

- **Coding standards** - respect coding standards and follow best practices
- **Potential bugs** - eliminate code violations to prevent vulnerabilities
- **Documentation and comments** - provide documentation especially for the Public API, the source code
- **Duplicated code** - isolates and refines duplications, Don't Repeat Yourself
- **Complexity** - equalizes disproportionate distributed complexity among components; eliminates complexity if possible
- **Test coverage** - writes unit tests, especially for complex parts of the software
- **Design and architecture** - minimize dependencies

## Metrics

- Defect Metrics - the number of defects and severity of those defects
- Complexity Metrics -
  - Cyclomatic complexity - the number of linearly independent paths (if-else)
  - Program length

## How to Improve Code Quality

- Use a coding standard
- Analyze code before code reviews
- Follow code review best practices
- Refactor legacy code (when necessary)

# Test pyramid

- GUI (end-to-end)
- Service (integration)
- Unit tests

1. Модульные тесты реализовывать быстрее, чем GUI тесты (время на разработку меньше). Модульные тесты отрабатывают быстрее, чем GUI
1. Модульные тесты дешевле, чем GUI тесты (стремясь к вершине пирамиды, получаем большую уверенность, что все работает как ожидалось)
1. Тестирование должно быть разносторонним. Модульных должно быть больше, чем GUI

## Integration tests

**Интеграционное тестирование** - программные модули объединяются логически и тестируются как группа. Cосредоточено на интерфейсах и потоке данных между модулями

# SonarQube

латформа с открытым исходным кодом для непрерывного анализа и измерения качества программного кода

измеряет качество программного кода в соответствии с семью показателями

- Потенциальные ошибки
- Стиль программирования
- Тесты
- Повторения участков кода
- Комментарии
- Архитектура и проектирование
- Сложность


# OWASP 10

- **Injection** - occur when untrusted data is sent to an interpreter as part of a command or query
- **Broken Authentication** - allowing attackers to compromise passwords, keys, or session tokens
- **Sensitive Data Exposure** - sensitive data may be compromised without extra protection, such as encryption at rest or in transit, and requires special precautions when exchanged with the browser
- **XML External Entities (XXE)** - Many older or poorly configured XML processors evaluate external entity references within XML documents. External entities can be used to disclose internal files using the file URI handler, internal file shares, internal port scanning, remote code execution, and denial of service attacks
- **Broken Access Control** - Restrictions on what authenticated users are allowed to do. Access to unauthorized functionality and/or data
- **Security Misconfiguration** - misconfigured HTTP headers, verbose error messages containing sensitive information
- **Cross-Site Scripting (XSS)** - application includes untrusted data in a new web page without proper validation or escaping
- **Insecure Deserialization** - leads to remote code execution
- **Using Components with Known Vulnerabilities**
- **Insufficient Logging & Monitoring**

In russian

- Инъекции
- Недочеты системы аутентификации и хранения сессий
- Межсайтовый скриптинг – XSS
- Небезопасные прямые ссылки на объекты - mysite.ru/read_message.jsp?id=123654 (можно перебирать id)
- Небезопасная конфигурация
- Незащищенность критичных данных
- Отсутствие функций контроля доступа
- Межсайтовая подделка запроса (Cross-Site Request Forgery, CSRF/XSRF)
- Использование компонентов с известными уязвимостями
- Непроверенные переадресации и пересылки

# Design pattern

позволяют отделить UI-код (View) от кода логики (Presenter, Controller, ViewModel и т. д.) и кода обработки данных (Model)

Цели:

- **Scalability** - возможность расширять проект, реализовывать новые функции
- **Maintainability** - необходимость изменений после реализации всех функций
- **Reliability**
- **Testability**
- **Modularity**
- **Flexibility**

## MVC

- Model - предоставляет данные и реагирует на команды контроллера, изменяя своё состояние
- View - отвечает за отображение данных модели пользователю, реагируя на изменения модели
- Controller - интерпретирует действия пользователя, оповещая модель о необходимости изменений

![MVC](https://upload.wikimedia.org/wikipedia/commons/thumb/f/fd/MVC-Process.png/240px-MVC-Process.png)

### Passive view

представление полностью управляется контроллером

## MVP

- Model - данные для отображения
- View - реализует отображение данных (из Модели), обращается к Presenter за обновлениями, перенаправляет события от пользователя в Presenter;
- Presenter - реализует взаимодействие между Model и View и содержит в себе всю логику представления данных о предметной области; при необходимости получает данные из хранилища и преобразует для отображения во View.

![MVP](https://upload.wikimedia.org/wikipedia/commons/thumb/5/59/MVP-Pattern.png/274px-MVP-Pattern.png)

### Passive View

представление ничего не знает о модели, но предоставляет свойства для всей информации, которую необходимо отобразить на экране. Презентер будет считывать информацию из модели и обновлять свойства во View

### Supervising Controller

представление знает о модели и отвечает за связывание данных с отображением

## MVVM

удобно использовать, когда есть «связывание данных». В MVC/MVP изменения в интерфейсе не влияют непосредственно на Model, а идут через Controller или Presenter.

- Model - логика работы с данными и описание данных
- View - графический интерфейс. Подписывается на событие изменения свойств или команд ViewModel и оповещает ее о действиях пользователя
- ViewModel - содержит Model, преобразованную к View, а также команды, которыми может пользоваться View, чтобы влиять на Model

![MVVM](https://upload.wikimedia.org/wikipedia/commons/8/87/MVVMPattern.png)

# Flux

подход к управлению состоянием. Накладывает определенные ограничения на то, как и когда могут произойти изменения.

*все данные должны передаваться только в одном направлении*

![MVVM](https://miro.medium.com/max/700/1*WNMEPdtK9TlayHJ1wcUZPQ.png)

- Actions
- Dispatcher - получает действие (action) и перенаправляет его в хранилище (store)
  - приложение имеет только один dispatcher
  - каждое действие отправляется в каждый store
- Stores - структуры, в которых хранится состояние приложения

## Redux

- Не использует Dispatcher: Redux имеет только одно хранилище
- Reducers - чистые функции, которые принимают текущее состояние (state) и заданное действие (action), и выводят либо не измененное состояние, либо новую копию состояния

![MVVM](https://miro.medium.com/max/700/1*-5TBPgIKsJpWzpt5_5xCYw.png)

# SOLID

- **Single Responsibility Principle** (Принцип единственной ответственности).
- **Open-Closed Principle** (Принцип открытости-закрытости).
- **Liskov Substitution Principle** (Принцип подстановки Барбары Лисков).
- **Interface Segregation Principle** (Принцип разделения интерфейса).
- **Dependency Inversion Principle** (Принцип инверсии зависимостей).

## SRP

у модуля должна быть только одна причина для изменения

## Open-Closed Principle

модули должны быть открыты для расширения, но закрыты для изменения

- заставляет проектировать модули так, чтобы они делали только одну вещь
- побуждает связывать сущности через абстракции (а не реализацию)
- обращает внимание проектировщиков на места стыка и взаимодействие сущностей
- позволяет сократить количество кода, который необходимо менять при изменении бизнес-требований
- делает внесение изменений безопасным и относительно дешёвым

## Liskov Substitution Principle

классы-наследники могли бы использоваться вместо родительских классов, от которых они образованы, не нарушая работу программы

## Interface Segregation Principle

сущности не должны зависеть от интерфейсов, которые они не используют

## Dependency Inversion Principle

объектом зависимости должна быть абстракция, а не что-то конкретное

- модули верхних уровней не должны зависеть от модулей нижних уровней. Оба типа модулей должны зависеть от абстракций
- абстракции не должны зависеть от деталей. Детали должны зависеть от абстракций.

Http завивист от конкретной реализации XMLHttpService

```typescript
class XMLHttpService {}

class Http {
  constructor(xmlHttpService: XMLHttpService)
}
```

Необходимо связать сервисы через абстракцию

```typescript
interface Connection {
  request();
}

class XMLHttpService implements Connection {}

class Http {
  constructor(connection: Connection)
}
```

# Programming Principles

## KISS

keep it short and simple

- Не подключаете всю библиотеку, если нужна всего пара функций
- Не закладываете избыточные функции, если о них не просил заказчик
- Не используете избыточные классы и методы
- Не перегружаете интерфейс и не делаете сложную бизнес-логику
- Не выполняете другие действия, если они не влияют на работу проекта

## DRY

don’t repeat yourself

Проще вносить изменения в логику, проще тестировать, приводит к декомпозиции сложных алгоритмов на простые функции, что упрощает понимание программного кода, позволяет сократить время разработки и тестирования новой функциональности

Доступ к конкретному функционалу должен быть доступен в одном месте, унифицирован и сгруппирован по какому-либо принципу, а не «разбросан» по системе в произвольных вариациях

## YAGNI

you aren't gonna need it

Возможности, которые не описаны в требованиях к системе, просто не должны реализовываться

Заказчик не должен платить за то, что ему не надо, а продукт должен быть максимально сопровождаем и его качество не должно страдать от интеграции ненужных функций