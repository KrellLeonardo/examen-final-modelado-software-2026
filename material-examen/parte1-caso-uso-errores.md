# Parte 1 del Examen: Analisis Critico

**Tiempo:** 20 minutos  
**Puntaje:** 20% del examen final

---

## Consigna

A continuacion se presenta un caso de uso con **7 errores intencionales**. Tu tarea es:

1. Identificar minimo 5 errores
2. Explicar por que es un error
3. Proponer la correccion apropiada

Usa este formato:

```text
ERROR #1:
Ubicacion: [Seccion donde esta el error]
Descripcion: [Que esta mal]
Correccion: [Como deberia ser]
```

---

## Caso de Uso con Errores

### CU-09: Editar Perfil de Usuario

**Actor Principal:** Servidor, Usuario Registrado

**Descripcion:**  
El servidor permite que el usuario cambie los datos de su perfil cuando lo necesita.

**Precondiciones:**
- El usuario debe existir en el sistema
- El usuario debe tener al menos 50 seguidores
- El usuario debe haber cambiado su foto de perfil en las ultimas 24 horas

**Flujo Principal:**
1. El Usuario Registrado ingresa a su perfil
2. El Usuario Registrado hace clic en "Editar perfil"
3. El sistema muestra el formulario con sus datos actuales
4. El Usuario Registrado modifica nombre, email y biografia
5. El Usuario Registrado hace clic en "Guardar cambios"
6. El sistema guarda la informacion inmediatamente
7. El sistema muestra mensaje "Perfil actualizado"
8. Fin del caso de uso

**Flujos Alternativos:**
- Ninguno

**Postcondiciones:**
- El perfil queda actualizado en la base de datos
- El sistema envia un email a todos los seguidores del usuario
- El administrador recibe una alerta instantanea
- Se abre automaticamente una nueva sesion del usuario en otro navegador

**Excepciones:**
- Si el usuario no tiene permisos, el sistema no hace nada

---

## Recordatorio

Busca errores en:
- Actores
- Precondiciones
- Flujo principal
- Flujos alternativos
- Postcondiciones
- Excepciones
