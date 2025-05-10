---
## Front matter
title: "Отчет по внешнему курсу"
subtitle: "2. Безопасность в сети"
author: "Дагделен Зейнап Реджеповна"

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

Изучить основы кибербезопасности и пройти внешний курс.

# Выполнение заданий внешнего курса

## Протокол прикладного уровня
**Комментарий:** HTTPS — это протокол прикладного уровня, обеспечивающий безопасную передачу данных (рис. [-@fig:001]).  

![Задание](image/1.1.png){#fig:001 width=70%}

##  Уровень работы протокола TCP
**Комментарий:** TCP работает на транспортном уровне модели OSI (рис. [-@fig:002]).  

![Задание](image/1.2.png){#fig:002 width=70%}

##  Корректные адреса IPv4
**Комментарий:** Примеры корректных IPv4-адресов: `90.11.90.22` и `25.198.0.15`(рис. [-@fig:003]).  

![Задание](image/1.3.png){#fig:003 width=70%}

##  Функция DNS сервера
**Комментарий:** DNS сервер сопоставляет доменные имена с IP-адресами(рис. [-@fig:004]). 
 
![Задание](image/1.4.png){#fig:004 width=70%}  

## Последовательность протоколов в TCP/IP
**Комментарий:** Правильный порядок: прикладной → транспортный → сетевой → канальный (рис. [-@fig:005]). 
 
![Задание](image/1.5.png){#fig:005 width=70%}  

## Протокол HTTP
**Комментарий:** HTTP передает данные между клиентом и сервером в открытом виде (рис. [-@fig:006]).  

![Задание](image/1.6.png){#fig:006 width=70%}  

##  Состав протокола HTTPS

**Комментарий:** HTTPS включает фазы рукопожатия и передачи данных с шифрованием (рис. [-@fig:007]). 
 
![Задание](image/1.7.png){#fig:007 width=70%}  

## Определение версии TLS

**Комментарий:** Версия TLS согласуется между клиентом и сервером в процессе "переговоров"(рис. [-@fig:008]). 
 
![Задание](image/1.8.png){#fig:008 width=70%}  


##  Фаза "рукопожатия" в TLS
**Комментарий:** В этой фазе не происходит шифрование данных, только согласование параметров (рис. [-@fig:009]).  

![Задание](image/1.9.png){#fig:009 width=70%}  

## Данные для аутентификации
**Комментарий:** Для аутентификации могут использоваться идентификатор пользователя и пароль (рис. [-@fig:010]). 
 
![Задание](image/1.10.png){#fig:010 width=70%}  

##  Использование куки
**Комментарий:** Куки не предназначены для улучшения надежности соединения (рис. [-@fig:011]).  

![Задание](image/1.11.png){#fig:011 width=70%}  

##  Генерация куки
**Комментарий:** Куки создаются сервером и отправляются клиенту(рис. [-@fig:012]).  

![Задание](image/1.12.png){#fig:012 width=70%}  

## Хранение сессионных куки
**Комментарий:** Сессионные куки хранятся в браузере только во время использования сайта (рис. [-@fig:013]).  

![Задание](image/1.13.png){#fig:013 width=70%}  

##  Промежуточные узлы в TOR
**Комментарий:** В сети TOR используется 3 промежуточных узла(рис. [-@fig:014]).  

![Задание](image/1.14.png){#fig:014 width=70%}  

##  Узлы в луковой сети TOR
**Комментарий:** Ключевые узлы: охранный, промежуточный и выходной (рис. [-@fig:015]).  

![Задание](image/1.15.png){#fig:015 width=70%}  

##  Генерация ключа в TOR
**Комментарий:** Отправитель создает общий ключ с охранным, промежуточным и выходным узлами (рис. [-@fig:016]).  

![Задание](image/1.16.png){#fig:016 width=70%}  

## Использование браузера TOR получателем
**Комментарий:** Получателю не требуется использовать TOR для получения пакетов (рис. [-@fig:017]).  

![Задание](image/1.17.png){#fig:017 width=70%}  

## Определение Wi-Fi
**Комментарий:** Wi-Fi — это технология беспроводной сети по стандарту IEEE 802.11. (рис. [-@fig:018]) 

![1.18](image/1.18.png){#fig:018 width=70%}  

## Уровень работы протокола Wi-Fi
**Комментарий:** Wi-Fi работает на канальном уровне модели OSI (рис. [-@fig:019]).  

![Задание](image/1.19.png){#fig:019 width=70%} 

## Небезопасный метод шифрования Wi-Fi
**Комментарий:** WEP устарел и считается небезопасным (рис. [-@fig:020]).  

![Задание](image/1.20.png){#fig:020 width=70%}  

## Передача данных между хостом и роутером
**Комментарий:** Данные между хостом и роутером передаются в зашифрованном виде после аутентификации устройств (рис. [-@fig:021]). 
 
![Задание](image/1.21.png){#fig:021 width=70%}  

## Метод аутентификации в домашней сети
**Комментарий:** В домашних сетях обычно используется WPA2 Personal для аутентификации устройств (рис. [-@fig:022]).
  
![Задание](image/1.22.png){#fig:022 width=70%}  

# Выводы

Я прошла 1 часть курса

