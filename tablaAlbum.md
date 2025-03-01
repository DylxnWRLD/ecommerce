# Creación de la Tabla para los Álbumes
## Elaborado en MySQL

### Elementos de la Tabla:

* ID: Un campo de tipo INT que se autoincrementa y se usa como clave primaria
(PRIMARY KEY).  
* Titulo: Un campo de tipo VARCHAR(255) que no puede ser NULL y almacena el
título del álbum.
* FechaLanzamiento: Un campo de tipo DATE que no puede ser NULL y almacena
la fecha de lanzamiento del álbum.
* IDArtista: Un campo de tipo INT que actúa como clave foránea que se refiere al ID
de la tabla Artista. La opción ON DELETE CASCADE asegura que, si se elimina un
artista, los álbumes asociados también serán eliminados. La opción ON UPDATE
CASCADE asegura que si el ID de un artista cambia (lo cual es poco probable),
también se actualicen los IDArtista en los álbumes.
* FOREIGN KEY (IDArtista) REFERENCES Artista(ID) ON DELETE
CASCADE ON UPDATE CASCADE: Establece la relación de clave foránea con
la tabla Artista.
* UNIQUE (Titulo, IDArtista): Funciona como índice secundario. Garantiza que no
haya dos álbumes con el mismo título para el mismo artista. Permite realizar
búsquedas o consultas en la tabla que involucren estas columnas de forma más rápida,
ya que el índice ayuda a optimizar el rendimiento de las operaciones de búsqueda,
inserción y actualización.

