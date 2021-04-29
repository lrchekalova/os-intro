---
# Front matter
lang: ru-RU
title: "Отчет по лабораторной работе №3"
author: "Чекалова Лилия Руслановна"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
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

# Цель работы

Научиться оформлять отчеты с помощью легковесного языка разметки Markdown.

# Задание

Сделать отчет по предыдущей лабораторной работе в Markdown.

# Выполнение лабораторной работы

Открываю шаблон отчета и меняю заголовок и авторство (рис. -@fig:001)

![Изменение заголовка и авторства](image/1.png){ #fig:001 width=70% }

Описываю цель и задание лабораторной работы (рис. -@fig:002)

![Описание цели и задания](image/2.png){ #fig:002 width=70% }

Описываю ход работы, делая ссылки на рисунки (рис. -@fig:003) (рис. -@fig:004)

![Описание хода работы](image/3.png){ #fig:003 width=70% }

![Папка с рисунками](image/4.png){ #fig:004 width=70% }

Добавляю вывод работы (рис. -@fig:005)

![Добавление вывода работы](image/5.png){ #fig:005 width=70% }

Сохраняю файл как report.md (рис. -@fig:006)

![Сохранение файла](image/6.png){ #fig:006 width=70% }

С помощью pandoc конвертирую md-файл в docx-файл и проверяю его наличие в папке (рис. -@fig:007)

![Конвертирование в docx-файл](image/7.png){ #fig:007 width=70% } 

Так же с помощью pandoc конвертирую md-файл в pdf-файл и проверяю его наличие в папке (рис. -@fig:008)

![Конвертирование в pdf-файл](image/8.png){ #fig:008 width=70% }

# Выводы

После выполнения данной лабораторной работы я приобрела навыки оформления отчетов с помощью языка Markdown.