# Eliminar un Álbum de la database
## Elaborado en MySQL
 
Se realizó el siguiente procedimiento almacenado: 

```MySQL
DELIMITER $$
CREATE PROCEDURE eliminar_album (IN album_id INT)
BEGIN
	DELETE FROM Album WHERE ID = album_id
END$$
DELIMITER $$;

```

Básicamente de entrada recibirá el ID de algún álbum,  
posteriormente recorrerá todos los ID de los álbumes dentro
de la tabla Álbum hasta que encuentre alguna coincidencia, 
en ese momento lo eliminará de la base de datos.