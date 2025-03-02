---
## Front matter
title: "Отчёт по 1-ому этапу индивидуального проекта"
subtitle: "Основы информационной безопасности"
author: "Бережной Иван Александрович"

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
lotTittle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Попрактиковать навыки установки дистрибутивов Linux на виртуальную машину.

# Задание

Установить Kali Linux на виртуальную машину VirtualBox.

# Выполнение лабораторной работы

Откроем VirtualBox, создадим в нём виртуальную машину и настроем её. Настройки выберем следующие: RAM - 4gb, CPU - 4 cores, ROM - 45gb (рис. [-@fig:001]).

![Создание ВМ](image/1.png){#fig:001 width=70%}

Запускаем машину, нас встречает установщик ОС (рис. [-@fig:002]). Языком системы выберем русский (рис. [-@fig:003]), но клавиатуру поставим английскую (рис. [-@fig:004]).

![Начало установки](image/2.png){#fig:002 width=70%}

![Язык системы](image/3.png){#fig:003 width=70%}

![Клавиатура](image/4.png){#fig:004 width=70%}

В качестве имени компьютера введём логин для входа учётной записи в компьютерных классах РУДН (рис. [-@fig:005]). Также впишем имя домена, согласно шаблону : <username>.localdomain (рис. [-@fig:006]).

![Имя пк](image/5.png){#fig:005 width=70%}

![Имя домена](image/6.png){#fig:006 width=70%}

Создадим пользователя и учётную запись. Для начала впишем некий никнейм (рис. [-@fig:007]), после - имя пользователя (рис. [-@fig:008]) и пароль для него (рис. [-@fig:009]).

![Реальное имя пользователя](image/7.png){#fig:007 width=70%}

![Имя пользователя](image/8.png){#fig:008 width=70%}

![Пароль](image/9.png){#fig:009 width=70%}

Выберем нужный часовой пояс (рис. [-@fig:010]). 

![Часовой пояс](image/10.png){#fig:010 width=70%}

Настроим диски. В следующем окне выберем "Авто" (рис. [-@fig:011]). Раздел сделаем общим (рис. [-@fig:012]) и подтверждаем (рис. [-@fig:013]).

![Разметка дисков 1](image/11.png){#fig:011 width=70%}

![Разметка дисков 2](image/12.png){#fig:012 width=70%}

![Разметка дисков 3](image/13.png){#fig:013 width=70%}

Выберем дополнительное ПО. Я оставлю по умолчанию (рис. [-@fig:014]). 

![Дополнительное ПО](image/14.png){#fig:014 width=70%}

Установим системный загрузчик GRUB (рис. [-@fig:015] и [-@fig:016]).  

![GRUB 1](image/15.png){#fig:015 width=70%}

![GRUB 2](image/16.png){#fig:016 width=70%}

После завершения установки убедимся, что оптический привод виртуалной машины стал пуст. После этого перезагрузим ОС (рис. [-@fig:017]). 

![Конец установки](image/17.png){#fig:017 width=70%}

Мы внутри Kali (рис. [-@fig:018]).

![Первый вход в систему](image/18.png){#fig:018 width=70%}

# Выводы

В ходе выполнения этапа проекта мы потренировались устанавливать ОС на виртуальную машину.
