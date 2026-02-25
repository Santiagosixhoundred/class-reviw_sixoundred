# Sistema de Gestión Médica (Base de Datos MySQL)

Este proyecto es una base de datos diseñada para gestionar los procesos básicos de una clínica u hospital. Incluye el registro de médicos, pacientes, citas, diagnósticos y recetas, todo organizado de forma que los datos sean confiables y fáciles de consultar
--
## ¿Qué hace este sistema?

El objetivo principal es tener toda la información médica centralizada en una sola base de datos, evitando errores y duplicados. Algunas de las cosas que permite hacer:

* Registrar y consultar médicos por especialidad y facultad.
* Agendar citas vinculando pacientes, médicos y sedes.
* Guardar diagnósticos y recetas por consulta.
* Registrar automáticamente cualquier error que ocurra durante una operación.
---
---
## Procedimientos almacenados

Para interactuar con los datos se usan procedimientos almacenados. Cada entidad tiene los suyos para crear, consultar, actualizar y eliminar registros.
---
## Registro de errores (Logs)

El sistema guarda automáticamente cualquier error en una tabla llamada `logs`. Esto hace más fácil detectar qué salió mal y cuándo

```
```

## Usuarios y permisos
Se definieron cuatro tipos de usuario, cada uno con acceso solo a lo que necesita:

## Tecnologías usadas

* MySQL
* Procedimientos almacenados y funciones
* Control de errores con `DECLARE EXIT HANDLER`

## Cómo usar el proyecto

1. Importar el archivo `.sql` en tu servidor MySQL.
2. Crear los usuarios con los roles correspondientes

3.  Ejecutar los procedimientos según la operación que necesites