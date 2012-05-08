FormalSemantics
===============

NLP SHAD 3rd task

В качестве предметной области выбрана геополитическая база.

Объекты - страны (COUNTRY), города (CITY), реки (RIVER), озера (LAKE), моря (SEA), океаны (OCEANS).

Отношения между объектами:

1. Общая граница стран: COUNTRY borders upon COUNTRY
2. Река протекает через страну: RIVER flows through COUNTRY
3. Река впадает в озеро: RIVER runs into LAKE
4. Страна находится в военном конфликте с другой страной: COUNTRY is at war with COUNTRY
5. Страна является союзником другой страны: COUNTRY is ally of COUNTRY
6. Город является столицей страны: CITY is a capital of COUNTRY
7. Город находится в стране: CITY is in COUNTRY
8. У страны есть выход к морю: COUNTRY has access to SEA
9. Озеро находится в стране: LAKE is in COUNTRY

Возможно некоторые объекты и отношения можно убрать, если они выяснится, что они избыточны.

Необходимо придумать и реализовать 12 типов синтаксически разных запросов. Предлагаемые для реалзации запросы:

1. Какие есть объекты?
What coutries are? - Какие есть страны?
What cities are? - Какие есть города?
What capitals are? - Какие есть столицы?
2. Запросы по прямым связям.
Who borders upon COUNTRY? - Кто граничит со страной страну COUNTRY?
Who runs through COUNTRY? (What rivers flow through COUNTRY?) - Какие реки протекают через страну COUNTRY?
What runs into LAKE? - Какие реки впадают в озеро LAKE?
Who is an ally of the COUNTRY? - Кто союзник страны COUNTRY?
3. Заросы по обратным связям.
Whom does RIVER runs into? - Куда впадает река RIVER?
4. Запросы с отрицанием в условии.
Who does not at war with COUNTRY? - Кто не воюет со страной COUNTRY?
5. Запросы со связками "и" в условии.
Who is an ally of the COUNTRY1 and does not at war with COUNTRY1? - Кто является союзником COUNTRY1 и не конфликтует с COUNTRY2?
6. Запросы со связками "или" в условии.
Who borders upon COUNTRY1 or borders upon COUNTRY2? - Кто граничит со страной COUNTRY1 или со страной COUNTRY2?
7. Считающие запросы.
How many lakes in COUNTRY? - Сколько озер в COUNTRY?
8. Да/нет запросы.
Is CITY the capital of COUNTRY? - Является ли город CITY столицей страны COUNTRY?

Еще надо придумать 4 типа запросов...
