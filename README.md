Aplicación de Consola: Integración con la API de Gutendex

Descripción del Proyecto

Esta es una aplicación basada en consola que interactúa con la API de Gutendex para obtener y procesar datos de libros. La aplicación utiliza una base de datos PostgreSQL para almacenar los datos y ofrece a los usuarios varias funcionalidades como listar autores, filtrar autores según criterios específicos y analizar datos de libros.

Funcionalidades

La aplicación ofrece las siguientes funcionalidades:

Lista de Autores

Obtener y mostrar todos los autores de la API de Gutendex.

Listar Autores Vivos en un Año Específico

Filtrar y mostrar autores que estaban vivos durante un año especificado por el usuario.

Exhibir la Cantidad de Libros en un Idioma Específico

Mostrar el total de libros disponibles en un idioma especificado por el usuario.

Recuperar Todos los Autores Vivos en un Año Especificado por el Usuario

Recopilar y mostrar todos los autores que estaban vivos en el año proporcionado por el usuario.

Endpoint de la API

La aplicación interactúa con el siguiente endpoint de la API:

Gutendex Books API: https://gutendex.com/books

Tecnologías Utilizadas

El proyecto está construido utilizando las siguientes tecnologías:

Java: Versión 17.

Maven: Gestor de dependencias (versión 4).

Spring Boot: Framework (versión 3.2.3).

PostgreSQL: Base de datos para almacenamiento de datos.

Dependencias

El proyecto fue creado a través de Spring Initializr y ya incluye las siguientes dependencias configuradas:

Spring Data JPA

Postgres Driver

Spring Boot Starter Web

Instrucciones de Configuración

Clona el repositorio en tu máquina local.

Asegúrate de tener instalada la versión 17 de Java o una versión superior.

Configura una base de datos PostgreSQL y actualiza el archivo de propiedades de la aplicación con las credenciales de tu base de datos.

Usa Maven para instalar las dependencias:

Esquema de la Base de Datos

La base de datos PostgreSQL está diseñada con el siguiente esquema:

Tablas:

Autores (Authors)

id (Clave primaria)

name (Nombre)

birth_year (Año de nacimiento)

death_year (Año de fallecimiento)

Libros (Books)

id (Clave primaria)

title (Título)

language (Idioma)

author_id (Clave foránea que referencia a Authors.id)

Flujo de la Aplicación

La aplicación obtiene datos de libros y autores desde la API de Gutendex.

Los datos se procesan y almacenan en la base de datos PostgreSQL.

Los usuarios interactúan con la aplicación a través de la consola para realizar consultas específicas y obtener resultados.

Cómo Usar

Al ejecutar la aplicación, sigue las instrucciones en la consola para seleccionar una funcionalidad:

Listar todos los autores.

Ingresar un año para listar autores vivos en ese periodo.

Especificar un idioma para ver la cantidad de libros disponibles en ese idioma.

Proporcionar un año para recuperar todos los autores vivos en ese año.

Mejoras Futuras

Implementar filtros y opciones de ordenamiento adicionales.

Agregar soporte para exportar datos a archivos CSV o JSON.

Ampliar el soporte para más endpoints de la API de Gutendex.

Licencia

Este proyecto es de código abierto y está disponible bajo la Licencia MIT.

Agradecimientos

API de Gutendex por proporcionar datos de libros y autores.

Spring Boot por su robusto framework.

PostgreSQL por su soporte confiable en bases de datos.

