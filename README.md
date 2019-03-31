# Запуск проекта
Вам нужно скачать пакетный менеджер brew https://brew.sh/index_ru  
Затем с помощью него скачать cocoapods (brew install cocoapods)  
Затем в папке с проектом запустить команду pod install  
В проекте есть пример файла .swiftint.yml с правилами для проверки кода, которые использую я. Вас может это заинтересовать

# Домашка

## General  
Мои задания это чисто базовый пример. Если у вас есть идеи, реализуйте их, я проверю любой код. Главное чтобы задачи (например загрузка из сети или сохранение на диск) были выполнены

## 1) Star wars
Для домашнего задания предлагаю использовать https://swapi.co/ (любое другое открытое апи подойдет, я просто даю пример)
Минимальные ожидания - два экрана. Первый таблица с персонажами/фильмами, по нажатию на ячейку открывается второй экран с детальной информацией о персонаже/фильме. Есть кнопка закрыть или назад.

Дальнейшие изыскания:
- загрузить картинки на экране с деталями (аватарку фильма)
- задизайнить свою ячейку в таблице (добавить в нее аватарку)
- добавить несколько переходов (например на экране фильма показывать список кликабельных планет)
- впаять swiftlint
- удиви меня и получишь наклейку

Ответить на вопросы:
- Что такое SOLID?
- Что такое протокол? Отличие от класса?
- Что такое ARC? 
- В чем разница между weak и unowned?
- Расскажите про виды очередей в GCD?


## 2) Star wars extended
Я добавил в репозиторий проект TodoList. Он использует базу данных Realm, я привел примеры на базовые действия (попробуйте смахнуть ячейку влево или добавить нажав +). Можно попробовать https://github.com/stephencelis/SQLite.swift или CoreData, но Realm ИМХО легче всего для знакомства.  

Вы должны добавить в предыдущий проект работу с базой данных. Если интернет есть -> качаем, сохраняем базу, показываем. Если интернета нет, достаем из базы, показываем.

Дальнейшие изыскания:
- попробуйте создать ячейку отдельным Xib файлом
- поиграйтесь со стилями, научитесь менять шрифты, цвета, длину сепаратора в таблице. Попробуйте сделать это через код и через визуальный редактор
- реализовать и использовать в базе данных операции записи, чтения, поиска (например поиск по имени героя звездных войн)
- впаять swiftlint
- удиви меня и получишь наклейку

Ответить на вопросы:
- Что такое KISS и DRY?
- Что такое extension?
- Перечислите все способы работы с optional
- В чем разница Dependency Injection и Dependency Inversion? Пример?
- Что такое method dispatch? Какие типы бывают в свифте? (хардкор вопрос)

## 3) Autolayout pro

### Материлы
- Ссылка на интересный видос про autolayout: https://developer.apple.com/videos/play/wwdc2018/220  
- Ссылка на все то, что я рассказывал на лекции: https://developer.apple.com/library/archive/documentation/UserExperience/Conceptual/AutolayoutPG/index.html
- И по русски (меньше): https://habr.com/ru/company/oleg-bunin/blog/437584/
- И про метод диспатч: https://www.raizlabs.com/dev/2016/12/swift-method-dispatch/

### Домашка

Сделать копию дизайна калькулятора Apple. Нужно проверить, что верстка не едет на разных моделях айфонов. Логику счета реализовывать НЕ НУЖНО.
Все клавиши в landscape тоже не нужно, добавьте один столбик. Главное чтобы верстка была разной для portrait/landscape. Вам могут помочь size classes, о которых нужно почитать самим.

![Portrait](Pics/portrait.jpg)

![Landscape](Pics/landscape.jpg)

Дальнейшие изыскания (все это можно положить в одно приложение на разные экраны tabbar):
- сделать таблицу с динамической высотой ячеек (контент не важен)
- сделать что нибудь со scrollView (контент не важен). Например экран логина. Убедиться что кнопка доступна пользователю после показа клавиуатуры.

![Login](Pics/login.jpg)
- удиви меня и получишь наклейку (Я ОБЕЩАЮ В ЭТОТ РАЗ ТОЧНО)

Ответить на вопросы:
- Что такое size class? Какие есть?
- Как сделать self-sizing cell?
- Я хочу поменять констрейнты/добавить из кода. В каком методе UIViewController/UIView нужно это делать?
- Что такое autoresizing masks?
- В чем отличие pixel от point в ios?
- Что такое method dispatch? Какие типы бывают в свифте? (хардкор вопрос)