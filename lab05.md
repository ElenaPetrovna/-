## лабораторная работа №5

### *генераторы сайтов на примере Jekyll*

*Цель работы* — познакомиться с программами для генерации
статических сайтов на примере программы jekyll, научиться находить
шаблоны готовых сайтов и применять их.

Мы попробовали сделать простейший персональный сайт используя
только язык разметки Markdown. В этой лабораторной работе мы рассмотрим
инструменты позволяющие из этого же простого языка разметки
получить сайты, выглядящие и построенные вполне профессионально. Мы
ограничим возможности сайта тем что он будет состоять только из
статичных HTML страниц. Это значит, что у нас не будет серверной части с
бизнес-логикой и БД (базой данных), как например, во всех онлайновых
магазинах. Мы также не сможем принимать данные от пользователя —
для этого также нужно взаимодействовать с сервером, которого у нас
нет. Но все возможности на стороне клиента, в браузере пользователя,
а именно  язык разметки HTML, стили CSS, встроенный интерпретатор JavaScript
-- мы можем использовать как угодно.

Программ для генерации статических сайтов множество, есть даже
статический сайт для сравнения подобных статических генераторов:
<https://jamstack.org/generators/>. Авторы данного сайта называют многие плюсы такого
подхода. Во-первых, это скорость работы и доступность сайта. Дело в
том, что одним из следствий облачной революции в ИТ стало появление
сервиса CDN (Content Delivery Network). Этот сервис находит и размещает статичные
объекты — страницы, файлы изображений, скрипты и стили — как можно
ближе к потребителю, в идеальном варианте непосредственно на
серверах сетевого провайдера. Во-вторых, продвигаемый Jamstack подход
позволяет делать т. н. фронтэнд, логику страниц, сколь угодно сложным,
используя Javascript и API services, т. е. стандартных сервисов на облачных
серверах, заменяющих отчасти самодельные сервисы и позволяющих
реализовать возможности доступные ранее только самым продвинутым
приложениям.

На хостинге <https://pages.github.com/> недавно добавили возможность
использовать популярную программу jekyll — один из старейших
генераторов статических сайтов. Для вашего персонального сайта
вы можете выбрать одну из 12 доступных в настоящий момент тем. Затем
гитхаб автоматически построит сайт из сделанных вами markdown файлов и
выбранной темы. Для включения сервиса jekyll надо выполнить следующие
шаги в вашем гитхаб проекте:

    1. открыть созданный ранее репозитарий
    2. нажать опцию «Settings»
    3. пролистать до секции «GitHub Pages»
    4. выбрать тему
    5. убедиться, что появилось сообщение для вашего проекта и названия
    репозитария : *Your site is ready to be published at https://проект.github.io/репо/*
    6. открыть указанную ссылку, должен открыться шаблон сайта
    7. вернуться в репозитарий из п.1.
    8. в списке ветвей вашего репозитария должна появиться новая ветка gh-pages — переключитесь на неё
    9. начальный файл index.md из выбранной темы был показан на шаге 6.
    Вы готовы наполнить свой сайт реальными страницами.

Сайт <https://ophilon.github.io/blog/> был создан именно так. Вы можете сделать себе
копию этого сайта обычным способом — откройте мой репозитарий
<https://github.com/ophilon/blog> и скопируйте точно как любой другой публичный
проект.