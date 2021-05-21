---
# Front matter
lang: ru-RU
title: "Отчет по лабораторной работе №10"
subtitle: "Дисциплина: Операционные системы"
author: "Чекалова Лилия Руслановна, ст.б. 1032201654"

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

Знакомство с операционной системой Linux и получение практических навыков работы с редактором Emacs.

# Выполнение лабораторной работы

Открываю редактор Emacs (рис. -@fig:001)

![Запуск emacs](image/1.png){ #fig:001 width=70% }

Создаю файл lab10.sh с помощью комбинации клавиш ctrl-x ctrl-f (рис. -@fig:002)

![Создание файла](image/2.png){ #fig:002 width=70% }

Ввожу текст (рис. -@fig:003)

![Ввод текста](image/3.png){ #fig:003 width=70% }

Сохраняю файл с помощью комбинации клавиш ctrl-x ctrl-s (рис. -@fig:004)

![Сохранение файла](image/4.png){ #fig:004 width=70% }

Начинаю редактирование файла: вырезаю целую строку командой ctrl-k (рис. -@fig:005)

![Вырезание строки](image/5.png){ #fig:005 width=70% }

Вставляю эту строку в конец файла командой ctrl-y (рис. -@fig:006)

![Вставка строки](image/6.png){ #fig:006 width=70% }

Выделяю область текста комбинацией клавиш ctrl-space и стрелочками (рис. -@fig:007)

![Выделение области текста](image/7.png){ #fig:007 width=70% }

Копирую фрагмент текста в буфер обмена командой alt-w (alt здесь используется вместо клавиши meta) и вставляю его в конец файла командой ctrl-y (рис. -@fig:008)

![Копирование и вставка текста](image/8.png){ #fig:008 width=70% }

Вновь выделяю область текста и вырезаю его комбинацией клавиш ctrl-w (рис. -@fig:009)

![Вырезание текста](image/9.png){ #fig:009 width=70% }

Отменяю последнее действие командой ctrl-/ (рис. -@fig:010)

![Отмена последнего действия](image/10.png){ #fig:010 width=70% }

Перемещаю курсор в начало строки командой ctrl-a (рис. -@fig:011)

![Перемещение курсора в начало строки](image/11.png){ #fig:011 width=70% }

Перемещаю курсор в конец строки командой ctrl-e (рис. -@fig:012)

![Перемещение курсора в конец строки](image/12.png){ #fig:012 width=70% }

Перемещаю курсор в начало буфера командой alt-shift-< (рис. -@fig:013)

![Перемещение курсора в начало буфера](image/13.png){ #fig:013 width=70% }

Перемещаю курсор в конец буфера командой alt-shift-> (рис. -@fig:014)

![Перемещение курсора в конец буфера](image/14.png){ #fig:014 width=70% }

Вывожу список активных буферов на экран командой ctrl-x ctrl-b (рис. -@fig:015)

![Список активных буферов](image/15.png){ #fig:015 width=70% }

Перемещаюсь в окно со списком буферов командой ctrl-x o и переключаюсь на другой буфер (рис. -@fig:016)

![Переключение на другой буфер с помощью списка](image/16.png){ #fig:016 width=70% }

Закрываю это окно комбинацией клавиш ctrl-x 0 (рис. -@fig:017)

![Закрытие окна](image/17.png){ #fig:017 width=70% }

Переключаюсь между буферами с помощью команды ctrl-x b (рис. -@fig:018)

![Переключение на другой буфер командой](image/18.png){ #fig:018 width=70% }

Разделяю фрейм на 4 части: на два окна по вертикали с помощью команды ctrl-x 3 и затем каждое окно на две части по горизонатли командой ctrl-x 2 (рис. -@fig:019)

![Разделение фрейма](image/19.png){ #fig:019 width=70% }

Открываю в каждом окне новый буфер с помощью комбинации клавиш ctrl-x ctrl-f (рис. -@fig:020)

![Открытие новых буферов](image/20.png){ #fig:020 width=70% }

В каждый из буферов ввожу несколько строчек текста (рис. -@fig:021)

![Ввод текста в каждый из буферов](image/21.png){ #fig:021 width=70% }

Переключаюсь в режим поиска с помощью клавиш ctrl-s и осуществляю поиск слова "новый" (рис. -@fig:022)

![Поиск слова](image/22.png){ #fig:022 width=70% }

Осуществляю поиск слова "текст" и переключаюсь между результатами поиска клавишами ctrl-s (рис. -@fig:023) (рис. -@fig:024)

![Переключение между результатами (1)](image/23.png){ #fig:023 width=70% }

![Переключение между результатами (2)](image/24.png){ #fig:024 width=70% }

Выхожу из режима поиска командой ctrl-g (рис. -@fig:025)

![Выход из режима поиска](image/25.png){ #fig:025 width=70% }

Перехожу в режим поиска и замены комбинацией клавиш alt-shift-%, ввожу слово, которое нужно заменить и нажимаю enter (рис. -@fig:026)

![Ввод текста для замены (1)](image/26.png){ #fig:026 width=70% }

Ввожу слово, на которое нужно произвести замену (рис. -@fig:027)

![Ввод текста для замены (2)](image/27.png){ #fig:027 width=70% }

На экране выделяется найденный текст (рис. -@fig:028)

![Результат поиска для замены](image/28.png){ #fig:028 width=70% }

Подтверждаю замену клавишами shift-! (рис. -@fig:029)

![Результат замены](image/29.png){ #fig:029 width=70% }

Перехожу в другой режим поиска с помощью клавиш alt-s (рис. -@fig:030)

![Другой режим поиска текста](image/30.png){ #fig:030 width=70% }

Данный режим отличается от ctrl-s тем, что он не выделяет результат цветом, а ставит курсор после найденного слова (рис. -@fig:031)

![Результат поиска](image/31.png){ #fig:031 width=70% }

# Выводы

После выполнения данной лабораторной работы я научилась с помощью горячих клавиш создавать файлы, вырезать, вставлять, выделять и копировать фрагменты текста, перемещать курсор, осуществлять поиск и замену, управлять буферами и окнами редактора Emacs.

# Библиография

1. Emacs: основные сочетания клавиш: https://gist.github.com/ulysses4ever/68f8eb09a45f78fd2be096aa03813d78
2. Теоретические материалы к лабораторной работе: https://esystem.rudn.ru/pluginfile.php/1142229/mod_resource/content/3/007-lab_emacs.pdf