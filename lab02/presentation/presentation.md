---
## Front matter
lang: ru-RU
title: Лаборатрная рабта №2
subtitle: Операционные системы
author:
  - Спиридонова Алина
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 17 февраля 2023

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
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Спиридонова Алина Артёмовна
  * студентка группы НБИбд-03-22
  * Российский университет дружбы народов


:::
::::::::::::::



## Объект и предмет исследования

- Презентация как текст
- Программное обеспечение для создания презентаций
- Входные и выходные форматы презентаций

## Цели и задачи

- Изучить идеологию и применение средств контроля версий.
- Освоить умения по работе с git.

## Материалы и методы

- Процессор `pandoc` для входного формата Markdown
- Результирующие форматы
	- `pdf`
	- `html`
- Автоматизация процесса создания: `Makefile`

# Создание презентации

## Процессор `pandoc`

- Pandoc: преобразователь текстовых файлов
- Сайт: <https://pandoc.org/>
- Репозиторий: <https://github.com/jgm/pandoc>

## Формат `pdf`

- Использование LaTeX
- Пакет для презентации: [beamer](https://ctan.org/pkg/beamer)
- Тема оформления: `metropolis`

## Код для формата `pdf`

```yaml
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
```

## Формат `html`

- Используется фреймворк [reveal.js](https://revealjs.com/)
- Используется [тема](https://revealjs.com/themes/) `beige`

## Код для формата `html`

- Тема задаётся в файле `Makefile`

```make
REVEALJS_THEME = beige 
```
# Результаты

## Получающиеся форматы

- Полученный `pdf`-файл можно демонстрировать в любой программе просмотра `pdf`
- Полученный `html`-файл содержит в себе все ресурсы: изображения, css, скрипты
.

## Содержание исследования

1. Зададим имя и email владельца репозитория:
![рисунок 1](image/nameemail.png){#fig:002 width=90%}

##
2. Настроим utf-8 в выводе сообщений git:
![рисунок 2](image/quotepath.png){#fig:003 width=90%}

##
3. Зададим имя начальной ветки (будем называть её master):
![рисунок 3](image/master.png){#fig:004 width=90%}

##
4. Параметр autocrlf:
![рисунок 4](image/input.png){#fig:005 width=90%}

##
5. Параметр safecrlf:
![рисунок 5](image/warn.png){#fig:006 width=90%}

##
6. Создадим ключи ssh по алгоритму rsa с ключём размером 4096 бит:
![рисунок 6](image/keygen4096.png){#fig:007 width=90%}
по алгоритму ed25519:
![рисунок 7](image/keygened.png){#fig:008 width=90%}

##
7. Генерируем ключ gpg
![рисунок 8](image/gpggenerate.png){#fig:009 width=90%}

##
8. Выводим список ключей и копируем отпечаток приватного ключа:
![рисунок 9](image/gpglong.png){#fig:010 width=90%}

##
9. Cкопируйте ваш сгенерированный PGP ключ в буфер обмена:
![рисунок 10](image/export.png){#fig:011 width=90%}

##
10. Используя введёный email, укажите Git применять его при подписи коммитов:
![рисунок 11](image/gitconfig.png){#fig:012 width=90%}

##
11. Авторизация github.
![рисунок 12](image/ghauth.png){#fig:013 width=90%}

##
12. Создаём репозиторий
![рисунок 13](image/mkdir.png){#fig:014 width=90%}

##
13. Настраиеваем каталог курса и отправляем файлы на сервер.
![рисунок 14](image/gitclone.png){#fig:015 width=90%}
![рисунок 15](image/gitcommit.png){#fig:016 width=90%}

## Результаты

- Настроили GitHub 
- Создали ключи

## Итоговый слайд

- В ходе выполнения лабораторной работы, я изучила идеологию и применение средств контроля версий и освоила умения работать с git.

