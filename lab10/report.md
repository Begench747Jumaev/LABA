---
# Front matter
lang: ru-RU
title: " отчёта по лабораторной работе №10"
subtitle: "Eкстовой редактор emacs"
author: "Джумаев Бегенч"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
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

 Познакомиться с операционной системой Linux. Получить практические навы-ки работы с редактором Emacs.
 
#  Задание 1

1. Ознакомиться с теоретическим материалом.

2. Ознакомиться с редактором emacs.

3. Выполнить упражнения

4. Ответить на контрольные вопросы

## задание 2 Основные команды emacs

1. Открыть emacs.

2. Создать файл lab07.sh с помощью комбинации Ctrl-x Ctrl-f (C-x C-f).

3. Наберите текст: 

4. Сохранить файл с помощью комбинацииCtrl-xCtrl-s(C-x C-s).

5. Проделать с текстом стандартные процедуры редактирования, каждое действиедолжно осуществляться комбинацией клавиш. 5.1 .Вырезать одной командой целую строку (С-k). 5.2. Вставить эту строку в конец файла (C-y). 5.3. Выделить область текста (C-space). 5.4. Скопировать область в буфер обмена (M-w). 5.5. Вставить область в конец файла. 5.6. Вновь выделить эту область и на этот раз вырезать её (C-w). 5.7. Отмените последнее действие (C-/).

 6. Научитесь использовать команды по перемещению курсора.
 6.1. Переместите курсор в начало строки (C-a). 6.2. Переместите курсор в конец строки (C-e). 6.3. Переместите курсор в начало буфера (M-<). 6.4. Переместите курсор в конец буфера (M->).
 
 7. Управление буферами.
 7.1. Вывести список активных буферов на экран (C-x C-b). 7.2.Переместитесь во вновь открытое окно (C-x) o со списком открытых буфе-ров и переключитесь на другой буфер. 7.3. Закройте это окно (C-x 0). 7.4. Теперь вновь переключайтесь между буферами, но уже без вывода их спискана экран (C-x b).
 
 8. Управление окнами. 8.1.Поделите фрейм на 4 части: разделите фрейм на два окна по вертикали(C-x 3), а затем каждое из этих окон на две части по горизонтали (C-x 2)(см. рис.7.1).8.2.В каждом из четырёх созданных окон откройте новый буфер (файл) и вве-дите несколько строк текста.
  
9. Режим поиска 9.1.Переключитесьврежимпоиска(C-s)и найдите несколько слов,присутствующих в тексте.9.2.Переключайтесь между результатами поиска, нажимая C-s.9.3.Выйдите из режима поиска, нажавC-g.9.4.Перейдите в режим поиска и замены (M-%), введите текст, который следуетнайти и заменить, нажмитеEnter, затем введите текст для замены. После то-го как будут подсвечены результаты поиска, нажмите!для подтверждения замены.9.5.Испробуйте другой режим поиска, нажав M-s o. Объясните, чем он отлича-ется от обычного режима?


# Выполнение лабораторной работы 
   основные команды emacs
 
1.  Я открыл emacs. 

