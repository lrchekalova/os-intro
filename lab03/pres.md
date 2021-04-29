---
# Front matter
lang: ru-RU
title: "Лабораторная работа №3"
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

Прагматика выполнения данной лабораторной работы заключается в сокращении времени, отведенного на форматирование и оформление отчетов.

# Цель работы

Целью данной работы являлось приобретение навыков оформления отчетов с помощью легковесного языка разметки Markdown.

# Задачи работы

Основными задачами работы были:

* Подготовка отчета лабораторной работы №2
* Преобразование отчета с помощью языка Markdown
* Конвертация файлов

# Подготовка отчета лабораторной работы №2

Данный этап заключался в:

* Предварительном составлении отчета по лабораторной работе №2
* Сохранении необходимых скриншотов в папку images

# Преобразование отчета с помощью языка Markdown

На этом этапе выполнялись следующие действия:

* Настройка шрифтов и отступов
* Создание структуры отчета
    * Изменение авторства и заголовка
    * Описание цели, задания и вывода лабораторной работы
    * Описание хода работы с использованием ссылок на скриншоты из папки images

# Конвертация файлов

Данный этап состоял из:

* сохранения отчета в формате .md
* запуска pandoc
* конвертации md-файла в docx- и pdf-файлы
* проверки наличия полученных файлов в папке

# Результаты работы

В результате выполнения данной лабораторной работы мной были приобретены навыки оформления отчетов с помощью языка Markdown и составлен отчет в форматах docx и pdf.

# Спасибо за внимание!