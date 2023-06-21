# Pruebas de Operaciones CRUD con Jest

Este repositorio contiene pruebas unitarias para verificar el buen funcionamiento de las operaciones CRUD de cafés en un servidor. Las pruebas se realizan con `Jest` y `supertest`.

## Requisitos

- Node.js (v10 o superior)

## Ejecución de las pruebas

Para ejecutar las pruebas, utiliza el siguiente comando:

    npm run test

*Esto ejecutará las pruebas y mostrará los resultados en la consola.*

## Descripción de las pruebas

Las pruebas se dividen en cuatro escenarios diferentes, cada uno de ellos prueba un aspecto específico de las operaciones CRUD de cafés:

  1. Obtener cafés:

     * Prueba que la ruta GET /cafes devuelve un código de estado 200 y un arreglo con al menos un objeto de café.

  2. Eliminar café inexistente:

     * Comprueba que se obtiene un código de estado 404 al intentar eliminar un café con un ID que no existe.

  4. Agregar nuevo café:

     * Prueba que la ruta POST /cafes agrega un nuevo café y devuelve un código de estado 201.

  5. Actualizar café:

     * Prueba que la ruta PUT /cafes devuelve un código de estado 400 si se intenta actualizar un café enviando un ID en los parámetros que sea diferente al ID dentro del payload.

*Cada prueba incluye una descripción detallada de lo que se está probando y qué resultados se esperan.*
