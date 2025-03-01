# MUSICPEDIA
## Proyecto para BD Relacionales e IHC / 3er Semestre
### Alumno: Flores Nuñez

MusicPedia es una plataforma donde se encuentra información relacionada al mundo de la
música. La entidad principal es Artista. Cada artista tiene un ID único que lo caracteriza y un
nombre. Un artista puede ser individual o un grupo. Un artista individual tiene una fecha de
nacimiento y una nacionalidad. Un grupo de artistas tiene una fecha de creación y una lista
de integrantes. Un artista debe tener N canciones, una canción tiene un ID único que la
identifica, así como una descripción, un título, una duración, y un género de una lista de
géneros.

Cada canción es única e irrepetible dentro de MusicPedia. Un artista puede tener N álbumes,
un álbum tiene un ID único que lo caracteriza, así como un título y una fecha de lanzamiento.
N canciones pueden pertenecer a M álbumes.

N Artistas pueden colaborar con N artistas, ya sea individuales o grupales, para crear una
colaboración, la colaboración tiene una descripción y una fecha de creación. Una
colaboración entre artistas puede resultar en N canciones.