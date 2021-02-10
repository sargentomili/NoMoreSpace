# NoMoreSpace
Aplicación de la práctica de Desarrollo de Aplicaciones Distribuidas de la URJC, curso 2020/2021: NoMoreSpacePlease!

Este proyecto busca la creación de una web de almacenamiento de ficheros de manera distribuida, sin contar con un (por ejemplo) servidor NFS centralizado.
En su lugar tendra "instancias" permanentes que almacenen estos ficheros y pueda escalar en función de los requisitos ademas de soportar toleracia a fallos (replicación).
Cabe destacar que esas instancias, aun no tenemos la certeza de que seran finalmente, por el momento los llamaremos "Bloques".

# Entidades previstas para la aplicación:
- Usuario(s) -> Que emplean la aplicación.
- Fichero(s) -> Que pueden ser gestionados por los usuarios (ademas de atributos internos, como un fichero que puede estar en N fragmentos).
- Pool(s) -> Agrupación o relación entre usuarios y ficheros (contiene el mapa de donde esta un fichero y a quien pertenece, mapreduce).
- Bloque(s) -> Nodos, instancias...(pendiente de desarrollo) donde se encuentran físicamente los ficheros, si un fichero es más grande que un bloque, puede estar repartido entre varios.
- Panel(s) -> Representación de como es el arbol de directorios de un usuario (una carpeta es una separación visual de un arbol de directorios).

# Autores/Integrantes del proyecto
- Ildefonso Macarro Pueyo i.macarro.2016@alumnos.urjc.es
- Javier Lamparero López j.lamparero@alumnos.urjc.es
