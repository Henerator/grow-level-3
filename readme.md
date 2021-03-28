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

[CI/CD](#ci/cd)

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

[Dependency Injection](#dependency-injection)

[Network Optimizations](#network-optimizations)

[JS Performance Optimizations](#js-performance-optimizations)

[Critical Rendering Path](#critical-rendering-path)

[Repaint, Re-flow, Composition](#repaint-re-flow-composition)

[Memory Leaks](#memory-leaks)

[Angular optimizations](#angular-optimizations)

[Angular Ivy](#angular-ivy)

[Angular Change Detection](#angular-change-detection)

[React Optimizations](#react-optimizations)

[React Change Detection](#react-change-detection)

[Design Patterns](#design-patterns)

[OOP Principles](#oop-principles)

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

# CI/CD

Continuous Integration / Continuous Delivery

Набор принципов и практик, которые позволяют разработчикам чаще и надежнее развертывать изменения программного обеспечения

**CI** - упаковывает, тестирует сборки и оповещает об ошибках

**CD** - автоматизирует развертывание приложений в различные окружения

Непрерывная интеграция и непрерывная поставка нуждаются в непрерывном тестировании

## Инструменты для автоматического развертывания:

- Jenkins
- CircleCI
- AWS CodeBuild
- Azure DevOps
- Atlassian Bamboo
- Travis CI

## Этапы CD-конвейера:

- Получение кода из системы контроля версий и выполнение сборки
- Настройка инфраструктуры
- Копирование кода в целевую среду
- Настройка переменных окружения для целевой среды
- Развертывание компонентов приложения (веб-серверы, API-сервисы, базы данных)
- Выполнение дополнительных действий (e.g. перезапуск сервисов)
- Выполнение тестов и откат изменений окружения в случае провала тестов
- Логирование и отправка оповещений о состоянии поставки

Используют контейнеры (Docker) и системы оркестрации (Kubernetes)

Контейнеры позволяют стандартизировать упаковку, поставку и упростить масштабирование и уничтожение окружений с непостоянной нагрузкой

## Continuous Delivery vs Continuous Deployment

Шаги пайплайна:

- Source Control - внесение изменений в систему контроля версий
- Build - сборка приложения и прогон unit тестов
- Staging - деплой на тестовое окружение, прогон интеграционных, нагрузочных тестов
- Production - деплой на окружение с пользователями

Для **Continuous Deployment** все шаги будут выполнены автоматически если предыдущий шаг был успешным

Для **Continuous Delivery** перед деплоем на Production пайплайн остановится и будет ждать ручного подтверждения

![deliveryVSdeployment](https://farm66.staticflickr.com/65535/49717371863_2e5c1535e8_o.jpg)

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

## Code Smell

Запахи кода - это ключевые признаки необходимости рефакторинга

В процессе рефакторинга происходит избавление от запахов кода, что обеспечивает возможность дальнейшего развития приложения с той же или большей скоростью. Отсутствие регулярного рефакторинга с течением времени способно полностью парализовать проект, поэтому запахи кода необходимо устранять на ранних стадиях

- Дублирование кода
- Длинный метод
- Большой класс
- Длинный список параметров
- Расходящиеся модификации - при модификации в системе невозможно выделить определённое место, которое нужно изменить
- Стрельба дробью - при выполнении любых модификаций приходится вносить множество мелких изменений в большое число классов
- Завистливые функции - метод обращается к данным другого объекта чаще, чем к собственным данным
- Временное поле - поле, которые нужны объекту только при определённых обстоятельствах

# Dependency Injection

DI - идея работать с зависимостями вне зависимого класса

## Способы работы с зависимостями

### Создавать зависимости в зависимом классе

```typescript
class ClassA {
  classB: ClassB
  constructor() {
    this.classB = ClassB()
  }
}
```

- ClassA и ClassB тесно связаны друг с другом
- При любом изменении в инициализации класса ClassB потребуется корректировать код  внутри класса ClassA
- ClassA невозможно протестировать

### Внедрять зависимости через класс компонента

```typescript
class ComponentClass(){
    action() {
        const classC = ClassC();
        const classB = ClassB(classC);
        const classA = ClassA(classB);
        classA.action();
    }
}
```

- код компонента сложен
- нарушается SRP - компонет отвечает не только за свою работу, но и за внедрение зависимостей в зависимые классы

### Зависимости обрабатываются третьей стороной

```typescript
class DependencyManager {
  provideClassC() {
    return ClassC()
  }

  provideClassB(classC: ClassC) {
    return ClassB(classC)
  }

  provideClassA(classB: ClassB) {
    return ClassA(classB)
  }
}
```

# Network Optimizations

поисковые системы при ранжировании сайтов, начали учитывать скорость загрузки страницы

- Уменьшите количество HTTP-запросов

  - Использование CSS-спрайтов - комбинированное изображение
  - Использование Inline-картинок
  - Объединение нескольких файлов в один

- Помещайте CSS файлы в начале страницы - позволяет получить постепенный рендеринг страницы
- Помещайте javascript в конец страницы- загрузка скриптов начнется после загрузки контента и стилей
- Минимизируйте css и javascript
- Используйте поддомены для параллельного скачивания - по спецификации HTTP/1.1 накладывается ограничение: не более 2-х компонентов одновременно загружаемых с одного хоста
- Используйте кэш браузера - HTTP-заголовок Expires
- Используйте CDN (Content Delivery Network) - множество веб-серверов, разнесенных географически для достижения максимальной скорости отдачи контента клиенту
- Оптимизируйте ваши изображения
- Используейте отложенную загрузки изображений - не отображается, пока не находится в видимой области (loading="lazy")
- Не масштабируйте изображения - не загружайте изображение большего размера, чем необходимо отобразить
- Используйте Gzip-сжатие - заголовк Accept-Encoding: gzip
- HTTP 2.0 Server Push - настройка сервера, которая позволяет вместе с html сразу отправить необходимые css, js и другие ресурсы

## Metrics

- **FCP** (First Contentful Paint) — время между ответом сервера и появлением первого контента. До FCP пользователь видит белый экран.
- **SI** (Speed Index) — индекс скорости загрузки или как быстро на странице появляется контент при отрисовке в браузере.
- **LCP** (Largest Contentfull Paint) — время, за которое отрисовывается крупный контент на первом экране.
- **TTI** (Time to Interactive) — время до взаимодействия или время, через которое страница готова взаимодействовать с пользователем.
- **TBT** (Total Blocking Time) — общее время блокировки основного потока. Учитываются все длинные задачи от FCP до TTI, которые выполнялись дольше 50 миллисекунд.
- **CLS** (Cumulative Layout Shift) — показатель смещения элемента в процентах на странице во время загрузки. Смещение элементов из-за подгрузки рекламных блоков, изображений и шрифтов.

# JS Performance Optimizations

- Удаляйте неиспользуемый код и функционал
  - uglify
  - tree shaking
  - npm prune for modules
- Кэшируйте
  - Cache-Control: no-store - не кэшировать
  - Cache-Control: no-cache - кеш запрашивает сервер на предмет актуальности ресурса
  - Cache-Control: private - для отдельного пользователя
  - Cache-Control: public - могут использовать разные пользователи (e.g. в локальной сети)
- Выходит из циклов без лишних операций
- Избавляйтесь от повторных вычислений - сохраняйте значения в замыкании
- Минимизируйте доступ к DOM
- Минимизируйте исходный код - может уменьшить размер файлов на 60%
- Используйте throttle и debounce
- Не используйте delete - operator has performance negative effects for the V8 hidden classes pattern
- Используйте асинхронный код, чтобы предотвратить блокировку потоков
- Используйте Code Splitting - вначале отсылаете пользователю только самые необходимые модули
- Используйте async и defer - по умолчанию браузер ожидает загрузки скрипта перед обработкой страницы
  - **async** - страница не ждет async-скрипты, контент обрабатывается и отображается
    - fetched asynchronously
    - when it’s ready the HTML parsing is paused to execute the script, then it’s resumed.

  - **defer** - загружать скрипт после окончания рендеринга
    - fetched asynchronously
    - executed only after the HTML parsing is done
- Используйте Web Worker-ы для запуска ресурсоемких задач в фоне

## Obfuscation

приведение исходного кода к виду, сохраняющему её функциональность, но затрудняющему анализ

## Minification

комментарии, переносы строк, пробельные символы удаляются

# Critical Rendering Path

The set of steps browsers must take to convert HTML, CSS and JavaScript into living, breathing websites

1. Сделать запрос
1. Получить HTML-документ
1. Провести парсинг HTML на предмет включенных ресурсов
1. Построить DOM tree (document object model)
1. Отправить запросы критических ресурсов. CSS, блокирующий JS (параллельно с предыдущим пунктом)
1. Получить весь CSS-код
1. Построить CSSOM tree
1. Выполнить весь полученный JS-код. Здесь могут вызываться layout, если из js кода происходит форсирование reflow
1. Перестроить DOM tree (при необходимости)
1. Построить Render tree
1. Отрисовать страницу (layout → paint → Composite)
  - **layout** - determines where and how the elements are positioned on the page

# Repaint, Re-flow, Composition

1. HTML парсится и разбивается на токены
1. Токены преобразуются в Ноды
1. Ноды собираются в DOM (Domain Object Model) дерево
1. Параллельно с этим процессом происходит парсинг CSS правил и строится CSSOM (CSS Object Model)
1. CSSOM и DOM объединяются в Render Tree, в котором
    - скрываются невидимые элементы (meta, script, link и display: none)
    - добавляются элементы которых нет в DOM (псевдоэлементы :before, :after)
1. Происходит Reflow, Repaint и Composition

## Layout/Reflow

определяются координаты каждого элемента и пространство которое он занимает

> Определение размеров и местоположений элементов происходит не за один проход по дереву,
проход может происходить несколько раз, если элементы встречающиеся позже, влияют на предыдущие элементы

при каждом изменении свойства стиля, отвечающего за положение и размеры элемента,
происходит повторный процесс расчета размеров и положений

Reflow срабатывает
- при запросе метрики элемента через JS (e.g. getBoundingClientRect())
- при скроллинге
- прие запуске на выполнение событий

## Paint/Repaint

создает записи о том как будут отрисованы элементы на странице (позиция x,y, ширина, высота, цвет)

> если вы измените элементу свойство width, произойдет Reflow, а затем и Repaint затронутых элементов

## Composite

конечная отрисовка элементов на странице

группирует различные элементы по слоям, растрирует эти слои (отрисовывает пиксели)
и затем объединяет эти слои в готовую страницу в отдельном потоке композитора

# Memory Leaks

## Garbage Collector

Объект считается подлежащим уничтожению сборщиком мусора, если количество ссылок на него равно нулю

### Mark and sweep

Стартуя из глобального бъекта, сборщик мусора находит все доступные объекты и уничтожает недоступные

## Sources

- неиспользуемые объекты в замыкании
- циклические ссылки
- глобальные объекты - all global objects by definition never get collected
  - window
  - all variables exported by javascript modules
- подписки

## Detection

- performance tab of dev tools
- если есть подозрение на утечку конкретных объектов, в них добавляют большие свойства-маркеры (new Array(999999).join('leak'))
- 3 snapshot technique
  - F5 to get a clean state. Take a heap snapshot
  - perform some actions and bring the page roughly back to the same state. Take another heap snapshot
  - change the page’s state as much as possible. take a third heap snapshot
- this will show all objects that were created between snapshot 1 and 2 that are still around in snapshot 3

# Angular optimizations

## OnPush change detection strategy

By default Angular detects the changes in the application, within the tree of components. It starts by checking the root component, then its children.

With OnPush the change detection will check if the reference of the object passed to the chid component is changed (inputs are changed by reference)

## RunOutsideAngular

The zone is created by Zone.js which listens on async events and tells them to Angular.

Help to run a code outside the Angular zone without CD

## Pure pipes

A **pure** pipe is only called when Angular detects a change in the value or the parameters passed to a pipe

An **impure** pipe is called for every change detection cycle no matter whether the value or parameter(s) changes

## Trackby

If just one element was added into array Angular will destroy the previous DOM elements and recreates the DOM.

We can add **trackBy** parameter to say Angular to render the newly added item only

## Unsubscribe from Observables

If a subscription is not closed the function callback attached to it will be continuously called, this poses a huge memory leak and performance issue.

## Optimize template expressions

do not use functions in templates: the function will have to finish before other UI codes will be run

you can use Pipes instead

## AOT compilation

 - JIT compiles at runtime (выполняется каждый раз при запуске приложения в браузере)
 - AOT (ahead-of-time) compiles at build (выполняется один раз при сборке приложения)

 AOT produces only the compiled templates, and removes the Angular compiler from the deployment bundle
 (reduces app payload by around 1MB) and rendering time is increased significantly

 ### Pros

- компиляция шаблонов до сборки (выявление ошибок при сборке)
- более быстрый запуск приложения
- скомпилированный файл получается меньше (не нужно включать компилятор в сборку)
- вопрос безопасности (меньше вероятность внедрения)

## Lazy loading

split application to feature modules and load them on-demand

## Preloading Modules

Once application is loaded we can start loading other modules on the background

- Preload everything (PreloadAllModules)
- Don’t preload anything (NoPreloading)

## Resolve Guards

Send the required HTTP call within the Resolve Guard, which will load the next component only if the HTTP call returns success

# Angular Ivy

- уменьшает размер бандла - нет заводских файлов. все декораторы конвертируются в статические функции (@Component превращается в ngComponentDef)
- ускоряет компиляцию - позволяет пересобирать отдельные директивы (e.g. ngIf) вместо всего компонента
- упрощает дебаг - отображает источник ошибки, возникшей в темплейте

## Locality

compiler is only allowed to use information defined by a component decorator and its class

the current implementation requires a global static analysis of the entire application
and produces artifacts in the form of extra files `metadata.json` and `component.factory.js`

## Tree-Shaking

no longer ship the entire framework code, you only bundle pieces of the framework functionality that you use

# Angular Change Detection

- compiler analyzes the template
- identifies properties of a component that are associated with DOM elements
- for each association creates a binding in the form of instructions
- change detection mechanism executes instructions that process bindings

## Change Detection Reason

- we can use the Change Detector service to run change detection manually
- we can also rely on the framework to trigger change detection automatically
  - zone.js - patches all asynchronous events in a browser and notify Angular when a certain event occurs

# React Optimizations

## Memo

memoize/cache functional components

## PureComponent

memoize/cache class components

checks the fields of state and props to know whether the component should be updated

shallowly compares the fields of the previous props and state objects with the fields of the next props and state objects

## UseMemo

memoize value

## UseCallback

memoize function declarations

## Avoid inline function

Since functions are objects in JavaScript, the inline function will always fail the prop diff when React does a diff check

## React Fragment

group a list of children without adding an extra node

## Avoid using Index as Key

When you push or remove an item from the list, if the key is the same as before, React assumes that the DOM element represents the same component

## Avoiding props in initial states

> Using props to initialize a state in constructor function often leads to duplication of "source of truth". This is because constructor function is only invoked when the component is first created.

Don't initialize state with props which can be changed later. Instead, use props directly in the component.

## Avoid spreading props

is unnecessary and a bad practice

```JSX
<div {...props}></div>
```

## Using reselect selectors

As Redux practices immutability means new object references will be created every time on action dispatch

Reselect library encapsulates the Redux state and checks the fields of the state and tells React when to render or not if the fields haven’t changed

## Lazy loading

split application to feature modules and load them on-demand

## SSR

Server-side rendering provides performance benefit and consistent SEO performance.

Popular solutions:

- Next.js
- Gatsby

# React Change Detection

The core part of the change detection mechanism in React is Virtual DOM comparisons

- create a new Virtual DOM tree from a component
- comparing it to the previous version of the tree
- generating a patch to update the relevant parts of the DOM
- performing updates

## Change Detection Reason

There’s no way to trigger change detection automatically in React. Every change detection cycle starts with the call to the setState function

# Design Patterns

## Singleton

ensure that a class has only one instance, while providing a global access point to this instance

### Pros

- Гарантирует наличие единственного экземпляра класса
- Предоставляет к нему глобальную точку доступа
- Реализует отложенную инициализацию

### Cons

- Нарушает принцип единственной ответственности класса

## Builder

предлагает вынести конструирование объекта за пределы его класса

```typescript
class Director {
  construct(builder: Builder) {
    builder.reset()
    builder.setSeats(2)
    builder.setEngine(new SportEngine())
    builder.setTripComputer(true)
    builder.setGPS(true)
  }
}

class Application {
  makeCar() {
    const director = new Director()

    const carBuilder = new CarBuilder()
    director.constructSportsCar(carBuilder)
    const car = builder.getResult()

    const manualBuilder = new CarManualBuilder()
    director.constructSportsCar(manualBuilder)
  }
}
```

### Pros

- Позволяет создавать продукты пошагово
- Позволяет использовать один и тот же код для создания различных продуктов
- Изолирует сложный код сборки продукта от его основной бизнес-логики

### Cons

- Усложняет код программы из-за введения дополнительных классов
- Клиент будет привязан к конкретным классам строителей

## Abstract Factory

...

## Proxy

позволяет подставлять вместо реальных объектов специальные объекты-заменители, перехватываюющие вызовы к оригинальному объекту, позволяя выполнить дополнительные действия до или после передачи вызова оригиналу

> объект-заместитель, обрабоатывающий обращение к базе данных. Ленивая инициализация БД, кэширование запросов

> кредитная карта по отношению к наличным

> логирование обращений к объекту

## Flyweight

позволяет вместить бóльшее количество объектов в отведённую оперативную память, разделяя общее состояние объектов между собой, вместо хранения одинаковых данных в каждом объекте

```typescript
class TreeFactory {
  static treeTypes: TreeType[];
  static getTreeType(name, color, texture) {
    const type = treeTypes.find(name, color, texture)
    if (type == null)
      type = new TreeType(name, color, texture)
      treeTypes.add(type)
    return type
  }
}
```

## State

позволяет объектам менять поведение в зависимости от своего состояния

предлагает создать отдельные классы для каждого состояния, в котором может пребывать объект, а затем вынести туда поведения, соответствующие этим состояниям

В *Стратегии* объекты не знают друг о друге и никак не связаны. В *Состоянии* конкретные состояния могут переключать контекст

> действие кнопки телефона в различных состояниях (locked, unlocked, turned off)

## Strategy

определяет семейство схожих алгоритмов и помещает каждый из них в собственный класс, после чего алгоритмы можно взаимозаменять прямо во время исполнения программы

> прокладывание маршрута в навигаторе для разных видов траснпорта (машина, автобус, велосипед)

## Chain of Responsibility

позволяет передавать запросы последовательно по цепочке обработчиков

для каждой проверки создается отдельный класс с единственным методом выполнения

- прерывать дальнейшие проверки, если текущая проверка не прошла
- прерывать дальнейшую передачу, если найден обработчик для события

> автоответчик -> оператор -> специалист по определенной теме

## Command

превращает запросы в объекты, позволяя передавать их как аргументы при вызове методов, ставить запросы в очередь, логировать их, а также поддерживать отмену операций

> операции в редакторе кода (e.g. сохранение), выполняемые через различные UI элементы (кнопка в меню, контекстное меню, горячие клавиши)

```typescript
class Command {
  abstract execute() {}
}

class CopyCommand extends Command {
  execute() {
    doSomething()
  }
}
```

## Iterator

даёт возможность последовательно обходить элементы составных объектов, не раскрывая их внутреннего представления

идея в том, чтобы вынести поведение обхода коллекции из самой коллекции в отдельный класс

> разные варианты обхода коллекции (в глубину, в ширину)


# OOP Principles

## The Principle of Least Knowledge

1. Each unit should have only limited knowledge about other units
1. Each unit should only talk to its friends; don’t talk to strangers
1. Only talk to your immediate friends