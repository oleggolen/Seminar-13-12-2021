# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.
## Подготовка репозитория
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
Для удаления ветки ввести команду "git branch -d 'name branch'"

## Внесенние изменений в удалённый репозиторий
*Пошаговая инструкция для создания Pull Request (внесения изменения) в удалённый репозиторий* - Для того, чтобы внести изменения в существующий, удалённый репозиторий (другого пользователя, команды, организации...) необходимо:

1. Найти необходимый репозиторий, в который хотим внести изменение; 

2. Сделать Fork этого репозитория в свой аккаунт на Github;

3. Копируем ссылку из своего репозитория и делаем клон **своей** версии в git (VSC). Делается при помощи командв *git clone*: 

    *git clone <ссылка на свой репозиторий>* 

4. Создаём новую ветку в файле и делаем в ней изменения, которые хотим предложить внести;

5. Сохраняем изменения, делаем commit;

6. Отправляем сохранённую версия на *свой* GitHub. Сделать это можно при помощи команды *git push*. Её надо просто написать в терминале. 

7. Обновляем свой репозиторий на Github, проверяем, появились ли обновления. 

8. Создаём pull reques. Для этого на Githud нижимаем кнопку *Pull requesr*. Можно добавить описание к тому, что было сделано, чтобы обладателю было понятно, что и зачем мы сделали. 
