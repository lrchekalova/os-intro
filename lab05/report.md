---
# Front matter
lang: ru-RU
title: "Отчет по лабораторной работе №5"
subtitle: "Дисциплина: Операционные системы"
author: "Чекалова Лилия Руслановна, ст.б 1032201654"

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

Приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.

# Выполнение лабораторной работы

Определяю полное имя моего домашнего каталога с помощью команды pwd (рис. -@fig:001)

![Полное имя домашнего каталога](image/1.png){ #fig:001 width=70% }

Перехожу в каталог /tmp с помощью команды cd и вывожу на экран его содержимое командой ls, ls -a (показывает также скрытые файлы), ls -F (показывает тип файла: * - исполняемый файл, / - каталог, @ - ссылка) и ls -l (показывает подробную информацию о файле: тип файла, право доступа, размер и т.д.) (рис. -@fig:002) (рис. -@fig:003) (рис. -@fig:004) (рис. -@fig:005)

![Вывод содержимого /tmp](image/2.png){ #fig:002 width=70% }

![Вывод содержимого /tmp со скрытыми файлами](image/3.png){ #fig:003 width=70% }

![Вывод содержимого /tmp с типами файлов](image/4.png){ #fig:004 width=70% }

![Вывод содержимого /tmp с подробной информацией о файлах](image/5.png){ #fig:005 width=70% }

Определяю, есть ли в каталоге /var/spool подкаталог с именем cron с помощью команды ls (рис. -@fig:006)

![Поиск подкаталога cron](image/6.png){ #fig:006 width=70% }

Перехожу в домашний каталог и вывожу на экран его содержимое командой ls. С помощью команды ls -l определяю, что владельцем файлов и подкаталогов является пользователь lrchekalova (рис. -@fig:007)

![Содержимое домашнего каталога](image/7.png){ #fig:007 width=70% }

Создаю в домашнем каталоге каталог newdir, а в нем подкаталог morefun с помощью команды mkdir (рис. -@fig:008)

![Создание каталогов newdir и morefun](image/8.png){ #fig:008 width=70% }

Создаю в домашнем каталоге каталоги letters, memos и misk и удаляю их с помощью команды rm -r (рис. -@fig:009)

![Создание и удаление каталогов](image/9.png){ #fig:009 width=70% }

Пробую удалить newdir командой rm и rmdir. Он не удаляется, потому что для удаления непустых каталогов нужны дополнительные опции (рис. -@fig:010) (рис. -@fig:011)

![Попытка удаления newdir](image/10.png){ #fig:010 width=70% }

![Проверка наличия newdir в домашнем каталоге](image/11.png){ #fig:011 width=70% }

Удаляю каталог ~/newdir/morefun (рис. -@fig:012)

![Удаление ~/newdir/morefun](image/12.png){ #fig:012 width=70% }

С помощью команды man определяю, какую опцию команды ls нужно использовать для просмотра содержимого не только указанного каталога, но и его подкаталогов - это опция -R или --recursive (рис. -@fig:013)

![Справка по команде ls -R](image/13.png){ #fig:013 width=70% }

С помощью команды man определяю, какую опцию команды ls нужно использовать для сортировки по времени последнего изменения выводимого списка содержимого с подробным описанием файлов - это опции -t (сортировка) и -l (подробное описание файлов) (рис. -@fig:014) (рис. -@fig:015)

![Справка по команде ls -t](image/14.png){ #fig:014 width=70% }

![Справка по команде ls -l](image/15.png){ #fig:015 width=70% }

С помощью команды man смотрю описание команды cd и ее основных опций: опция -P использует физическую структуру каталогов вместо следования символическим ссылкам, -L следует символическим ссылкам, а -e выдает сообщение об ошибке (рис. -@fig:016)

![Справка по команде cd](image/16.png){ #fig:016 width=70% }

С помощью команды man смотрю описание команды pwd и ее основных опций: опция -L позволяет использовать pwd, даже если полное имя файла содержит символические ссылки, -P избегает все символические ссылки, --version выводит информацию о версии файла (рис. -@fig:017)

![Справка по команде pwd](image/17.png){ #fig:017 width=70% }

С помощью команды man смотрю описание команды mkdir и ее основных опций: опция -m устанавливает права доступа для создаваемого каталога, -p создает при необходимости родительские директории для создаваемого каталога, -v выводит сообщение для каждой создаваемой директории (рис. -@fig:018)

![Справка по команде mkdir](image/18.png){ #fig:018 width=70% }

С помощью команды man смотрю описание команды rmdir и ее основных опций: опция -p удаляет указанную директорию и предшествующие ей каталоги, -v выводит диагностику для каждой обрабатываемой директории, --ignore-fail-on-non-empty игнорирует ошибки, связанные с тем, что удаляемый каталог не пустой (рис. -@fig:019)

![Справка по команде rmdir](image/19.png){ #fig:019 width=70% }

С помощью команды man смотрю описание команды rm и ее основных опций: опция -d удаляет пустую директорию, -r рекурсивно удаляет каталог и его содержимое, -i запрашивает подтверждение перед каждым удалением (рис. -@fig:020)

![Справка по команде rm](image/20.png){ #fig:020 width=70% }

Используя информацию, полученную при выполнении команды history, выполняю модификацию и исполнение нескольких команд из буфера команд (рис. -@fig:021) (рис. -@fig:022) (рис. -@fig:023)

![Результат исполнения команды history](image/21.png){ #fig:021 width=70% }

![Выполнение команды cd из буфера команд](image/22.png){ #fig:022 width=70% }

![Модификация команды ls -a](image/23.png){ #fig:023 width=70% }

# Выводы

После выполнения данной лабораторной работы я приобрела навыки взаимодействия с системой посредством командной строки: научилась выводить на экран содержимое каталогов, создавать и удалять каталоги, пользоваться справкой, модифицировать и использовать команды из буфера команд.

# Библиография

1. Курячий Г.В., Маслинский К.А. Операционная система Linux. - М.: Интуит.Ру, 2005
2. Курячий Г.В. Операционная система UNIX. - М.: Интуит.Ру, 2004
