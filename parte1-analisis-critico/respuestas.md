# Parte 1: Analisis Critico - Respuestas

**Nombre del estudiante:**  Leonardo Krell
**Fecha:** 26/05/2026

---

## Error 1

**Ubicacion:** Precondiciones

**Descripcion:** Que una precondición sea que el usuario tenga al menos 50 seguidores es innecesario y no se relaciona con la edición de su perfil.

**Correccion:** Quitar esa precondición, ya que las precondiciones deben ser estados previos necesarios para realizar el proceso.

---

## Error 2

**Ubicacion:** Flujo principal

**Descripcion:** En el paso 5, el usuario hace clic en "Guardar cambios" y los cambios se guardan inmediatamente en el paso 6 sin pedirle al usuario que confirme.

**Correccion:** Agregar dos pasos entre el 5 y 6. Uno que le pida confirmación al usuario y otro donde este confirme. Luego guardar cambios.

---

## Error 3

**Ubicacion:** Flujos alternativos

**Descripcion:** No hay ningún flujo alternativo.

**Correccion:** Agregar flujos alternativos. Por ejemplo, que el usuario retroceda antes de guardar los cambios o que el usuario haga clic en cancelar.

---

## Error 4

**Ubicacion:** Postcondiciones

**Descripcion:** Las postcondiciones "El sistema envía un correo electrónico a todos los seguidores del usuario", "El administrador recibe una alerta instantánea", "Se abre automáticamente una nueva sesión del usuario en otro navegador" no son necesarias para el proceso de editar perfil. No es necesario enviar un correo a todos los seguidores del usuario para notificar los cambios. Tampoco es necesario alertar al administrador. Y que se abra una nueva sesión en otro navegador no tiene sentido, ya que el usuario realizó los cambios en esa sesión y no necesita que se abra otra.

**Correccion:** Eliminar las últimas tres condiciones y en su lugar agregar "los cambios son visibles para todos los usuarios".

---

## Error 5

**Ubicacion:** Actores

**Descripcion:** No hay actor secundario.

**Correccion:** Agregar a la Base de Datos (donde se guardan los cambios) como actor secundario.



