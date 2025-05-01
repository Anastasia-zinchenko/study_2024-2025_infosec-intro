---
## Front matter
title: "Отчёт по выполнению 4-ого этапа индивидуального проекта"
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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
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

Научиться тестировать приложения с помощью сканера nikto

# Задание

Ипспользование nikto

# Выполнение лабораторной работы

Чтобы работать с nikto, необходимо полготовить веб-приложение, которое будем сканировать запустила apache2 (рис. [-@fig:001]).

![Запуск apache2](image/001.png){#fig:001 width=70%}

Ввожу в адресной строке браузера адрес DVWA, перехожу в режим выбора уровня безопасности, ставлю минимальный (рис. [-@fig:002]).

![Запуск DVWA](image/002.png){#fig:002 width=70%}

Запускаю nikto (рис. [-@fig:003]).

![Запуск nikto](image/003.png){#fig:003 width=70%}

Проверить веб-приложение можно, введя его полный URL и не вводя порт, попробовала просканировать так (рис. [-@fig:004]).

![Запуск DVWA](image/004.png){#fig:004 width=70%}

Затем попробовала просканировать введя алрес хоста и адрес порта, результаты незначительно отличаются (рис. [-@fig:005]).

![Запуск DVWA](image/005.png){#fig:005 width=70%}


# Выводы

Научилась тестировать приложения с помощью сканера nikto

# Список литературы{.unnumbered}

::: {#refs}
:::
