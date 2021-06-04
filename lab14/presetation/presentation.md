---
## Front matter
lang: ru-RU
title: "Средства, применяемые приразработке программного обеспечения в ОС типа UNIX/Linux"
author: |
	Джумаев Бегенч
date: 03.06.2021

## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---

# Цель работы

 Приобрести простейшие навыки разработки, анализа, тестирования и отладкиприложений в ОС типа UNIX/Linux на примере создания на языке программирова-ния С калькулятора с простейшими функциями.

         

## Создание подкаталога

![](image/01.png){#fig:001  dth=70%}
 
## Создание файлов

![](image/02.png){#fig:001  dth=70%}

## Реализация функций калькулятора в файле calculate.c

![](image/03.png){#fig:001  dth=70%}

## Реализация функций калькулятора в файле calculate.c

![](image/04.png){#fig:001  dth=70%}

## Интерфейсный файл calculate.h

 ![](image/05.png){#fig:001  dth=70%}
 
## Основной файл main.c

![](image/06.png){#fig:001  dth=70%}


## Команда gcc

![](image/07.png){#fig:001  dth=70%}

## Компиляция

![](image/08.png){#fig:001  dth=70%}

## Makefile

![](image/10.png){#fig:001  dth=70%}

## Отладчик GDB и run

![](image/11.png){#fig:001  dth=70%}

## Команда list

![](image/12.png){#fig:001  dth=70%}

## Команда list,точка остановка и информaция

![](image/13.png){#fig:001  dth=70%}

## Run, команда backtrace, Numeral и удаление точки останова

![](image/14.png){#fig:001  dth=70%}

## Анализ calculate.c

![](image/15.png){#fig:001  dth=70%}

## Анализ main.c

![](image/16.png){#fig:001  dth=70%}

## Вывод

 Изучал основы программирования в оболочке ОС UNIX, научилась писать бо-
лее сложные командные файлы с использованием логических управляющих
конструкций и циклов.

