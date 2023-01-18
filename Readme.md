# Инструкция для работы с Git и удалёнными репозиториями
В последне время популярность git демонстрирует взрывной рост. Эта система контроля версий использвется различными проектами с открытым исходным кодом. 
## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.
## Основы
Git - это набор онсольных утилит, которые отслеживают и фиксируют изменения в файлах. Изначально Git был создан Линусом Торвальдсом при разработке ядра Linux. Однако инструмент так понравился разработчикам, что впоследствии он получил широкое распространение и его стали использовать в других проектах. С его помощью иожно сравнивать, анализировать, редактировать, сливать изменения и возвращаться назад к последнему сохранению. Этот процесс называется конролем версий, который, во-первых, позволяет отследить изменения, произошедшие с проектом со временем. Во-вторых, лн чрезвычайно мполезен при одновременной работе нескольких специалистов над одним проектом. 
## Установка Git
Прежде чем исполоьзовать Git, вы должны установить его на своем компьютере, что можно сделать из собранного пакета или другого установщика, либо скачать исходный код и скомпелировать его самомтоятельно. 
### Установка в Windows
Для установки Git в Windows имеется несколько способов. ОФициальная сборка доступна для скачивания на официальном сайте Git. Необходимо просто перейти на страницу https://git-scm.com/downloads, и загрузка запустится автоматически.
gitgit## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## Создание коммитов

### Git add
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

## Ветки в Git

### Создание ветки

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

## Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"git branch
