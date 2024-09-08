---
## Front matter
title: "Отчет по этапу индивидуального проекта №1"
subtitle: "Операционные системы"
author: "hanjiangtao"

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

Научиться размещать сайт на Github pages. Выполнить первый этап реализации индивидуального проекта.

# Задание

1. Установить необходимое ПО
2. Скачать шаблон темы сайта
3. Разместить его на хостинге Git
4. Установить параметр для URLs сайта
5. Разместить заготовку сайта на Github pages.

# Выполнение этапа индивидуального проекта

## Установка необходимого ПО

Скачиваю последнюю версию исполняемого файла hugo для своей операционной системы (рис. @fig:001).

![Выбор версии ПО](image/1.png){#fig:001 width=70%}

Распаковываю архив с исполняемым файлом (рис. @fig:002).

![Распаковка архива](image/2.png){#fig:002 width=70%}

Создаю в домашнем каталоге пустую папку bin с помощью утилиты mkdir, переношу в эту папку исполняемый файл hugo (рис. @fig:003).

![Перемещение файла](image/3.png){#fig:003 width=70%}

## Скачивание шаблона темы сайта

Открываю репозиторий с шаблоном темы сайта (рис. @fig:004).

![Репозиторий с шаблоном темы сайта](image/4.png){#fig:004 width=70%}

Создаю свой репозиторий blog на основе репозитория с шаблоном темы сайта (рис. @fig:005).

![Создание репозитория](image/5.png){#fig:005 width=70%}

Клонирую созданный репозиторий к себе в локальный репозиторий (рис. @fig:006).

![Клонирование репозитория](image/7.png){#fig:006 width=70%}

## Размещение его на хостинге Git

Запускаю исполняемый файл (рис. @fig:007).

![Запуск исполняемого файла](image/10.png){#fig:007 width=70%}

Удаляю папку public которая сейчас нам не понадобится, тем более мы создадим свою (рис. @fig:008).

![Удаление каталога](image/9.png){#fig:008 width=70%}

Снова запускаю исполняемый файл с командой server (рис. @fig:009).

![Запуск исполняемого файла](image/11.png){#fig:009 width=70%}

Получилась страничка сайта на локальном сервере (рис. @fig:010).

![Сайт на локальном сервере](image/12.png){#fig:010 width=70%}

## Установка параметр для URLs сайта

Теперь создаю новый пустой репозиторий чье имя будет адресом сайта (рис. @fig:011).

![Создание репозитория](image/13.png){#fig:011 width=70%}

Клонирую созданный репозиторий, чтобы создать локальный репозиторий у себя на компьютере (рис. @fig:012).

![Клонирование репозитория](image/15.png){#fig:012 width=70%}

Создаю главную ветку с именем main (рис. @fig:013).

![Создание главное ветки](image/16.png){#fig:013 width=70%}

Создаю пустой файл README.md и отправляю изменения на глобальный репозиторий, чтобы его активировать (рис. @fig:014).

![Создание файла](image/17.png){#fig:014 width=70%}

Перед тем как подключать созданный пустой репозиторйи к каталогу public из репозитория blog, нужно отключить в файле gitignore public, чтобы каталоги с таким названием не игнорировались (рис. @fig:015).

![Редактирование файла](image/19.png){#fig:015 width=70%}

Подключаю репозиторий к каталогу public (рис. @fig:016).

![Подключаение репозитория к каталогу](image/20.png){#fig:016 width=70%}

Снова выполняю команду исполняемого файла, чтобы заполнить создавшийся каталог public (рис. @fig:017).

![Название рисунка](image/21.png){#fig:017 width=70%}

## Размещение заготовку сайта на Github pages.

Проверяю есть ли подключение между public и репозиторием evdvorkina.github.io, после чего отправляю изменения на глобальный репозиторий (рис. @fig:018).

![Отправка изменений на глобальный репозиторий](image/22.png){#fig:018 width=70%}

# Выводы

Я научилась размещать сайт на Github pages и, следовательно, выполнила первый этап реализации индивидуального проекта.

