# Инструкция по работе с git репозиторием

## Для начала работы
git init

Усли имя пользователя и почиа ещё не были заданы
git config --global user.name
git config --global user.emeil


## Работа с файлами

Для того чтобы добавить файл, нужно:
1. git add file_name
    добавляем файл с именем file_name для отслеживания
2. git commit -m "some message"

    добавляем текущие изменения в репозиторий и подлписываем их с помощью тега -m
    если добавить тег -a, то к коммиту добавятся все измененные файлы которые отслеживались

Чтобы отследить состояние репозитория:
1. git status
2. git log
3. git diff


## Работа с коммитами
Для того чтобы перейти к определеннму коммиту можно использовать команду
git checkout code_commit
    code commit - код коммита к которому хотим перейти, его можно посмотрить в git log

Чтобы вернуться к самому последнему состоянию

git checkout master

![batman](batman.jpg)


## Ветки в git
Чтобы посмотреть все ветки:
> git branch

для создания новой веткис именеи branch_name:
> git branch branch_name

Переместиться к ветке с именем branch_name:
> git checkout branch_name

## Удаление веток
Для того чтобы удалить ветку с именем branch_name:
> git branch -d branch_name

Удаление с игнорированием ошибок:
> git branch -D branch_name