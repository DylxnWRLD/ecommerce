# Cómo insertar un álbum
## Elaborado en MySQL

Para insertar un álbum, simplemente tenemos que poner los datos de la siguiente manera: 

```MySQL
INSERT INTO Album (ID, Titulo, FechaLanzamiento, IDArtista)
VALUES (1, 'Goodbye & Good Riddance', '2018-05-23', 1); -- JuiceWRLD

```

Este es un ejemplo de cómo se vería la tabla con el dato:

| Atributo | Dato |
|-|-|
| ID | 1 |
| Título | Goodbye & Good Riddance |
| FechaLanzamiento | 2018-05-23 |
| IDArtista | 1 | 