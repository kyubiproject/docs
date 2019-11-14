# Tipos de dato

Primero queremos despejar posibles dudas y aclarar que los tipos de datos finales no difiere de los soportados por el lenguaje. 
__Kyubi__ promueve la programación implicita y evalua la singularidad de tus definiciones, por lo cual si lo definiste una vez ese será el comportamiento de cada campo y/o objeto, no obstante, 
si deseas cambiar o establecer un comportamiento particular puedes hacerlo sin problema alguno.  

## Frecuentes

Tipo | SQL | Rules | Input | View
:---: | :---: | :---: | :---: | :---:
string | VARCHAR(100) | | text | text
word | VARCHAR(60) | | text | text
password | VARCHAR(60) | password | password | -
email | CHAR(96) | email | email | email
phone | VARCHAR(20) | | tel | text
color | CHAR(7) | color | color | color
money | FLOAT | number | money | money
percent | FLOAT | number | percent | percent
dni | CHAR(20) UNIQUE | unique | text | text
code | CHAR(20) | | text | text
url | CHAR(255) | url | url | link
path | CHAR(255) | | text | link
slug | CHAR(255) | slug | text | text

## HTML

Tipo | SQL | Rules | Input | View
:---: | :---: | :---: | :---: | :---:
confirm | BIT(1) | boolean | check | text
button | BIT(1) | boolean | button | text
toggle | ENUM(A, B) | in | toggle | text
select | ENUM(...) | in | select | text
radiolist | ENUM(...) | in | radiolist | text
multiple | SET(..) | in, filter.json_encode | select.multiple | mixed
checklist | SET(...) | in, filter.json_encode | checklist | mixed
list | JSON | filter.json_encode | select.tags | mixed
slider | SMALLINT | | slider | number
range | DECIMAL | range | range | mixed
text | VARCHAR(100) | | text | text
textarea | TEXT | | textarea | ntext
html | BLOB | html | editor | html

## Epeciales

Tipo | SQL | Rules | Input | View
:---: | :---: | :---: | :---: | :---:
alpha | CHAR(30) | match | text | text
alpha_num | CHAR(30) | match | text | text
alpha_dash | CHAR(30) | match | text | text
line | VARCHAR(255) | | text.row | text
uuid | CHAR(36) DEFAULT[UUID()] UNIQUE | match, unique | text | text
ip/ipv4 | CHAR(15) | match | text | text
ipv6 | CHAR(23) | match | text | text
mac | CHAR(17) | match | text | text

- __file|image__: FK[extra__file.id]
- __file_path|image_path__: CHAR(255)
- __file_binary|image_binary__: LONGBLOB
- __curl__: FK[extra__curl.id]

Los campos podrian tener una formato particular adicional


## SQL
- __boolean__: BIT(1)
- __small__: SMALLINT
- __medium__: MEDIUMINT
- __big__: BIGINT
- __datetime__: TIMESTAMP

## Opciones
- __auto__: UNIQUE NOT NULL AUTO_INCREMENT
- __required__: NOT NULL
- __!__: PRIMARY KEY
- __?__: UNIQUE
- __*__: NOT NULL
- __+__: UNSIGNED
- __0__: ZEROFILL
  
## Predefinidos
- __id__: MEDIUMINT(8) UN NN AI PK
- __now__: TIMESTAMP DEFAULT[CURRENT_TIMESTAMP]
- __created__: TIMESTAMP DEFAULT[CURRENT_TIMESTAMP]
- __updated__: TIMESTAMP DEFAULT[@NULL ON UPDATE CURRENT_TIMESTAMP]
- __deleted__: TIMESTAMP

