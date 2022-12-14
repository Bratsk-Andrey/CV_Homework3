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

Имя основной ветки Git-проекта по умолчанию - master.

### Создание ветки

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

## Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"

## Основные команды Git

<H2> <p style="text-align: center;"> Команды GIT </p> </H2>
<table>
<tr><th><p style="text-align: center;">Команда</th><th><p style="text-align: center;">Описание</th></tr>
<tr><th>init</th><th> Создаёт пустой репозиторий в текущем местоположении</th></tr>
<tr><th>status</th><th>Показывает текущее состояние репозитория</th></tr>
<tr><th>add</th><th>Добавляет файл к будущему коммиту</th></tr>
<tr><th>commit</th><th>Записывает коммит</th></tr>
<tr><th>commit -m "commit message"</th><th>Записывает коммит с сообщением</th></tr>
<tr><th>log</th><th>Просмотр истории коммитов</th></tr>
<tr><th>reflog</th><th>Просмотр истории действий. Пишет изменения не только commit'ов, но и всех операций, которые были совершены во время работы в репозитории</th></tr>
<tr><th>reset [хэш-код]</th><th>Сброс текущего состояния истории</th></tr>
<tr><th>revert</th><th>Отмена последствий коммита. Не сбрасывает состояние репозитория на конкретный commit, а она создаёт новый commit, который отменяет действие, совершенное в предыдущем</th></tr>
<tr><th>restore</th><th>Сброс состояния файла на указанное</th></tr>
<tr><th>branch</th><th>Управление ветками</th></tr>
<tr><th>checkout</th><th>Переключение веток</th></tr>
<tr><th>checkout -b [name branch]</th><th>Создание и переход на ветку</th></tr>
<tr><th>fetch</th><th>Подгружает обновления из репозитория</th></tr>
<tr><th>pull</th><th>Скачивает последние обновления ветки</th></tr>
<tr><th>push</th><th>Загружает в репозиторий локальные изменения</th></tr>
<tr><th>merge</th><th>Про слияние веток</th></tr>
<tr><th>clone url-адрес репозитория<></th><th>Клонирует внешний репозиторий на локальный ПК</th></tr>
<tr><th>pull</th><th>Получение изменений и слияние с локальной версией</th></tr>
<tr><th>push</th><th>Отправляет локальную версию репозитория на внешний</th></tr>
<tr><th>rebase</th><th>Перемещает мои изменения в тот или иной момент времени</th></tr>
</table>


<H2> <p style="text-align: center;"> Работа с удаленными репозиториями</p> </H2>

Команда **git clone** составная: она не только
загружает все изменения, но и пытается слить
все ветки на локальном компьютере и в
удаленном репозитории.

Команда **git pull** позволяет скачать все из текущего репозитория и автоматически
сделать merge с нашей версией.

Команда **git push** позволяет отправить нашу
версию репозитория на внешний репозиторий. ТРЕБУЕТ АВТОРИЗАЦИИ на внешнем репозитории.