![](image/01.png){ #fig:001 width=70% }

2. Я cоздал файл lab10.sh с помощью комбинации Ctrl-x Ctrl-f (C-x C-f).
 
 ![](image/10.png){ #fig:001 width=70% }
 
 3. Я набрал текст:
 ```
  #!/bin/bash
  HELL=Hello
  function hello {
  LOCAL HELLO=World
  echo $HELLO
  }
  echo $HELLO 
  hello

  ```
 
 ![](image/02.png){ #fig:001 width=70% }
 
4. Я сохранил файл с помощью комбинации Ctrl-x Ctrl-s (C-x C-s)
  
![](image/03.png){ #fig:001 width=70% }

5. Я проделал с текстом стандартные процедуры редактирования, каждое действиедолжно осуществляться комбинацией клавиш.5.1.Я вырезал одной командой целую строку (С-k).5.2.Я вставил эту строку в конец файла (C-y).5.3.Я выделил область текста (C-space).5.4.Я скопировал область в буфер обмена (M-w).5.5.Я вставил область в конец файла.5.6.Я вновь выделить эту область и на этот раз вырезать её (C-w).5.7.я отменил последнее действие (C-/).

![](image/04.png){ #fig:001 width=70% }

![](image/05.png){ #fig:001 width=70% }

![](image/5.5.png){ #fig:001 width=70% }

![](image/5.6.1.png){ #fig:001 width=70% }

![](image/5.6.png){ #fig:001 width=70% }

![](image/5.7.png){ #fig:001 width=70% }

6. Я научился использовать команды по перемещению курсора.6.1.Я переместил курсор в начало строки (C-a).6.2.Я переместил курсор в конец строки (C-e).6.3.Я переместил курсор в начало буфера (M-<).6.4.Переместил курсор в конец буфера (M->).

![](image/6.1.png){ #fig:001 width=70% }

![](image/6.2.png){ #fig:001 width=70% }

![](image/6.3.png){ #fig:001 width=70% }

![](image/6.4.png){ #fig:001 width=70% }

7. Управление буферами.
 7.1.Я вывел список активных буферов на экран (C-x C-b).7.2.Я переместился во вновь открытое окно (C-x) o со списком открытых буфе-ров и переключился на другой буфер.7.3.Я закрыл это окно (C-x 0).7.4.Теперь вновь переключил между буферами, но уже без вывода их спискана экран (C-x b).

![](image/7.1.png){ #fig:001 width=70% }

![](image/7.2.png){ #fig:001 width=70% }

![](image/7.3.png){ #fig:001 width=70% }

![](image/7.4.png){ #fig:001 width=70% }

8. Управление окнами.
 8.1.Я поделил фрейм на 4 части: разделил фрейм на два окна по вертикали(C-x 3), а затем каждое из этих окон на две части по горизонтали (C-x 2). 8.2.В каждом из четырёх созданных окон откройте новый буфер (файл) и вве-дите несколько строк текста

![](image/8.1.png){ #fig:001 width=70% }

![](image/8.2.png){ #fig:001 width=70% }

9. Режим поиска 
 9.1.Я переключился в режим поиска (C-s) и нашел несколько слов,присутствующих в тексте.9.2.Я переключился между результатами поиска, нажимал C-s.9.3.Вышел из режима поиска, нажав C-g.9.4.Я перешел в режим поиска и замены (M-%), ввел текст, который следует найти и заменить, нажмите Enter, затем ввел текст для замены. После то-го как будут подсвечены результаты поиска,я нажал!для подтверждения замены. 9.5.Испробуйте другой режим поиска, нажав M-s o.

![](image/9.1.png){ #fig:001 width=70% }

![](image/9.4.png){ #fig:001 width=70% }

![](image/9.5.1.png){ #fig:001 width=70% }

![](image/9.5.2.png){ #fig:001 width=70% }

# Выводы

Я познакомился с операционной систомой Linux и получил практические навыки работы с редактором Emacs.

# Контрольные вопросы
1. Emacs представляет собой мощный экранный редактор текста, написанныйна языке высокого уровня Elisp.

2. Развитие Emacs в сторону его многогранности послужило причиной того,что и без того интуитивно непонятная программа стала чрезвычайно слож-ной в применении. В частности, управление осуществляется при помощиразличных клавиатурных комбинаций, запомнить которые будет непросто.

3. Буфер – что-то, состоящее из текста. Окно – область с одним из буферов.

4. В одном окне можно открыть больше 10 буферов.

5. После запуска emacs без каких-либо параметров в основном окне отобра-жается буферscratch, который используется для оценки выражений EmacsLisp, а также для заметок, которые вы не хотите сохранять. Этот буфер несохраняется автоматически.

6. Чтобы ввести следующую комбинацию C-c | я нажмуклавиши: Control+c иShift+, и для C-c C-|: Control+c и Control+Shift+.

7. Поделить текущее окно на две части можно двумя комбинациями клавиш:C-x 3 или C-x 2.

8. Настроить  или  расширить  Emacs  можно  написав  или  изменив  файл~/.emacs.

9. Клавиша ß выполняет функцию перемещения курсора в открытом окнетакже, как и многие другие клавиши её можно переназначить.

10. Редактор emacs показался мне удобнее из-за возможности открытиянескольких окон с буферами и работать комбинациями клавиш в этот23
редакторе мне было проще
  
