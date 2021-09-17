---
# Front matter
title: "Отчёт по лабораторной работе №1"
subtitle: "Установка и конфигурация операционной системы на виртуальную машину"
author: "Захарова Софья Михайловна"

# Generic otions
lang: ru-RU

# Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

# Pdf output format
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
### Fonts
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
## Misc options
indent: true
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.


# Задание

Лабораторная работа подразумевает установку на виртуальную машину VirtualBox операционной системы
Linux, дистрибутив Centos.


# Выполнение лабораторной работы

Заходим в терминал, в каталог /var/tmp, создаем каталог smzakharova1 для дальнейшей работы, перейти в общий каталог, где размещён образ виртуальной машины.

![Рис.1. Создание каталога для работы.](images/1.jpg){ #fig:001 width=70% }

Копируем образ в каталог, созданный на предыдущем шаге.

![Рис.2. Копирования образа ВМ в smzakharova1.](images/2.jpg){ #fig:001 width=70% }

Заходим в VB Менеджер и создаем виртуальную машину Base с типом Linux версией Red Hat(64-bit)

![Рис.3. Создание виртуальной машины.](images/3.jpg){ #fig:001 width=70% }

Указываем объем памяти - 1024 МБ.

![Рис.4. Установка объема памяти.](images/4.jpg){ #fig:001 width=70% }

Выбираем новый виртуальный жесткий диск.

![Рис.5. Создание нового жесткого диска.](images/5.jpg){ #fig:001 width=70% }

Указываем тип: VDI.

![Рис.6. Тип VDI.](images/6.jpg){ #fig:001 width=70% }

Указываем формат хранения.

![Рис.7. Динамический виртуальный жесткий диск.](images/7.jpg){ #fig:001 width=70% }

Указываем имя и размер файла.

![Рис.8. Размер - 40 ГБ.](images/8.jpg){ #fig:001 width=70% }

Устанавливаем папку для снимков.

![Рис.9. Папка для снимков.](images/9.jpg){ #fig:001 width=70% }

Устанавливаем носитель.

![Рис.10. Носитель.](images/10.jpg){ #fig:001 width=70% }

Запускаем виртуальную машину Base и устанавливаем язык.

![Рис.11. Установка языка.](images/11.jpg){ #fig:001 width=70% }

Устанавливаем дату и время.

![Рис.12. Дата и время.](images/12.jpg){ #fig:001 width=70% }

Раскладку клавиатуры меняем на русскую.

![Рис.13. Меняем клавиатуру.](images/13.jpg){ #fig:001 width=70% }

Устанавливаем сервер с GUI и дополнения "средства разработки".

![Рис.14. Изменения сервера и дополнений.](images/14.jpg){ #fig:001 width=70% }

Выбираем нужное устройство.

![Рис.15. Выбор устройства.](images/15.jpg){ #fig:001 width=70% }

Меняем сеть и имя узла.

![Рис.16. Сеть и имя узла.](images/16.jpg){ #fig:001 width=70% }

Задаем пароль.

![Рис.17. Пароль.](images/17.jpg){ #fig:001 width=70% }

Вводим имя пользователя для дальнейшей работы и вводим пароль.

![Рис.18. Имя пользователя.](images/18.jpg){ #fig:001 width=70% }

Принимаем лицензионное соглашение.

![Рис.19. Лицензионное соглашение.](images/19.jpg){ #fig:001 width=70% }

Сеть и имя узла установлены на предыдущих шагах, оставляем неизменными.

![Рис.20. Сеть и имя узла.](images/20.jpg){ #fig:001 width=70% }

Заходим под своим профилем, вводим пароль от учетной записи.

![Рис.21. Вход в учетную запись.](images/21.jpg){ #fig:001 width=70% }

Переходим под учетную запись root в терминале с помощью команды su, Обновляем системные файлы и устанавливаем необходимые программы.

![Рис.22. Работа в терминале виртуальной машины.](images/22.jpg){ #fig:001 width=70% }

Заходим в менеджер виртуальных носителей и освобождаем жесткий диск, изменяем атрибуты носителя на множественное подключение.

![Рис.23. Создание виртуальной машины.](images/23.jpg){ #fig:001 width=70% }

# Выводы

В ходе работы мы установили операционную систему на виртуальную машину, настроили минимально необходимые для дальнейшей работы сервисы.
