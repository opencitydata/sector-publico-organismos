Este repositorio contiene el material relacionado con el vocabulario sobre organismos para España, que a partir del 25 de julio de 2018 se comenzará a identificar (y publicar) en la siguiente URI:

http://vocab.linkeddata.es/datosabiertos/def/sector-publico/organizacion

Previamente este vocabulario se identificaba mediante la URI http://datos.gob.es/def/sector-publico/organizacion, que se generó como resultado del trabajo encargado por el Ministerio de Hacienda y Administraciones Públicas para la generación de RDF sobre el directorio DIR3 (se puede ver la noticia en http://datos.gob.es/es/noticia/publicado-el-contenido-del-directorio-comun-dir3-en-formato-abierto-y-reutilizable-rdf-xml). A su vez, esta implementación se basó en el documento de trabajo del grupo W3C Open Data Spain alojado en https://docs.google.com/document/d/1W3ki8kY4P8_Z_gSWOHtdOgYLBwMQMSPj5XxhJBGiDlM

Las versiones iniciales de este vocabulario fueron mantenidas en el repositorio general sobre vocabularios de datos abiertos https://github.com/opencitydata/vocabularios-datos-abiertos, que actualmente se encuentra en estado *deprecated*, dado que en 2018 se ha decidido crear un repositorio en GitHub por cada uno de los vocabularios con los que se trabaja en la iniciativa global OpenCityData.

### Lista de cambios
* [1/03/2018] Añadido fichero de la ontología.
* [03/05/2018] Aceptado pull request para la generación de documentación [[OnToology update #2]](https://github.com/opencitydata/sector-publico-organismos/pull/2)
* [25/07/2018] Modificación de la implementación de la ontología para facilitar la generación de datos no sólo de DIR3, sino también de los organigramas de los ayuntamientos. Estos son los cambios más representativos de esta versión:
* * Modificación de la URI de http://datos.gob.es/def/sector-publico/organizacion a http://vocab.linkeddata.es/datosabiertos/def/sector-publico/organizacion
* * Eliminación de owl:import innecesarios, como el de esadm (territorio) y SKOS.
* * Actualización de skos:ConceptScheme utilizados. Se han actualizado los de tipo de entidad (http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/organizacion/tipo-entidad), nivel de administración (http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/organizacion/nivel-administracion) y estado de la entidad (http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/organizacion/estado-entidad).
* * Eliminación de skos:ConceptScheme innecesarios, como ServicioOficina y AmbitoTerritorial.
* * Actualización de rangos incorrectos en las Object Properties que tenían referencias a skos:ConceptScheme.
* * Modificación de los nombres de algunas propiedades, como estado, que ahora se convierte a estadoEntidad
* * Reorganización de la jerarquía de propiedades (unidadRaiz es ahora subclase de org:unitOf)

### Cambios propuestos
Por un lado, se trabajará en mejorar la documentación del vocabulario, y también se modificarán más elementos teniendo en cuenta las implantaciones realizadas por diversos ayuntamientos
