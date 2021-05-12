---
# Front matter
lang: ru-RU
title: "Отчет по лабораторной работе №8"
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

Освоение основных возможностей командной оболочки Midnight Commander, приобретение навыков практической работы по просмотру каталогов и файлов и манипуляций с ними.

# Выполнение лабораторной работы

Midnight Commander (или mc) — псевдографическая командная оболочка для UNIX/Linux систем, то есть интерфейс взаимодействия пользователя с операционной системой и программным обеспечением посредством команд. Для запуска mc необходимо в командной строке набрать mc и нажать enter.

Читаю справку по mc, вызвав в командной строке man mc (рис. -@fig:001)

![Справка по mc](image/1.png){ #fig:001 width=70% }

Запускаю mc из командной строки (рис. -@fig:002)

![Запуск mc](image/2.png){ #fig:002 width=70% }

Выполняю несколько операций в mc: переключаюсь между левой и правой панелями с помощью комбинации клавиш ctrl + u (рис. -@fig:003) (рис. -@fig:004)

![Переключение между панелями (1)](image/3.png){ #fig:003 width=70% }

![Переключение между панелями (2)](image/4.png){ #fig:004 width=70% }

Копирую файл pres.md клавишей f5 (рис. -@fig:005)

![Копирование файла](image/5.png){ #fig:005 width=70% }

Перемещаю файл pres.md в папку presentation под именем presentation.md с помощью клавиши f6 (рис. -@fig:006)

![Перемещение файла с переименовыванием](image/6.png){ #fig:006 width=70% }

Удаляю файл presentation.md нажатием клавиши f8 (рис. -@fig:007)

![Удаление файла](image/7.png){ #fig:007 width=70% }

Выполняю основные команды меню правой панели - команды Дерево и Информация. Дерево выводит структуру дерева каталогов, а Информация выводит сведения о файле и текущей файловой системе, расположенных на активной панели: имя, права доступа, размер, дату последнего изменения, дату последнего открытия и другое (рис. -@fig:008) (рис. -@fig:009)

![Использование команды Дерево](image/8.png){ #fig:008 width=70% }

![Использование команды Информация](image/9.png){ #fig:009 width=70% }

Используя возможности подменю Файл, просматриваю содержимое текстового файла 1.txt (рис. -@fig:010)

![Просмотр содержимого файла](image/10.png){ #fig:010 width=70% }

Редактирую содержимое текстового файла (без сохранения результата) (рис. -@fig:011)

![Редактирование содержимого файла](image/11.png){ #fig:011 width=70% }

Создаю новый каталог txt и копирую туда файл (рис. -@fig:012) (рис. -@fig:013)

![Создание нового каталога](image/12.png){ #fig:012 width=70% }

![Копирование файла](image/13.png){ #fig:013 width=70% }

С помощью средств подменю Команда осуществляю поиск в файловой системе файла с расширением .c, содержащего строку main (рис. -@fig:014)

![Поиск файла](image/14.png){ #fig:014 width=70% }

Выбираю и повторяю одну из предыдущих команд с помощью команды История командной строки (я осуществила переход в домашний каталог) (рис. -@fig:015) (рис. -@fig:016)

![История командной строки](image/15.png){ #fig:015 width=70% }

![Переход в домашний каталог](image/16.png){ #fig:016 width=70% }

Анализирую файл меню и файл расширений с помощью команд Редактирование файла меню и Редактирование файла расширений. В файле меню описываются пункты меню пользователя - команды, доступные для выполнения, а в файле расширений указываются расширения файлов и применимые к ним команды (рис. -@fig:017) (рис. -@fig:018)

![Редактирование файла меню](image/17.png){ #fig:017 width=70% }

![Редактирование файла расширений](image/18.png){ #fig:018 width=70% }

В подменю Настройки изучаю команды, определяющие структуру экрана mc - меняю способ разбиения панелей и убираю отображение командной строки (рис. -@fig:019)

![Настройка структуры экрана mc](image/19.png){ #fig:019 width=70% }

В командной строке создаю текстовый файл text.txt с помощью команды touch (рис. -@fig:020)

![Создание файла](image/20.png){ #fig:020 width=70% }

Открываю его в текстовом редакторе mc (рис. -@fig:021)

![Открытие файла в текстовом редакторе mc](image/21.png){ #fig:021 width=70% }

Вставляю в файл скопированный из Интернета фрагмент текста, разделив его на несколько строк (рис. -@fig:022)

![Создание файла](image/22.png){ #fig:022 width=70% }

Используя горячие клавиши, выполняю несколько действий. Удаляю строку текста с помощью комбинации клавиш ctrl + y (рис. -@fig:023)

![Удаление строки](image/23.png){ #fig:023 width=70% }

Выделяю фрагмент текста с помощью клавиши f3 и копирую его на новую строку клавишей f5 (рис. -@fig:024) (рис. -@fig:025)

![Выделение фрагмента текста](image/24.png){ #fig:024 width=70% }

![Копирование фрагмента текста на новую строку](image/25.png){ #fig:025 width=70% }

Выделяю фрагмент текста с помощью клавиши f3 и перемещаю его на новую строку клавишей f6 (рис. -@fig:026)

![Перемещение фрагмента текста на новую строку](image/26.png){ #fig:026 width=70% }

Сохраняю файл нажатием клавиши f2 (рис. -@fig:027)

![Сохранение файла](image/27.png){ #fig:027 width=70% }

Отменяю последние действия - сохранение файла и перемещение фрагмента текста - сочетанием клавиш ctrl + u (рис. -@fig:028)

![Отмена последних действий](image/28.png){ #fig:028 width=70% }

Перехожу в конец файла с помощью комбинации клавиш ctrl + end и записываю текст (рис. -@fig:029)

![Запись текста в конце файла](image/29.png){ #fig:029 width=70% }

Перехожу в начало файла с помощью комбинации клавиш ctrl + home и записываю текст (рис. -@fig:030)

![Запись текста в начало файла](image/30.png){ #fig:030 width=70% }

Открываю файл с исходным текстом на c++. В данный момент включена подстветка синтаксиса (рис. -@fig:031)

![Файл с исходным текстом на c++](image/31.png){ #fig:031 width=70% }

Отключаю подстветку синтаксиса с помощью меню редактора (рис. -@fig:032)

![Отключение подстветки синтаксиса](image/32.png){ #fig:032 width=70% }

# Выводы

После выполнения данной лабораторной работы я изучила возможности командной оболочки Midnight Commander, такие как создание новых каталогов, просмотр, копирование, перемещение и редактрирование файлов, просмотр информации о файлах и каталогах, а также приобрела навыки работы с файлами с помощью текстового редактора mc.

# Библиография

1. Колисниченко Д.Н. Linux: От новичка к профессионалу. - СПб.: БХВ-Петербург, 2018
2. Midnight Commander: команды и горячие клавиши. - http://mydebianblog.blogspot.com/2011/01/midnight-commander.html
3. Горячие клавиши в mcedit. - https://any-key.net/mcedit-hotkeys
