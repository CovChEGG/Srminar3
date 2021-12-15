# Инструкция по работе с Git и работе с ветками

## Что такое Git

**Git**- одна из реализаций распределённых систем контроля версий (**VCS**), имеющая как локальную версионность, так и версионность на сервере. **Git** является самой популярной системой контроля версий на сегодняшний день.  

## Подготовка репозитория

Для того, чтобы создать репоизиторий в выбранной папке используется комманада `git init`.
Для этого достаточно написать в терминале `git init` в папке с будущим репозиторием.

## Создание фиксаций

### Добавление файла к коммиту

Для того, чтобы добавить изменённый файл к новому коммиту (*сохранению*) необходимо использовать команду `git add`. Используется она сделующим образом: в папке с репозиторием пишем команду `git add <имя файла>`. 

### Создание коммитов

Для создания новой фиксации необходимо использовать комманду *git commit*. Используется она следующим образом: в папке с репозиторием вводится команда `git commit -m "<сообщение к комиту>"`. Все файлы коммита должны быть предварительно добавлены с помощью команды `git add` (либо добавлен ключ `-a` после команды *git commit*,например: `git commit -a -m "<сообщение к комиту>"` ).


### Просмотр информации об изменениях

Для того чтобы посмотреть информацию об изменения сделанных в текущей ветке необходимо использовать команду *`git status`*. Для этого достаточно использовать комманду *`git status`* в папке с репозиторием.

## Перемещение между сохранениями

Для перемещения между коммитами необходимо использовать команду *`git checkout`*. Используется она следующим образов в папке репозитори: *`git checkout <номер коммита>`*.

## Журнал изменений

Для просмотра журнала изменений необходимо использовать команду: *`git log`*. Для этого необходимо в папке с репоизторием дать команду *`git log`*.

## Ветки в Git

### Слияние веток

Для слияния веток используется команда *`git merge`*. Для этого сначала нужно перейти на ветку куда мы хотим произвести слияние с помощью комманды *`git checkout <имя ветки>`*. После этого применить команду *`git merge <имя ветки из которой будем производить слияние с той в которую перешли>`*.

### Просмотр списка веток

Для того, чтообы просмотреть список веткок необходимо использовать команду *`git branch`*. Для этого в папке с репозиторием надо набрать команду *`git branch`*

### Переход между ветками
  
Для того, чтобы перейти на дургую ветку необходимо использовать команду *`git checkout <название ветки>`*. Используется она в папке с репозиторием следующим образом: *`git checkout <название ветки>`*

Если вы хотите переместится в новую ветку, то необходимо с указанно командой использовать параметр *`-b`*, например: _`git checkout -b <название новой ветки>`_ 

### Удаление веток

Для удаления слитой ветки используется команда *`git branch -d "<имя ветки на удаление>"`*
