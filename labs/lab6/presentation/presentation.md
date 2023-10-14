---
## Front matter
lang: ru-RU
title: Лабораторная работа №6
subtitle: Мандатное разграничение прав в Linux
author:
  - Кекишева А.Д.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 10 октября 2023

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

1. Развить навыки администрирования ОС Linux. Получить первое практическое знакомство с технологией SELinux1.
2. Проверить работу SELinx на практике совместно с веб-сервером Apache.

# Задание

Выполнить последовательность дейсвий описанных в лабораторной работе №6.


# Выполнение лабораторной работы

# Шаг 1

![Задание параметра](image/1.png){#fig:001 width=70%}

# Шаг 2

![Отключение пакетного фильтра и вход в систему](image/2.png){#fig:002 width=70%}

# Шаг 3

![Проверка статуса веб-сервера](image/3.png){#fig:003 width=70%}

# Шаг 4

![Список процессов](image/4.png){#fig:004 width=70%}
 
# Шаг 5

![Состояния переключателей](image/5.png){#fig:005 width=70%}

# Шаг 6

![Статистика - команда seinfo](image/6.png){#fig:006 width=70%}

# Шаг 7

![Определение типов файлов](image/7.png){#fig:007 width=70%}

# Шаг 8

![Файл test.html](image/8.png){#fig:008 width=70%}

# Шаг 9

![Отображение содержимого файла в браузере](image/9.png){#fig:009 width=70%}

# Шаг 10

![Команда man httpd_selinux - контексты для httpd](image/10.png){#fig:010 width=70%}

# Шаг 11

![Команда chcon](image/11.png){#fig:011 width=70%}

# Шаг 12

![Отказ в доступе - соообщение об ошибке от браузера](image/12.png){#fig:012 width=70%}

# Шаг 13

![Просмотр системых лог-фвйлов](image/13.png){#fig:013 width=70%}

# Шаг 14

![Изменение Listen 80 на Listen 81](image/14.png){#fig:014 width=70%}

# Шаг 15

![Перезапуск Apache](image/15.png){#fig:015 width=70%}

# Шаг 16

![Содержимое файла - /var/log/audit/audit.log](image/16.png){#fig:016 width=70%}

# Шаг 17

![Список портов](image/17.png){#fig:017 width=90%}

# Шаг 18

![перезапуск и изменение контекста](image/19.png){#fig:019 width=70%}

# Шаг 19

![Просмотр содеримого файла через браузер](image/19.png){#fig:019 width=70%}

# Шаг 20

![Исправление конфигурационный файл](image/20.png){#fig:020 width=70%}

# Шаг 21

![Удаление привязки к порту 81 и удаление файла](image/21.png){#fig:021 width=90%}


# Выводы

1. Развила навыки администрирования ОС Linux. 
2. Получила первое практическое знакомство с технологией SELinux1.
2. Проверила работу SELinx на практике совместно с веб-сервером Apache.


