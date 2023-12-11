---
## Front matter
title: "Шаблон отчёта по лабораторной работе"
subtitle: "Простейший вариант"
author: "Абдул Васе Фейсал Ахмад"

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

Целью работы является освоение процедуры оформления отчетов с помощью легковесного
языка разметки Markdown.

# Задание

1.) Откройте терминал

2.) Перейдите в каталог курса сформированный при выполнении лабораторной работы №2:
  
  cd ~/work/study/2023-2024/"Архитектура компьютера"/arch-pc/

Обновите локальный репозиторий, скачав изменения из удаленного репозитория с помо-
щью команды
  
  git pull
  
![git pull](/home/Ahmad/work/study/2023-2024/computer_architecture/study_2023-2024_arch-pc/labs/lab03/report/image/msg1755786255-4755.jpg)

  __комментарий:__ Я обновил свое рабочее пространство с помощью команды git pull.
   
3.) Перейдите в каталог с шаблоном отчета по лабораторной работе № 3

  cd ~/work/study/2023-2024/"Архитектура компьютера"/arch-pc/labs/lab03/report

![лабораторной работе № 3](/home/Ahmad/work/study/2023-2024/computer_architecture/study_2023-2024_arch-pc/labs/lab03/report/image/msg1755786255-4754.jpg)

  __комментарий:__ Я сменил каталог на каталог с шаблоном отчета для лаб 3
  
4.) Проведите компиляцию шаблона с использованием Makefile. Для этого введите ко-
манду
   
   make
   
При успешной компиляции должны сгенерироваться файлы report.pdf и report.docx.
Откройте и проверьте корректность полученных файлов.
 
   
![make](/home/Ahmad/work/study/2023-2024/computer_architecture/study_2023-2024_arch-pc/labs/lab03/report/image/msg1755786255-4757.jpg)
  
  __комментарий:__Скомпилировал шаблон с помощью make-файла и убедился, что необходимые файлы созданы с помощью команды ls
   
5.) Удалите полученный файлы с использованием Makefile. Для этого введите команду

  make clean

Проверьте, что после этой команды файлы report.pdf и report.docx были удалены.

![make clean](/home/Ahmad/work/study/2023-2024/computer_architecture/study_2023-2024_arch-pc/labs/lab03/report/image/msg1755786255-4758.jpg)

  __комментарий:__ Я удалил файлы, созданные после команды make. Я сделал это с помощью команды make clean.Я убедился, что файлы были удалены с помощью команды ls

6.) Откройте файл report.md c помощью любого текстового редактора, например gedit

  gedit report.md

![gedit report.md](/home/Ahmad/work/study/2023-2024/computer_architecture/study_2023-2024_arch-pc/labs/lab03/report/image/Screenshot from 2023-12-11 12-33-29.png)

__комментарий:__ Я открыл файл report.md с помощью текстового редактора gedit.


7.) Заполните отчет и скомпилируйте отчет с использованием Makefile. Проверьте кор-
ректность полученных файлов. (Обратите внимание, для корректного отображения
скриншотов они должны быть размещены в каталоге image)








# Выводы

Здесь кратко описываются итоги проделанной работы.

# Список литературы{.unnumbered}

::: {#refs}
:::
