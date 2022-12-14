## Начало работы с GIT 

*в начале работы не обходимо нициализировать рабочий файл* 

**git init**

*после инециализации файла необходимо его запутить в работу*

**git add название файла** 

*после запуска в работу необходимо создать коммид* 

**git commit -m**

**git commit -a**

**git commit -am** 

*для просмотра статуса рабочего файла*

**git status**

## работа с версиями 

*для просмортра версий*

**git log** 
*команда для просмотра актуальных версий* 

**git log --all** 
*команда для просмотра всех существующих версий* 

**git log --oneline** 
*для просмотра крадкого содержания* 

**так же --all --oneline можно приенять в одной команде** 

*что бы сравнить версии между собой*

**git diff 1111 2222** 

*что бы переместиться между версиями* 

**git checkout 11111**


## ветвление  

       Ветвление в git нужно для разделения файла на части для того что бы могли работать несколько человек или разделить на разные задачи.

*для просмотра ветви в которой я работаю* 

**git branch** 

*для создание новой ветви* 

**git branch название ветви** 

*для пермещение по ветвям* 

**git checkout название ветви** 

        для слияния ветвей в первую очередь необходимо перейти в основную ветвь master 

    
*слияние ветвей* 

**git merge название ветви** 

*для просмотра версий и их ветвление* 

**git log --all --oneline --graph** 

*для удвление ветви* 

**git branch -d назване ветви**

## работа с текстом в Markdown 


*ЗАГОЛОВКИ*

        #H1
        ##H2 
        ###H3
        ####H4
        #####H5
        ######H6 

**Кроме того, H1 и H2 можно обозначить подчеркиванием:**

Alt-H1
======

Alt-H2
------


**Курсив** обозначается *звездочками* или _подчеркиванием_.

Полужирный шрифт - двойными **звездочками** или __подчеркиванием__.

Комбинированное выделение **звездочками и _подчеркиванием_**.

Для зачеркнутого текста используются две тильды (~~).     ~~Уберите это.~~


**Списки** 
       
        В данном примере предшествующие и завершающие пробелы обозначены точками: ⋅


1. Первый пункт нумерованного списка
1. Второй пункт
⋅⋅*Ненумерованный вложенный список.
1. Сами числа не имеют значения, лишь бы это были цифры
 ⋅⋅1. Нумерованный вложенный список
1. И еще один пункт.
  ⋅⋅⋅Внутри пунктов списка можно вставить абзацы с таким же отступом. Обратите внимание на пустую строку выше и на пробелы в начале (нужен по меньшей мере один, но здесь мы добавили три, чтобы также выровнять необработанный Markdown).

 

* Ненумерованный список можно размечать звездочками
- Или минусами
+ Или плюсами

**ссылки**

        Ссылки можно оформить разными способами.

[Обычная ссылка в строке](https://www.google.com)

[Обычная ссылка с title](https://www.google.com "Сайт Google")

[Ссылка со сноской][Произвольный регистронезависимый текст]

[Относительная ссылка на документ](../blob/master/LICENSE)

[Для ссылок со сноской можно использовать цифры][1]

Или можно просто вставить ссылку в квадратные скобки [текст ссылки]

Произвольный текст, после которого можно привести ссылки.

[произвольный регистронезависимый текст]: https://www.mozilla.org
[1]: http://slashdot.org
[текст ссылки]: http://www.reddit.com

1
2
3
4
5
6
7

**Таблицы**

    Таблицы не являются частью Markdown, но многие обработчики, например Markdown Here и Github, поддерживают их. Они позволяют легко добавить таблицы в электронное письмо -- в других случаях для этого нужно копировать их из другого приложения.

    Вертикальные линии обозначают столбцы.

| Таблицы       | Это                | Круто |
| ------------- |:------------------:| -----:|
| столбец 3     | выровнен вправо    | $1600 |
| столбец 2     | выровнен по центру |   $12 |
| зебра-строки  | прикольные         |    $1 |

    Внешние вертикальные линии (|) не обязательны, и они нужны только чтобы сам код Markdown выглядел красиво. Тот же код можно записать так:

 Markdown | не такой | красивый
--- | --- | ---
*Но выводится* | `так же` | **клево**
1 | 2 | 3

