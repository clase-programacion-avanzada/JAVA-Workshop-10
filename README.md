# Taller 10 - Reportes de la aplicación de música

En este taller se trabajará la carga y escritura de archivos de texto y binarios. Se trabajará sobre el proyecto de la aplicación de música que se ha venido desarrollando en los talleres anteriores.

## Indice

1. [Enunciado](#enunciado)
2. [Calificación](#calificación)
3. [¿Qué sigue?](#¿qué-sigue?)
4. [Recursos en línea](#recursos-en-línea)


## Enunciado

El proyecto debe ser modificado para agregar un nuevo módulo que permita la generación de reportes. Los reportes deben ser guardados en archivos de texto y deben ser mostrados en pantalla. Los reportes que se deben generar son los siguientes:

1. Se debe mostrar la cantidad de canciones que tiene cada artista. El reporte debe ser guardado en un archivo de texto llamado `reporte_artistas.txt`. El formato del archivo debe ser el siguiente:

    ```
    Reporte de artistas
    
    <Nombre del artista 1>: <Cantidad de canciones>
    <Nombre del artista 2>: <Cantidad de canciones>
    ...
    <Nombre del artista n>: <Cantidad de canciones>
    
    Total de canciones: <Cantidad total de canciones>
    
    ```

2. Se debe mostrar la popularidad de cada artista (Si un artista no existe dentro de las listas de reproducción, o no es seguido, no debe mostrarse en el reporte). La popularidad de un artista se calcula de la siguiente manera:
   
   - Si un artista aparece en una lista de reproducción, se le suma 1 a su popularidad por cada canción que tenga en la lista de reproducción.
   - Por cada follow que tenga un cliente de un artista, se le suma 2 a la popularidad del artista.

    El reporte debe ser guardado en un archivo de texto llamado `reporte_popularidad.txt`. En este archivo deben aparecer los artistas con una popularidad mayor a 0. El formato del archivo debe ser el siguiente:    

    ```
    Reporte de popularidad
    
    <Nombre del artista 1>: <Popularidad>
    <Nombre del artista 2>: <Popularidad>
    ...
    <Nombre del artista n>: <Popularidad>
    
    ```
3. Para cada cliente, se debe mostrar la cantidad de canciones que tiene en sus listas de reproducción, la cantidad de artistas que sigue y el nombre del artista que más escucha (Este artista será el que más se repita en las listas de reproducción). El reporte debe ser guardado en un archivo de texto llamado `reporte_clientes.txt`. El formato del archivo debe ser el siguiente:

    ```
    Reporte de clientes
    
    <Nombre del cliente 1>
    - Canciones en listas de reproducción: <Cantidad de canciones>
    - Artistas seguidos: <Cantidad de artistas>
    - Artista que más escucha: <Nombre del artista>
   
    <Nombre del cliente 2>
    - Canciones en listas de reproducción: <Cantidad de canciones>
    - Artistas seguidos: <Cantidad de artistas>
    - Artista que más escucha: <Nombre del artista>
   
    ...
   
    <Nombre del cliente n>
    - Canciones en listas de reproducción: <Cantidad de canciones>
    - Artistas seguidos: <Cantidad de artistas>
    - Artista que más escucha: <Nombre del artista>
   
    ```

[Volver al índice](#indice)

## Calificación

El programa debe compilar y ejecutar sin errores. Se debe cumplir con los siguientes requerimientos:

1. Las clases deben estar en los paquetes correctos (servicios, controladores, vistas, modelos y excepciones). (0.5)
2. La clase `Main` y las clases del paquete `views` son las únicas que pueden interactuar con el usuario.(0.5)
3. Los controladores deben llamar a los métodos de los servicios correspondientes.(0.5)
4. Los servicios deben llamar a los métodos de las clases del paquete `models` correspondientes.(0.5)
5. El programa debe escribir los reportes en archivos de texto con el formato indicado.(1.0)
6. El programa debe mostrar los reportes en pantalla.(1.0)
7. Los reportes deben mostrar la información correcta.(1.0)

**Este taller hace parte de su proyecto. Los posteriores talleres no se calificarán hasta que se haya completado este.
Si todo está correcto, sumará 1.0 a su proyecto final.
Este taller debe ser entregado durante la semana 14**

## ¿Qué sigue?

El proyecto parece completo, sin embargo, aún falta implementar un sistema de jerarquía de usuarios. En el siguiente taller se trabajará en la implementación de este sistema.
## Recursos en línea

- [Sort a HashMap in Java](https://www.baeldung.com/java-hashmap-sort) [Artículo]