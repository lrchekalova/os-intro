---
# Front matter
lang: ru-RU
title: "Лабораторная работа №6"
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

Прагматика выполнения данной лабораторной работы заключается в увеличении скорости работы с файлами и каталогами.

# Цель работы

Целью данной работы являлось ознакомление с файловой системой Linux, её структурой, именами и содержанием каталогов, а также приобретение практических навыков по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы.

# Задачи работы

Основными задачами работы были:

* Копирование, переименование и перемещение файлов и каталогов
* Изменение прав доступа к файлам
* Работа с файловыми системами

# Копирование, переименование и перемещение файлов и каталогов

Данный этап заключался в:

* Выполнении примеров из теоретического материала к лабораторной работе
* Копировании файлов с помощью команды cp и каталогов командой cp -r
* Создании файлов командой touch и каталогов командой mkdir
* Переименовывании и перемещении файлов и каталогов командой mv
* Просмотре файлов командой cat
* Проверке успешности выполнения операций с помощью команды ls

# Изменение прав доступа к файлам

На этом этапе выполнялись следующие действия:

* Выполнение примеров из теоретического материала к лабораторной работе
* Добавление владельцу файла/каталога прав доступа командой chmod u+rwx
* Лишение владельца файла/каталога прав доступа командой chmod u-rwx
* Просмотр содержимого файла с ограничением права на чтение
* Переход в каталог с ограничением права на выполнение
* Проверка успешности выполнения операций с помощью команды ls -l

# Работа с файловыми системами

Данный этап состоял из:

* Чтения справки по команде mount
* Анализа результатов выполнения команды mount
* Чтения справки по командам fsck, mkfs и kill

# Результаты работы

В результате выполнения данной лабораторной работы я познакомилась с файловой системой Linux и научилась применять команды для работы с файлами и каталогами, а также команды по управлению процессами, проверке использования диска и обслуживанию файловой системы, такие как cat, touch, cp, mv, chmod, mount и другими.

# Спасибо за внимание!