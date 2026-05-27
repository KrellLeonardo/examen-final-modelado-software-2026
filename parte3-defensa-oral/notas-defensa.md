# Parte 3: Notas para Defensa Oral

## Presentacion del Proyecto

- Nombre del proyecto: Sistema de likes.
- Feature principal: Permitir que los usuarios puedan dar y quitar “me gusta” a artículos publicados, y hacerlo solo una vez.
- Arquitectura general: Arquitectura MVC.

## Decisiones de Diseno

- Estructura de clases:
  - Usuario
  - Articulo
  - Like
  - BaseDeDatos
  - SistemaLikes

- Uso de MVC:
  - Modelo: Es la lógica del programa.
  - Vista: Es lo que ve el usuario.
  - Controlador: Es el intermediario entre el modelo y la vista.

- Patrones identificados:
  - MVC.

## Defensa del Caso de Uso

- Que funcionalidad modele:
  - La funcionalidad de dar y quitar “me gusta” a artículos publicados.

- Que clases agregue:
  - Usuario
  - Articulo
  - Like
  - BaseDeDatos
  - SistemaLikes

- Como se relacionan:
  - SistemaLikes interactúa con Usuario para verificar si ya dio like a un artículo.
  - SistemaLikes se comunica con Articulo para aumentar o disminuir la cantidad de likes según la acción del usuario.
  - Después de registrar o eliminar un like, SistemaLikes utiliza BaseDeDatos para guardar y actualizar la información.
  - La BaseDeDatos almacena y actualiza los objetos Like.
  - La clase Like funciona como una entidad de relación entre Usuario y Articulo, guardando datos como el identificador y la fecha del like.

## Conceptos a Repasar

- Actor primario y secundario
- Precondicion y postcondicion
- Diferencia entre diagrama de clases y secuencia
- Principios SOLID basicos
