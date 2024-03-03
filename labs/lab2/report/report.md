---
## Front matter
title: "Отчет по лабораторной работе №2"
subtitle: "Дисциплина: Основы информационной безопасности."
author: "Лобанова Полина Иннокентьевна"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Получение практических навыков работы в консоли с атрибутами файлов, закрепление теоретических основ дискреционного разграничения доступа в современных системах с открытым кодом на базе ОС Linux.

# Выполнение лабораторной работы

1. В установленной при выполнении предыдущей лабораторной работы операционной системе создаем учётную запись пользователя guest.

![*Создание нового пользователя.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/1.png){#fig:001 width=70%}

2. Задаем пароль для пользователя guest.

![*Запись пароля.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/2.png){#fig:001 width=70%}

3. Входим в систему от имени пользователя guest.

![*Смена пользователя.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/3.png){#fig:001 width=70%}

4. Определяем директорию, в которой вы находитесь, командой pwd. Она совпадает с приглашением командной строки, но не является домашней директорией, поэтому переходим в нее.

![*Командой pwd.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/4.png){#fig:001 width=70%}

5. Уточняем имя вашего пользователя командой whoami.

![*Проверка пользователя.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/5.png){#fig:001 width=70%}

6. Уточняем имя вашего пользователя, его группу, а также группы, куда входит пользователь, командой id. Сравниваем вывод id с выводом команды groups, они совпадают.

![*Команда id.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/6.png){#fig:001 width=70%}

![*Команда groups.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/7.png){#fig:001 width=70%}

7. Сравниваем полученную информацию об имени пользователя с данными, выводимыми в приглашении командной строки. Они совпадают.

8. Просмотрим файл /etc/passwd и сравним найденные данные с полученными в предыдущих пунктах. Они тоже совпадают.

![*Команда echo.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/9.png){#fig:001 width=70%}

9. Определим существующие в системе директории. Нам удалось ли вам получить список поддиректорий директории /home. 

![*Команда ls -l.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/10.png){#fig:001 width=70%}

10. Проверим какие расширенные атрибуты установлены на поддиректориях, находящихся в директории /home.

![*Команда lsattr.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/11.png){#fig:001 width=70%}

11. Создадим в домашней директории поддиректорию dir1. Определим командами ls -l и lsattr, какие права доступа и расширенные атрибуты были выставлены на директорию dir1.

![*Создание директории.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/12.png){#fig:001 width=70%}

![*Команда ls -l.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/13.png){#fig:001 width=70%}

![*Команда lsattr.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/14.png){#fig:001 width=70%}

12. Снимем с директории dir1 все атрибуты и проверим с её помощью правильность выполнения команды
ls -l.

![*Снятие прав.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/15.png){#fig:001 width=70%}

13. Попытайтесь создать в директории dir1 файл file1. Поскольку мы только что сняли все права для всех пользователей, у нас не получилось это сделать. В сообщении об ошибке говориться, что нам отказано в доступе и файл не создался.

![*Попытка создать файл.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/16.png){#fig:001 width=70%}

14. Заполним таблицу «Установленные права и разрешённые действия», выполняя действия от имени владельца директории (файлов), определив опытным путём, какие операции разрешены, а какие нет. Если операция разрешена, занесите в таблицу знак «+», если не разрешена, знак «-».

![*«Установленные права и разрешённые действия».*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/17.png){#fig:001 width=70%}

15. На основании заполненной таблицы определим те или иные минимально необходимые права для выполнения операций внутри директории dir1, заполнив табл. 2.2.

![*«Минимально необходимые права для выполнения операций».*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/labs/lab2/report/image/лаба 2/18.png){#fig:001 width=70%}

# Выводы

Я получила практические навыки работы в консоли с атрибутами файлов.
