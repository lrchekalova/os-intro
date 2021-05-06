---
# Front matter
lang: ru-RU
title: "Лабораторная работа №5"
subtitle: "Дисциплина: Операционные Системы"
author: "Чекалова Лилия Руслановна, ст. б. 1032201654"

# Formatting
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Прагматика выполнения работы

Прагматика выполнения данной лабораторной работы заключается в том, что научившись использовать командную строку, можно быстро работать с системой.

# Цель работы

Целью данной работы являлось приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.

# Задачи работы

Основными задачами работы были:

* Просмотр содержимого каталогов и переход между каталогами
* Создание и удаление каталогов
* Знакомство с возможностями командной строки

# Просмотр содержимого каталогов и переход между каталогами

Данный этап заключался в:

* Передвижении по файловой системе с помощью команды cd
* Использовании команды ls для просмотра содержимого каталогов
* Использовании опции -a команды ls для просмотра скрытых файлов
* Использовании опции -F команды ls для просмотра типов файлов
* Использовании опции -l команды ls для получения подробной информации о файлах

# Создание и удаление каталогов

На этом этапе выполнялись следующие действия:

* Создание каталогов newdir и morefun с помощью команды mkdir
* Удаление этих каталогов с помощью команды rmdir
* Создание одновременно трех каталогов одной командой mkdir
* Удаление одновременно трех каталогов одной командой rm с опцией -r
* Проверка наличия удаленных каталогов с помощью команды ls

# Знакомство с возможностями командной строки

Данный этап состоял из:

* Чтения справки по команде ls и поиска опций для выполнения нужных нам действий
* Чтения справки по командам cd, pwd, mkdir, rmdir и rm и изучения их опций
* Использования команды history для получения буфера команд
* Модифицирования и исполнения команд из буфера команд

# Результаты работы

В результате выполнения данной лабораторной работы мной были приобретены навыки взаимодействия с системой посредством командной строки: научилась выводить на экран содержимое каталогов, создавать и удалять каталоги, пользоваться справкой, модифицировать и использовать команды из буфера команд.

# Спасибо за внимание!