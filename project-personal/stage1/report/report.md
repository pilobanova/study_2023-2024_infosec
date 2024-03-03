---
## Front matter
title: "Отчет по первому этапу индивидуального проекта"
subtitle: "Дисциплина: Основы информационной безопасности"
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

Установить Kali Linux на виртуальную машину VirtualBox.

# Выполнение лабораторной работы

1. Создаем новую виртуальную машину в VirtualBox, называем ее, выбираем тип операционной системы и версию.

![*Создание виртуальной машины.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/project-personal/stage1/report/image/этап 1/1.png){#fig:001 width=70%}

2. Выбираем объем основной памяти. Я выбрала 2048 МБ.

![*Объем основной памяти.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/project-personal/stage1/report/image/этап 1/2.png){#fig:001 width=70%}

3. Создаем новый жесткий диск и выбираем его размер (40 ГБ).

![*Новый жесткий диск.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/project-personal/stage1/report/image/этап 1/3.png){#fig:001 width=70%}

4. Добавляем в носители наш образ и запускам виртуальную машину.

![*Добавляем образ.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/project-personal/stage1/report/image/этап 1/4.png){#fig:001 width=70%}

5. Выбираем английский язык.

![*Выбор языка.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/project-personal/stage1/report/image/этап 1/5.png){#fig:001 width=70%}

6. Задаем имя хоста.

![*Название хоста.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/project-personal/stage1/report/image/этап 1/6.png){#fig:001 width=70%}

7. Задаем имя узла.

![*Название узла.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/project-personal/stage1/report/image/этап 1/7.png){#fig:001 width=70%}

8. Задаем имя пользователя. По заданию оно должно быть root.

![*имя пользователя.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/project-personal/stage1/report/image/этап 1/8.png){#fig:001 width=70%}

9. Устанавливаем пароль. 

![*Установка пароля.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/project-personal/stage1/report/image/этап 1/10.png){#fig:001 width=70%}

10. Выбираем часовой пояс.

![*Часовой пояс.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/project-personal/stage1/report/image/этап 1/11.png){#fig:001 width=70%}

11. Выбираем наш диск.

![*Выбор диска.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/project-personal/stage1/report/image/этап 1/12.png){#fig:001 width=70%}

12. Завершаем настройку виртуальной машины.

![*Настроенная виртуальная машина.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/project-personal/stage1/report/image/этап 1/13.png){#fig:001 width=70%}

# Выводы

Я установила дистрибутив Kali Linux на виртуальную машину для дальнейшего выполнения индивидуального проекта.

