# Parte 2: Caso de Uso

**ID:**  CU-01
**Nombre:** Sistema de likes.

**Actor Principal:**  El usuario.
**Actores Secundarios:** La base de datos

## Descripcion

- El sistema permite a un usuario dar like a un artículo, pero solo puede hacerlo una vez.

## Precondiciones

- El usuario debe estar registrado.
- El artículo debe estar publicado.
- El usuario no debe haber dado like a ese mismo artículo.

## Flujo Principal

1. El usuario ingresa a la sección de artículos.
2. El usuario entra a un artículo.
3. El usuario hace clic en "like".
4. El sistema verifica que ese usuario no haya dado like antes.
5. El sistema incrementa la cantidad de likes en ese artículo.
6. La base de datos guarda el cambio de la cantidad de likes.
7. Fin del caso de uso.

## Flujos Alternativos

### FA1

1. El sistema verifica que el usuario ya dió like a ese artículo.
2. El sistema muestra un mensaje al usuario que dice "solo se puede dar like una vez".
3. El sistema no incrementa la cantidad de likes.
4. Fin del caso de uso.

### FA2

1. El usuario desea quitar like a un artículo.
2. El usuario hace clic en "ya no me gusta".
3. El sistema decrementa la cantidad de likes en ese artículo.
4. La base de datos guarda el cambio de la cantidad de likes.
5. Fin del caso de uso.

## Postcondiciones

- El usuario no puede dar like de nuevo a ese artículo.
- La cantidad de likes en ese artículo queda actualizada.
- El sistema muestra la cantidad de likes actualizada a todos los usuarios.


