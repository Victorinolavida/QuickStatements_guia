# Como usar QuickStatements ( guia rápida)

### Paso 1:
Debes saber el id del item que quieres modificar de [WikiData]('https://www.wikidata.org/wiki/Wikidata:Main_Page'), normalmente, lo puedes encontrar en la última parte del link
de dicho item, por ejemplo:
https://www.wikidata.org/wiki/**Q110999040**

## Paso 2: 
Debes saber la propiedad que quieres editar, y necesitas saber el codigo de la misma, aqui algunos de esos codigos como ejemplo: 

|código|propiedad|
|------|---------|
|P4793 | identifiers.org prefix   |
|P407  | language of work or name |
|P1687 | Wikidata property        | 
|P112  | founded by               |
|P136  | genre                    |
|P2002 | Twitter username         |
|P248  | stated in                |
|P195  | collection               |
|P248  | stated in                |
|P400  | platform                 | 
|P457  | foundational text        | 
|P921  | main subject             |
|P1019 | web feed URL             |
|P1640 | curator                  |
|P2647 | source of material       |
|P2650 | interested in            |  
|P2701 | file format              |
|P462  | color                    |
|P787  | spore print color        |
|P805  | statement is subject of  |  
|P941  | inspired by              |  
|P944  | Code of nomenclature     |  
|P1109 | refractive index         |
|P1163 | media type               |

## Paso 4:
Ya que tienes los dos datos anteriores, para formar una declaración en la versión 2 de **QuickStatements** necesitamos tres parametros, una entidad, una propiedad y un valor.
Un ejemplo de declaración es:
```
Q110999040|P1687|valor
```
Ahora, debes conocer que tipo de valor quieres editar al item(entidad), ya que dependiendo del tipo de dato, se hace de distinta maneta, ve la carpeta de ejemplos(**aun en contrucción**), entre los tipos de datos podemos ver:

- Strings (texto): esto incluye URL's, o información númerica, por ejemplo ID's extenas, este tipo de datos debe ir entre doble comillas **""**, por ejempo:
```
Q110999040|P1019|"https://ejemplo.es"
```
##### Esto hace que a la [Invasión rusa de Ucrania de 2022](https://www.wikidata.org/wiki/Q110999040) se le añadio la propiedad de **web feed URL** el valor de https://ejemplo.es 

- Texto sin traducción: si tienes una frase o palabra que no tiene traducción , puedes recalcal que dicha palabra NO tiene traduccion en otro idioma, ejemplo:
```
Q1214098|P1476|pl:"Krzyżacy"
```
##### Esto hace que el libro [The Knights of the Cross](https://www.wikidata.org/wiki/Q1214098) tenga como titulo **Krzyżacy** del Polaco.

## Paso 5
Una vez tienes todos tus declaraciónes, debes ir al link de [QuickStatements](https://quickstatements.toolforge.org/#/) , debes loguearte para poder usar la herramienta y debes pegar tus declaraciones (o subir un csv, mas infromacion en la parte de ejemplos) y enviar tus declaraciones.

![Imagen de ejemplo](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e9/QuickStatement_V2_intro_screen.png/640px-QuickStatement_V2_intro_screen.png)

clickeando en **new batch** se abrirar una pantalla como esta 

![Imagen de ejemplo](https://addshore.com/wp-content/uploads/2020/07/image-6-1024x462.png)

y ahi puedes pegar todas tus nuevas declaraciones, finalmente para terminar , le das click a **Import v1 commants** lo cual subira tus declaraciones.

### Si necesitas más informacion, consulta la documentación oficial.
<https://www.wikidata.org/wiki/Help:QuickStatements>