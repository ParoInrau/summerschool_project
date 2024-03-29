# Онтология Бухгалтерской отчетности организаций и ИП (Росстат)

|Описание| Свойства|
|:------------ |:-----|
|Текущая версия: | https://w3id.org/datafabric.cc/ontologies/rosstat# |
|Download serialization: | RDF/XML N-Triples TTL|
|Лицензия:|http://insertlicenseURIhere.org|

## Описание

Онтология бухгалтерской отчетности организаций и индивидуальных предпринимателей предназначена для отображения данных бухгалтерских балансов, размещенных на сайте Росстата http://www.gks.ru/accounting_report.

## Содержание

1. Введение
    1. Определение пространств имен
        1. Используемые пространства имен
2. Обзор классов и свойств
    1. Свойства объекта
    2. Свойства данных
    3. Поименованные классы
3. Описание Data cube
    1. Оси куба
    2. Меры куба
4. Перекрестные ссылки: классы, свойства и свойства данных
    1. Object Properties
    2. Data Properties
    3. Named Individuals
    4. Легенда


## Введение

Онтология спроектирована для представления данных из реестра Росстата в графовую структуру. 
Такой формат моделирования данных был избран для сохранения структуры представления данных, которая используется в бухгалтерских балансах.

Структура онтологии организована вокруг следующих базовых классов:

- баланс,
- раздел баланса,
- строка баланса,
- справочники.

## Определение пространств имен

### Используемые пространства имен

|Название| Ссылка|
|:------------ |:-----|
|formalorganizations	|<https://spec.edmcouncil.org/fibo/ontology/FND/Organizations/FormalOrganizations/> |
|owl|	<http://www.w3.org/2002/07/owl#>|
|concept|	<http://purl.org/linked-data/sdmx/2009/concept#>|
|xsd|	<http://www.w3.org/2001/XMLSchema#>|
|rdfs|	<http://www.w3.org/2000/01/rdf-schema#>|
|measure|	<http://purl.org/linked-data/sdmx/2009/measure#>|
|rdf|	<http://www.w3.org/1999/02/22-rdf-syntax-ns#>|
|terms|	<http://purl.org/dc/terms/>|
|attribute|	<http://purl.org/linked-data/sdmx/2009/attribute#>|
|cube|	<http://purl.org/linked-data/cube#>|
|vann|	<http://purl.org/vocab/vann/>|
|dimension|	<http://purl.org/linked-data/sdmx/2009/dimension#>|
|rosstat|	<https://w3id.org/datafabric.cc/ontologies/rosstat#>|

## Обзор классов и свойств

Представленная онтология состоит из следующих классов и свойств:

### Свойства объекта:

1. Организация.

### Свойства данных:

1. Выручка,
2. Дебиторская задолженность,
3. Денежные средства,
4. Запасы,
5. Кредиторская задолжность,
6. Налог на прибыль,
7. Нераспределенная прибыль (непокрытый убыток),
8. Период,
9. Чистая прибыль (убыток).

### Поименованные классы:

1. RDF Data Cube: схема данных бухгалтерской отчетности организаций и ИП,
2. Бухгалтерская отчетность организации или ИП за отчетный период,
3. Выручка,
4. Дебиторская задолженность, 
5. Денежные средства,
6. Запасы,
7. Кредиторская задолжность,
8. Налог на прибыль,
9. Нераспределенная прибыль (непокрытый убыток),
10. Организация,
11. Период,
12. Чистая прибыль (убыток).

## Описание Data cube

Data cube схемы данных бухгалтерской отчетности организаций и ИП состоит из осей и мер.

### Оси куба:
- Период,
- Организация.

### Меры куба:
- 1210 Запасы,
- 1230 Дебиторская задолженность,
- 1520 Кредиторская задолжность,
- 1250 Денежные средства,
- 1370 Нераспределенная прибыль (непокрытый убыток),
- 2400 Чистая прибыль (убыток),
- 2110 Выручка,
- 2410 Налог на прибыль.


## Перекрестные ссылки: классы, свойства и свойства данных

### Object Properties
#### Организация
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#refOrganization`

`has range`
`formal organization c`
`is also defined as`
`named individual`
----
### Data Properties
#### Выручка
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-2110`

`has super-properties`
`obs value dp`
`has range`
`decimal`
`is also defined as`
`named individual`

#### Дебиторская задолженность
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-1230`

`has super-properties`
`obs value dp`
`has range`
`decimal`
`is also defined as`
`named individual`

#### Денежные средства
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-1250`

`has super-properties`
`obs value dp`
`has range`
`decimal`
`is also defined as`
`named individual`

#### Запасы
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-1210`

`has super-properties`
`obs value dp`
`has range`
`decimal`
`is also defined as`
`named individual`

#### Кредиторская задолжность
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-1520`

`has super-properties`
`obs value dp`
`has range`
`decimal`
`is also defined as`
`named individual`

#### Налог на прибыль
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-2410`

`has super-properties`
`obs value dp`
`has range`
`decimal`
`is also defined as`
`named individual`

#### Нераспределенная прибыль (непокрытый убыток)
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-1370`

`has super-properties`
`obs value dp`
`has range`
`decimal`
`is also defined as`
`named individual`

#### Период
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#refPeriod`

`has super-properties`
`ref period dp`
`has range`
`g year`
`is also defined as`
`named individual`

#### Чистая прибыль (убыток)
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-2400`

`has super-properties`
`obs value dp`
`has range`
`decimal`
`is also defined as`
`named individual`

----
### Named Individuals
#### RDF Data Cube: схема данных бухгалтерской отчетности организаций и ИП
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#RosstatAccountingReportDSD`

`belongs to`
`data structure definition c`

#### Бухгалтерская отчетность организации или ИП за отчетный период
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#SliceByYearAndOrg`

`belongs to`
`slice key c`

#### Выручка
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-2110`

`belongs to`
`measure property c`
`is also defined as`
`data property`

#### Дебиторская задолженность
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-1230`

`belongs to`
`measure property c`
`is also defined as`
`data property`

#### Денежные средства
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-1250`

`belongs to`
`measure property c`
`is also defined as`
`data property`

#### Запасы
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-1210`

`belongs to`
`measure property c`
`is also defined as`
`data property`

#### Кредиторская задолжность
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-1520`

`belongs to`
`measure property c`
`is also defined as`
`data property`

#### Налог на прибыль
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-2410`

`belongs to`
`measure property c`
`is also defined as`
`data property`

#### Нераспределенная прибыль (непокрытый убыток)
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-1370`

`belongs to`
`measure property c`
`is also defined as`
`data property`

#### Организация
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#refOrganization`

`belongs to`
`dimension property c`
`is also defined as`
`object property`

#### Период
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#refPeriod`

`belongs to`
`dimension property c`
`is also defined as`
`data property`


#### Чистая прибыль (убыток)
`IRI: https://w3id.org/datafabric.cc/ontologies/rosstat#measure-2400`

`belongs to`
`measure property c`
`is also defined as`
`data property`

----
### Легенда
|Сокращение|Расшифровка|
|:---|:---|
|c | Классы |
|op| Object Properties |
|dp| Data Properties |
|ni| Named Individuals|
