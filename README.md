# gitTest


# Инструкция GIT

## При первом использовании Git необходимо представиться.  Для этого нужно ввести в терминале 2 команды:
* *git config --global user.name «Ваше имя английскими буквами»*  
* *git config --global user.email ваша почта@example.com*


 
## Создаем свой первый проект 

1. Создать директорю проекта
2. Внутри директори выполнить команду ***git init***
3. Создать текстовый файл **README.md**

## Отслеживание файлов

Чтобы Git отслеживал изменения файлов  проекта необходимо создать **commit.**

* Добавим все файлы проекта в нам будующий commit.
git add .
* Или git add --all

Если хотим добавить конкретный файл то 
* git add .\<имя_файла> 

Теперь создаем **commit.** Обязательно указываем комментарий.

* git commit -m "<комментарий>"

# Проверка статуса репозитория

Для проверки текущего состояния репозитория, просмотра списка измененных файлов используется команда
* **git status**


Для просмотра изменений в файлах команда
* **git diff**

# История изменений

Для просмтра истории изменений всех *commit* используется команда
* **git log**

Пример

commit 4f459bb9c05c64135367787842d36f5f8dfc93c9
Author: Zhanna <mail@ispolina.art>
Date:   Mon Nov 14 20:50:16 2022 +0300

    secomd commit

commit 2545e492b9335be300462e65914abcd67fe356af
Author: Zhanna <mail@ispolina.art>
Date:   Mon Nov 14 20:29:38 2022 +0300

    first commit

# Перемещение по истории 

Для востанвления любой сограненной версии репозитория применяют команду

* **git checkout 0000**

где 0000 - это первые 4 символа нужного вам идентификатора comit
В случае совпадения первых символов - добавьте еще один или два символа. 


## Возврат

Для возврата в актуальную версию репозитория применять когманду

* **git checkout master**


----------------------------------------------

## Работа с удаленным репозиторием ##

1. Открыть сайт GitHub. 

2. Открыть страницу репозитория, в который мы собираемся внести изменения

3. Создать Fork данного репозитория

4. Склонировать в VSCode командой git clone "ссылка на Fork"

5. Перейти в директорию репозитория cd

6. Bнести изменения. Сделать git commit -a

7. Запушить изменения в репозиторий Fork (Это мой репозиторий) командой git push 

8. Создать Pull Request на GitHub из нашей созданной ветки в репозитории Fork в целевую ветку репозитория от которого мы делали Fork

9. Ура. Ждем Merge