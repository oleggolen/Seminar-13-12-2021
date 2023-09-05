# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
>**Git** - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.[Гит на вики](https://ru.wikipedia.org/wiki/Git)
![git_image](https://res.cloudinary.com/practicaldev/image/fetch/s--kTEtBWYJ--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dev-to-uploads.s3.amazonaws.com/i/ka0rfekqburijjrb9yoh.png)

## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)
>**Репозиторий Git** — это виртуальное хранилище проекта. В нем можно хранить версии кода для доступа по мере необходимости.

## Создание коммитов
>**Git коммит** - снимок текущего состояния изменений, добавленных в раздел проиндексированных файлов.
![git_commit_example](https://www.brainstormcreative.co.uk/wp-content/uploads/view-unpushed-commits.png)

### Git add
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*
![git_add_example](https://media.geeksforgeeks.org/wp-content/uploads/20220915182823/GitAdd1.jpg)

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

## Ветки в Git
>**Git ветка** - это простой перемещаемый указатель на один из таких коммитов
![git_branch_image](data:image/png;base64,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)

### Создание ветки

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

## Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"
