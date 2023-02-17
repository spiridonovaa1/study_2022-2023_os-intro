---
## Front matter
title: "Лабораторная работа №2"
subtitle: "Операционные системы"
author: "Спиридонова Алина Артёмовна"

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

 Изучить идеологию и применение средств контроля версий.
 Освоить умения по работе с git.


# Задание

    Создать базовую конфигурацию для работы с git.
    Создать ключ SSH.
    Создать ключ PGP.
    Настроить подписи git.
    Зарегистрироваться на Github.
    Создать локальный каталог для выполнения заданий по предмету.


# Теоретическое введение



# Выполнение лабораторной работы

Описываются проведённые действия, в качестве иллюстрации даётся ссылка на иллюстрацию (рис. @fig:001).

![Название рисунка](image/placeimg_800_600_tech.jpg){#fig:001 width=70%}
1. Зададим имя и email владельца репозитория:
![рисунок 1](image/nameemail.png){#fig:002 width=90%}
2. Настроим utf-8 в выводе сообщений git:
![рисунок 2](image/quotepath.png){#fig:003 width=90%}
3. Зададим имя начальной ветки (будем называть её master):
![рисунок 3](image/master.png){#fig:004 width=90%}
4. Параметр autocrlf:
![рисунок 4](image/input.png){#fig:005 width=90%}
5. Параметр safecrlf:
![рисунок 5](image/warn.png){#fig:006 width=90%}
6. Создадим ключи ssh по алгоритму rsa с ключём размером 4096 бит:
![рисунок 6](image/keygen4096.png){#fig:007 width=90%}
по алгоритму ed25519:
![рисунок 7](image/keygened.png){#fig:008 width=90%}
7. Генерируем ключ gpg
![рисунок 8](image/gpggenerate.png){#fig:009 width=90%}
8. Выводим список ключей и копируем отпечаток приватного ключа:
![рисунок 9](image/gpglong.png){#fig:010 width=90%}
9. Cкопируйте ваш сгенерированный PGP ключ в буфер обмена:
![рисунок 10](image/export.png){#fig:011 width=90%}
10. Используя введёный email, укажите Git применять его при подписи коммитов:
![рисунок 11](image/gitconfig.png){#fig:012 width=90%}
11. Авторизация github.
![рисунок 12](image/ghauth.png){#fig:013 width=90%}
12. Создаём репозиторий
![рисунок 13](image/mkdir.png){#fig:014 width=90%}
13. Настраиеваем каталог курса и отправляем файлы на сервер.
![рисунок 14](image/gitclone.png){#fig:015 width=90%}
![рисунок 15](image/gitcommit.png){#fig:016 width=90%}

# Выводы
В ходе выполнения лабораторной работы мне удалось изучить идеологию и применение средств контроля версий,а также освоить умения по работе с git.


# Список литературы{.unnumbered}

::: {#refs}
:::
