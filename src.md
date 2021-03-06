# Новый ительменский алфавит
## Новый ительменский кириллический алфавит
Этот проект вводит новый кириллический алфавит для ительменского языка, на основе русского алфавита и строго БЕЗ дополнительных символов, кроме символов русского алфавита. Делается это из следующих соображений:

1. Ительменский алфавит был создан без учёта компьютеризации в 1988 году.
2. Все "тяжелые для написания" (требующие особой раскладки) буквы ительменского алфавита обозначают звуки собственно ительменского языка.
3. В то же время все буквы русского алфавита также включены в ительменский алфавит, хотя некоторые из них используются только в заимствованиях из русского.
4. Очень глупо при разработке отдельной ительменской раскладки было бы менять положение русских букв.
5. В то же самое время получается, что все дополнительные "тяжелые" буквы, которые часто встречаются именно в ительменских словах, написать будет весьма непросто. Например, придется "писать" их, кликая по таблице символов юникода, или же через эскейп-последовательности на клавиатуре. Долго, муторно, неочевидно, сложно - а значит плохо
6. Язык умирает, усложнять его таким алфавитом недопустимо.

Без предисловий, эта ситуация исправляется переводом алфавита ительменского языка 1988 года на чисто русский алфавит, а именно следующими заменами (**шаг 1**):

- Ӄ --> Къ
- Ӽ --> Хъ
- Ӈ --> Нъ
- Њ --> Нь
- Љ --> Ль

таким образом удаляются буквы с "хвостами" снизу. Далее черёд удалить букву Э ительменское (**шаг 2**):

- Ә --> Э'

далее черёд удалить все "лежачие полумесяцы" (*"краткие"*) над Ӑ, О̆, Ў, заменив полумесяц на апостроф и сделав замены (**шаг 3**):

- Ӑ --> А' 
- О̆ --> O' 
- Ў --> У'

И в конце концов требуется избавиться от апострофа. Написать апостроф несложно, однако в стандартной русской раскладке на ПК он отсутствует, и поэтому это плохо. Переключаться для набора апострофа на другую раскладку - никуда не годится. Потому что в пределах одного слова придется перепрыгивать несколько раз с русской раскладки на раскладку с апострофом. Добавить в русскую раскладку хотя бы один символ также идёт вразрез с нашими целями.

Поэтому, замены такие (**шаг 4**):

- A' --> Aь
- О' --> Оь
- У' --> Уь
- Э' --> Эь
- К' --> Кь
- Къ' --> Къь
- П' --> Пь
- Т' --> Ть
- Ч' --> Чь

Если же апостроф обозначал гортанную смычку, то ныне его обозначать так (**шаг 5**): 

- ' (*гортанная смычка*) --> Ьь ьь.

И, наконец, осталось разобраться со значком огубления перед словом. Никуда он не годится, и поэтому заменяем его на последовательность "ъ-" перед словом (**шаг 6**):

- ˚ --> ъ-

Новый ительменский кириллический алфавит готов после шага 6, путём проведения замен **шаг 1** - **шаг 6** над ительменским алфавитом 1988 года.

### Примеры
Рассмотрим примеры написания до и после:

- кзуњӆӄукнин - кзуньлъкъукнин
- вэтаткиԓӽ - вэтаткилъхъ
- тӽӑлтӽӑл - тхъаьлтхъаьл
- ч'эном - чьэном
- ӄ'ыӄ' - къьыкъь
- йуӈйучҳ - йунъйучхъ

и так далее.

## Новый ительменский латинский алфавит
Напоследок, несколько замечаний относительно латинского алфавита и взаимоперевода ительменского языка с латинского алфавита на кириллический. Старый латинский ительменский алфавит имеет радикально меньше букв, чем кириллический алфавит 1988 года. Имея всего три дополнительные буквы, он весьма пригляден для практического использования, в отличие от ительменского алфавита 1988 года. Однако:

1. Большинство учебников по ительменскому написаны на алфавите 1988 года. 
   *Примечание*: Самое смешное, что существует разнобой в напечатании "строго ительменских букв" - то бишь с хвостиками и так далее - издательства понятия не имеют, как печатать ительменский и используют "похожие" буквы.

2. Затруднительно найти даже таблицу перевода с латиницы ительменской на кириллицу. Это недопустимо для умирающего языка.

Вынесем новоительменский кириллический алфавит в таблицу:

Было:

|     |   |     |   |     |   |   |   |   |   |   |     |
|-----|---|-----|---|-----|---|---|---|---|---|---|-----|
|А а  |Б б|В в  |Г г|Д д  |Е е|Ё ё|Ж ж|З з|И и|Й й|К к  |
|К’ к’|Ӄ ӄ|Ӄ’ ӄ’|Л л|Љ љ  |Ԓ ԓ|М м|Н н|Њ њ|Ӈ ӈ|О о|П п  |
|П’ п’|Р р|С с	|Т т|Т’ т’|У у|Ф ф|Х х|Ӽ ӽ|Ц ц|Ч ч|Ч’ ч’|
|Ш ш  |Щ щ|Ъ ъ  |Ы ы|Ь ь  |Ә ә|Э э|Ю ю|Я я|’  |   |     |

Стало:

|     |     |       |   |     |     |   |   |     |     |   |     |
|-----|-----|-------|---|-----|-----|---|---|-----|-----|---|-----|
|А а	|Б б  |В в    |Г г|Д д  |Е е  |Ё ё|Ж ж|З з  |И и  |Й й|К к  |
|Кь кь|Къ къ|Къь къь|Л л|Ль ль|Лъ лъ|М м|Н н|Нь нь|Нъ нъ|О о|П п  |
|Пь Пь|Р р  |С с	  |Т т|Ть ть|У у  |Ф ф|Х х|Хъ хъ|Ц ц  |Ч ч|Чь чь|
|Ш ш  |Щ щ  |Ъ ъ    |Ы ы|Ь ь  |Эь эь|Э э|Ю ю|Я я  |Ьь ьь|   |     |

После перевода на новоительменский алфавит нет трудностей в переводе ительменского на латиницу взаимнооднозначным способом:

|     |       |       |   |     |     |     |     |     |     |     |       |
|-----|-------|-------|---|-----|-----|-----|-----|-----|-----|-----|-------|
|A a	|B b	  |V v	  |G g|D d	|Ye ye|Yo yo|Zh zh|Z z	|I i	|Y y	|K k    |
|Kx kx|Kq kq  |Kqx kqx|L l|Lx lx|Lq lq|M m  |N n  |Nx nx|Nq nq|O o  |P p    |
|Px px|R r    |S s    |T t|Tx tx|U u  |F f  |J j  |Jq jq|C c  |Ch ch|Chx chx|
|Sh sh|Sch sch|Q q    |W w|X x  |Ex ex|E e  |Yu yu|Ya ya|Xx xx|

где из кириллических йотовых буквы вынесен йот Y, и некоторые буквы используются строго для модификации значения предыдущей буквы и нигде более: Q = Ъ, X = Ь, а H лишь помогает в передаче букв Ж Ш Щ Ч и нигде кроме этого не используется.

### Примеры
Рассмотрим примеры написания до и после (с латиницей):

- кзуњӆӄукнин - kzunxlqkquknin
- вэтаткиԓӽ - vetatkilqjq
- тӽӑлтӽӑл - tjaxltjaxl
- ч'эном - chxenom
- ӄ'ыӄ' - kqxwkqx
- йуӈйучҳ - yunqyuchxjq
