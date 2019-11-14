# Recomendaciones

## Estándares de nomenclatura
Utiliza convenciones y/o estándares de nomenclatura, forma parte de las buenas prácticas y facilitará la lectura del código, de esta forma será entendible y mantenible por terceros sobre todo. 

##### 1. PascalCase
Cadena capitalizada sin espacios, las letrás mayúsculas delimitan los espacios.

##### 2. camelCase 
Igual a __PascalCase__, la primera letra va minúscula.

##### 3. snake_case:
Todo va en minúscula,  utiliza el guión bajo `_` para los espacios..

##### 4. kebab-case
Igual a __snake_case__,  utiliza el guión `-` para los espacios.

##### 5. SCREAMING_CASE
Variante del __snake_case__ con la diferencia todo va en mayúscula.  

##### 6. Train_Case
Variante del __PascalCase__,  utiliza el guión bajo `_` para los espacios.

##### 6. Dotted
Variante del __snake_case__,  utiliza el punto `.` para los espacios.


## PHP
- __PascalCase__: nombres de clases, namespaces.
- __camelCase__: atributos y métodos dentro de una clase.
- __snake_case__: nombre variables, métodos y/o funciones globales.
- __kebab-case__: nombre de ficheros.
- __UPPER_CASE__: variables estáticas, constantes.
- Utiliza un (1) guión bajo "_" para variables __protected__.
- Utiliza dos (2) guiones bajos "__" para variables __private__.

## SQL
- __snake_case__: nombra tus base de datos, tablas y campos.
- __camelCase__: nombre de funciones, procedimientos y variables.
- Nombra tus tablas es singular.
- No agregues prefijos innecesarios a tus campos.
- Llama tu clave primaria `id`.
- Define tus clave foránea de la forma `<tabla>_<campo>`.
- Sí una tabla se vincula de forma directa y única al padre, utiliza el mismo nombre del campo.
- Si defines un módulo o componente, añade un prefijo a tus tablas (no en tus columnas).

## CSS
- __kebab-case__: clases.
- __snake_case__: id.
- Si una clase es una particularización de otra añádela como prefijo, acompañado de dos (2) guiones "--".

`Recuerda solo son "recomendaciones" por lo cual pueden ser pasadas por alto.`