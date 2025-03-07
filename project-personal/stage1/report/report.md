---
## Front matter
title: "Отчет по индивидуальному проекту часть 1"
subtitle: "Дисциплина: Основы информационной безопасности"
author: "Зинченко Анастасия Романовна"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Целью данной работы является установка Kali


# Выполнение лабораторной работы

Указала имя виртуальной машины, тип операционной системы — Linux, Debian (64-bit)  (рис. [-@fig:001]).

![Имя виртуальной машины, тип операционной ситстемы](image/01.png){#fig:001 width=70%}

Указала размер основной памяти виртуальной машины (рис. [-@fig:002]).

![Размер основной памяти виртуальной машины](image/02.png){#fig:002 width=70%}

Задала размер диска — 40 ГБ (рис. [-@fig:003]).

![Размер диска](image/03.png){#fig:003 width=70%}

Выбрала язык (рис. [-@fig:004]).

![Язык](image/04.png){#fig:004 width=70%}

Выбрала местонахождения (рис. [-@fig:005]).

![Местонахождение](image/05.png){#fig:005 width=70%}

Настроила клавиатуру (рис. [-@fig:006]).

![Настройка клавиатуры](image/06.png){#fig:006 width=70%}

Настроила клавиатуру (рис. [-@fig:007]).

![Настройка клавиатуры](image/07.png){#fig:007 width=70%}

Ввела имя компьтера (рис. [-@fig:008]).

![Имя компьтера](image/08.png){#fig:008 width=70%}

Ввела имя домена (рис. [-@fig:009]).

![Имя домена](image/09.png){#fig:009 width=70%}

Создала учетную запись (рис. [-@fig:010]).

![Учётная запись](image/10.png){#fig:010 width=70%}

Выбрала имя пользователя (рис. [-@fig:011]).

![Имя пользователя](image/11.png){#fig:011 width=70%}

Придумала пароль (рис. [-@fig:012]).

![Пароль](image/12.png){#fig:012 width=70%}

Настроила время (рис. [-@fig:013]).

![Время](image/13.png){#fig:013 width=70%}

Произвела разметку дисков (рис. [-@fig:014]).

![Разметка дисков](image/14.png){#fig:014 width=70%}

Произвела разметку дисков (рис. [-@fig:015]).

![Разметка дисков](image/15.png){#fig:015 width=70%}

Произвела разметку дисков (рис. [-@fig:016]).

![Разметка дисков](image/16.png){#fig:016 width=70%}

Произвела разметку дисков (рис. [-@fig:017]).

![Разметка дисков](image/17.png){#fig:017 width=70%}

Произвела разметку дисков (рис. [-@fig:018]).

![Разметка дисков](image/18.png){#fig:018 width=70%}

Установила GRUB (рис. [-@fig:019]).

![GRUB](image/19.png){#fig:019 width=70%}

Установила GRUB (рис. [-@fig:020]).

![GRUB](image/20.png){#fig:020 width=70%}

Запуск (рис. [-@fig:021]).

![Запуск](image/21.png){#fig:021 width=70%}

# Выводы

В ходе выполнения лабораторной работы мы приобрели практические навыки установки Kali

# Список литературы{.unnumbered}

::: {#refs}
:::
