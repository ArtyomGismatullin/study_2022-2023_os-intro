---
## Front matter
title: "Отчёт по второму этапу индивидуального проекта"
subtitle: "дисциплина: Операционные системы"
author: "Гисматуллин Артём Вадимович НПИбд-01-22"

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
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Добавить к сайту данные о себе.

# Задание

1. Разместить фотографию владельца сайта.
2. Разместить краткое описание владельца сайта.
3. Добавить информацию об интересах.
4. Добавить информацию об образовании.
5. Сделать пост по прошедшей неделе.
6. Добавить пост на тему: "Управление версиями.Git."

# Выполнение индивидуального проекта

Для начала добавим нашу фотографию. Для этого мы должны проделать данный путь: "work", "blog", "content", "authors", "admin". (рис. [-@fig:001]).

![Добавление фотографии](image/01.png){ #fig:001 width=100% }

В этом же каталоге ("admin") открываем файл "_index.md". В него мы внесём наше имя, фамилию. Также добавим биографию, интересы, образование и др. (рис. [-@fig:002]).

![Добавление информации о себе](image/02.png){ #fig:002 width=100% }

Следующим шагом будет создание двух постов. Открываем терминал из каталога "blog" и вводим команду: hugo new --kind post post/(название поста) (рис. [-@fig:003]).

![Создание двух постов](image/03.png){ #fig:003 width=100% }

После этого в каталоге "post" появляются наши новые подкаталоги "Git" и "Моя-1-неделя". Именно внутри этих подкаталогов мы будем добавлять информацию для постов (рис. [-@fig:004]).

![Новые подкаталоги для постов](image/04.png){ #fig:004 width=100% }

Внесём информацию для нашего поста "Управление версиями.Git." (рис. [-@fig:005]).

![Информация для поста](image/05.png){ #fig:005 width=100% }

Чтобы вся наша информация выгрузилась на сайт, откроем в каталоге "blog" терминал и запустим команду hugo (рис. [-@fig:006]).

![Запуск команды hugo](image/06.png){ #fig:006 width=100% }

Как только команда hugo выполнилась перейдём первым этапом в подкаталог "public" и проделаем указанные на скриншоте действия. Вторым этапом проделаем все те же самые действия, но уже в каталоге "blog" (рис. [-@fig:007]).

![Выгрузка из подкаталога "public"](image/07.png){ #fig:008 width=100% }

Последним шагом перейдём на наш сайт и посмотрим итог работы (рис. [-@fig:008]) и (рис. [-@fig:009]). 

![Информация о себе на сайте](image/08.png){ #fig:008 width=100% }

![Новые посты на сайте](image/09.png){ #fig:009 width=100% }

# Выводы

В ходе выполнения второго этапа индивидуального проекта мы научились добавлять к сайту информацию о себе, а также создавать новые посты.

