---
## Front matter
lang: ru-RU
title: Лабораторная работа № 4
subtitle: Основы информационной безопасности
author:
  - Зинченко А.Р
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 05 апреля 2025

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
---

# Информация

## Докладчик

  * Зинченко Анастасия Романовна
  * НБИбд-02-23
  * Российский университет дружбы народов

---
## Front matter
title: "Отчёт по лабораторной работе №4"
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

Целью данной работы является получение практических навыков работы в консоли с  расширенными атрибутами файлов

# Выполнение лабораторной работы

От имени пользователя guest определим расширенные атрибуты файла /home/guest/dir1/file1 командой
*lsattr /home/guest/dir1/file1* 

Установим командой *chmod 600 file1* на файл file1 права, разрешающие чтение и запись для владельца файла 

Попробуем установить на файл /home/guest/dir1/file1 расширенный атрибут *a* от имени пользователя guest: *chattr +a /home/guest/dir1/file1*. В ответ мы получили отказ на выполнение операции 

Попробуем установить расширенный атрибут a на файл /home/guest/dir1/file1 от имени суперпользователя: *chattr +a /home/guest/dir1/file1* 

От пользователя guest проверим правильность установления атрибута: *lsattr /home/guest/dir1/file1* 

Выполним дозапись в файл file1 слова «test» командой *echo "test" >> dir1/file1*. И после этого выполним чтение файла file1 командой *cat dir1/file1* 

Попробуем удалить файл file1, а затем переименовать его. Обе операции не доступны 

Далее попробуем с помощью команды *chmod 000 file1* установить на файл file1 права, например, запрещающие чтение и запись для владельца файла. Этого нам тоже сделать не удалось 

Далее снимем расширенный атрибут *a* с файла /home/guest/dirl/file1 от имени суперпользователя командой *chattr -a /home/guest/dir1/file1*. И повторим операции, которые нам ранее не удавалось выполнить 

Далее повторим наши действия по шагам, заменив атрибут «a» атрибутом «i»

# Выводы

В результате выполнения работы мы повысили свои навыки использования интерфейса командой строки (CLI), познакомились на примерах с тем, как используются основные и расширенные атрибуты при разграничении доступа. Имели возможность связать теорию дискреционного разделения доступа (дискреционная политика безопасности) с её реализацией на практике в ОС Linux. Опробовали действие на практике расширенных атрибутов «а» и «i»

# Список литературы

1. Лаборатораня работа №4 [Электронный ресурс] URL: https://esystem.rudn.ru/pluginfile.php/2580982/mod_resource/content/3/004-lab_discret_extattr.pdf
