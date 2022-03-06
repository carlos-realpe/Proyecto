# Proyecto
Cómo funciona Amazon S3 
Amazon S3 es un servicio de almacenamiento de objetos que almacena datos como objetos dentro de buckets. Un objeto es un archivo y cualquier metadato que describa ese archivo. Un bucket es un contenedor de objetos. 
Bucket(valde) es el contenedor donde se almacenan los objetos, estos objetos que son, son imágenes, videos, archivos javascripts entre otros
El nombre debe ser único en todo amazon web server
Para almacenar datos en Amazon S3, primero debe crear un bucket y especificar un nombre de bucket y Región de AWS. A continuación, cargue datos a ese bucket como objetos en Amazon S3. Cada objeto tiene unclave(oNombre de clave), que es el identificador único del objeto dentro del bucket. 
S3 proporciona funciones que puede configurar para admitir su caso de uso específico. Puede utilizar S3 Versioning para mantener varias versiones de un objeto en un bucket y restaurar objetos que se eliminan o sobrescriben accidentalmente. 
Los buckets y los objetos que contienen son privados y solo se puede acceder a ellos si concede explícitamente permisos de acceso. Puede utilizar políticas de bucket,AWS Identity and Access Management(IAM), listas de control de acceso (ACL) y puntos de acceso S3 para administrar el acceso. 

PRACTICA QUE SE REALIZO
En la practica que se realizo de Amazon S3 creamos un bucket donde procedimos a subir una pagina web estatica, el nombre del bucket debe ser único en todo amazon web server al crear el bucket seleccionamos si deseamos que los archivos que se encuentren en el bucket se puedan hacer público, por defecto se encontraran privados.
En Control de versiones de buckets nos va a permitir crear diferentes versiones del mismo archivo, es decir su subimos un archivo con el mismo nombre en lugar de reemplazar el archivo crea una nueva versión del mismo archivo.
Por ultimo tenemos la opción de Object Lock en la cual permite que los objetos se bloqueen por una determinada cantidad de días o de forma indefinida para que nadie pueda eliminar o modificar dichos archivos.
Una vez creado el bucket procedemos a subir nuestro archivo entrado al bucket creado y dandole click a update file o simplemente arrastrando.
Una vez creado el bucket realizamos configuracion en los permisos y habilitamos el alojamiento de sitios web estaticos.
Para configurar permisos nos dirigimos al apartado permisos, Amazon S3 recomienda realizar este tipo de configuracion por IAM o por politicas de bucket, en nuestro caso lo hicimos por politicas de bucket donde procedimos a generar las politicas respectivas
