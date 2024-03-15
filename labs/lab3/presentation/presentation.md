---
## Front matter
lang: ru-RU
title: "Лабораторная работа №3"
subtitle: "Дисциплина: Основы информационной безопасности."
author:
  - Лобанова П. И.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 15 марта 2024

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Информация

## Докладчик


  * Лобанова Полина Иннокентьевна
  * Учащаяся на направлении "Компьютерные и информационные технологии"
  * Студентка группы НКАбд-01-22
  * [polla-2004@mail.ru](polla-2004@mail.ru)
  

# Цель

Получение практических навыков работы в консоли с атрибутами файлов для групп пользователей.

# Выполнение лабораторной работы

1. В установленной операционной системе создадим учётную запись пользователя guest. Поскольку мы уже делали это в прошлой лабораторной работе, такой пользователь у меня уже есть.

![*Создание пользователя guest.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/infosec/labs/lab3/report/image/лаба3/1.png){#fig:001 width=70%}

2. Аналогично создадим второго пользователя guest2.

![*Создание пользователя guest2.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/infosec/labs/lab3/report/image/лаба3/2.png){#fig:002 width=70%}

## .

3. Добавим пользователя guest2 в группу guest.

![*Добавление пользователя guest2 в группу guest.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/infosec/labs/lab3/report/image/лаба3/3.png){#fig:003 width=70%}

## .

4. Осуществим вход в систему от двух пользователей на двух разных консолях.

![*Консоли с двумя разными пользователями.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/infosec/labs/lab3/report/image/лаба3/4.png){#fig:004 width=70%}

## .

5. Для обоих пользователей командой pwd определим директорию, в которой находимся.

![*Директория пользователя guest.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/infosec/labs/lab3/report/image/лаба3/5.png){#fig:005 width=70%}

![*Директория пользователя guest2.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/infosec/labs/lab3/report/image/лаба3/6.png){#fig:006 width=70%}

## .

6. Уточним имя пользователя, его группу, кто входит в неё и к каким группам принадлежит он сам. Определим командами groups guest и groups guest2, в какие группы входят пользователи guest и guest2. Сравним вывод команды groups с выводом команд id -Gn и id -G.

![*Информация о пользователе guest.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/infosec/labs/lab3/report/image/лаба3/7.png){#fig:007 width=70%}

![*Информация о пользователе guest2.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/infosec/labs/lab3/report/image/лаба3/8.png){#fig:008 width=70%}

## .

7. Сравним полученную информацию с содержимым файла /etc/group.

![*Содержимое файла /etc/group.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/infosec/labs/lab3/report/image/лаба3/9.png){#fig:009 width=50%}

8. От имени пользователя guest2 выполним регистрацию пользователя guest2 в группе guest.

![*Регистрация пользователя guest2 в группе guest.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/infosec/labs/lab3/report/image/лаба3/10.png){#fig:010 width=70%}

## .

9. От имени пользователя guest изменим права директории /home/guest, разрешив все действия для пользователей группы.

![*Изменение прав директории /home/guest*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/infosec/labs/lab3/report/image/лаба3/11.png){#fig:011 width=70%}

## .

10. От имени пользователя guest снимем с директории /home/guest/dir1 все атрибуты.

![*Снятие всех атрибутов с директории /home/guest/dir1.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/infosec/labs/lab3/report/image/лаба3/12.png){#fig:012 width=70%}

## .

11. Меняя атрибуты у директории dir1 и файла file1 от имени пользователя guest и делая проверку от пользователя guest2, заполним табл. 3.1.

![*Таблица 3.1.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/infosec/labs/lab3/report/image/лаба3/13.png){#fig:013 width=30%}

## .

12. На основании заполненной таблицы определим те или иные минимально необходимые права для выполнения пользователем guest2 операций внутри директории dir1 и заполните табл. 3.2.

![*Таблица 3.2.*](/home/pilobanova/work/study/2023-2024/Основы информационной безопасности/infosec/labs/lab3/report/image/лаба3/14.png){#fig:014 width=70%}

# Вывод

Я получила практические навыки работы в консоли с атрибутами файлов для групп пользователей.
