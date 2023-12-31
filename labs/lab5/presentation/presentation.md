---
## Front matter
title: Лабораторная работа № 5
subtitle: Дискреционное разграничение прав в Linux. Исследование влияния дополнительных атрибутов.
author:
  - Кекишева А.Д.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 25 сентября 2023

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

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Кекишева Анастасия Дмитриевна
  * Бизнес-информатика
  * Кафедра теории веротности и кибербезопасности
  * Российский университет дружбы народов
  * 1032201194@pfur.ru
  * <https://github.com/adkekisheva>

:::
::: {.column width="30%"}

:::
::::::::::::::

# Цель работы

Изучение механизмов изменения идентификаторов, применения SetUID- и Sticky-битов. Получение практических навыков работы в консоли с дополнительными атрибутами. Рассмотрение работы механизма смены идентификатора процессов пользователей, а также влияние бита Sticky на запись и удаление файлов.

# Задание

Выполнить последовательность дейсвий, указанных в лабораторной работе, создавая программы и работая с битами (SetUID, SetGID, Sticky-бит), чтобы изучить влияние дополнительных атрибутов.

# Теоретическое введение

Рассмотрим некоторые команды, которые пригодяться нам в данной лабораторной.

- chown [ПАРАМЕТР]… [ВЛАДЕЛЕЦ][:[ГРУППА]] ФАЙЛ…
Эта команда позволяет сменить владельца и группу указанного ФАЙЛА на ВЛАДЕЛЬЦА и/или ГРУППУ.
- gcc [ИМЯ_ФАЙЛА].c -o [ИМЯ_ПРОГРАММЫ] 
Это команда поможет нам конвертировать файлы.

# Выполнение лабораторной работы

Изучение механики SetUID

# Шаг 1 - Создание программы simpleid.c

![Создание программы simpleid.c](image/1.jpg){#fig:001 width=90%}    

# Шаг 2 - Компиляция и запуск программы

![Компиляция и запуск программы](image/2.jpg){#fig:002 width=90%}     

# Шаг 3 - Написание программы simpleid2.c

![Написание программы simpleid2.c](image/3.jpg){#fig:003 width=90%}     

# Шаг 4 - Компиляция и запуск программы simpleid2

![Компиляция и запуск программы simpleid2](image/4.jpg){#fig:004 width=90%}     

# Шаг 5 - Компиляция и запуск программы

![Компиляция и запуск программы](image/5.jpg){#fig:005 width=90%}     

# Шаг 6 - Установка SetGID-бита

![Установка SetGID-бита](image/6.jpg){#fig:006 width=90%}     

# Шаг 7 - Создание и компиляция программы readfile.c

![Создание и компиляция программы readfile.c](image/7.jpg){#fig:007 width=90%}     

# Шаг 8 - Настройка прав для файла readfile.c

![Настройка прав для файла readfile.c](image/8.jpg){#fig:008 width=90%}     

# Шаг 9 - Чтение файла /etc/shadow с помощью программы readfile

![Чтение файла /etc/shadow с помощью программы readfile](image/9.jpg){#fig:009 width=90%}     

# Исследование Sticky-бита

# Шаг 1 - Проверка атрибута sticky и создание файла
 
![Проверка атрибута sticky и создание файла](image/10.jpg){#fig:010 width=90%}     

# Шаг 2 - Добавление прав остальным пользователям на чтение и запись

![Добавление прав остальным пользователям на чтение и запись](image/11.jpg){#fig:011 width=90%}     

# Шаг 3 - Проверка атрибута sticky и создание файла

![Проверка атрибута sticky и создание файла](image/12.jpg){#fig:012 width=90%}     

# Шаг 4 - Шаги без sticky-бита

![Шаги без sticky-бита](image/13.jpg){#fig:013 width=90%}     


# Выводы

Изучила механизмы изменения идентификаторов, применения SetUID- и Sticky-битов. Получила практические навыки работы в консоли с дополнительными атрибутами. Рассмотрела работы механизма смены идентификатора процессов пользователей, а также влияние бита Sticky на запись и удаление файлов.






