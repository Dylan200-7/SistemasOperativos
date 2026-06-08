# Semana 14 - Seguridad en Sistemas Operativos Linux

## Archivo Principal

📄 **SISTEMAS_OPERATIVOS_SEMANA_14.pdf**

Este documento contiene el desarrollo completo de la práctica realizada durante la Semana 14.

---

## Descripción

En esta semana se desarrolló una práctica de laboratorio enfocada en la implementación de mecanismos de seguridad en sistemas operativos Linux.

Se realizaron actividades relacionadas con:

- Gestión de usuarios.
- Políticas de contraseñas.
- Validación de integridad mediante hashes.
- Control de acceso.
- Aplicación del principio de mínimo privilegio.
- Administración segura de evidencias mediante Git y GitHub.

---

## Integrantes

- Mathias Dylan Henry Quispe Charres
- Josue Cristhian Mateo Mogollon Flores
- Kevin Esty Carvallo Neciosup

---

## Objetivos

- Comprender los mecanismos básicos de seguridad en Linux.
- Gestionar usuarios y grupos de forma segura.
- Aplicar políticas de contraseñas.
- Validar la integridad de archivos utilizando funciones hash.
- Configurar permisos mediante ACL.
- Aplicar el principio de mínimo privilegio.
- Gestionar evidencias utilizando Git y GitHub.

---

## Actividades Realizadas

### Capítulo 3: Políticas y Mecanismos de Seguridad

#### Creación de Usuarios

Se creó el usuario `estudiante1` y se verificó su registro dentro del sistema Linux.

#### Configuración de Políticas de Contraseña

Se analizaron los siguientes parámetros:

- `PASS_MAX_DAYS`
- `PASS_MIN_DAYS`
- `PASS_WARN_AGE`

Estos parámetros permiten controlar la vigencia y renovación de las contraseñas de los usuarios.

---

### Capítulo 4: Validación

#### Verificación de Integridad Mediante Hash

Se generó un hash SHA-256 para un archivo de prueba y posteriormente se modificó su contenido.

Resultado:

- El hash cambió completamente después de modificar el archivo.
- Se comprobó que SHA-256 permite detectar alteraciones en los archivos.

#### Validación de Usuarios

Se utilizaron los siguientes comandos:

```bash
id
groups
```

para identificar el usuario actual y los grupos a los que pertenece.

---

### Capítulo 5: Protección y Control de Acceso

#### Gestión de Grupos

Se creó el grupo `seguridad` y se agregó el usuario `estudiante1`.

#### Uso de ACL

Se instalaron y configuraron listas de control de acceso (ACL) para asignar permisos específicos sobre archivos.

Las ACL permiten una gestión más flexible que los permisos tradicionales de Linux.

---

### Capítulo 6: Modelos Formales de Protección

#### Principio de Mínimo Privilegio

Se creó un usuario con permisos limitados y se verificó que no podía modificar archivos protegidos.

#### Análisis de Privilegios

Se identificaron procesos ejecutados con privilegios elevados:

- systemd
- sshd
- cron

Estos servicios son fundamentales para el funcionamiento del sistema.

---

## Gestión Segura con Git y GitHub

Durante la práctica se realizaron las siguientes actividades:

- Configuración inicial de Git.
- Creación de repositorio privado.
- Organización de evidencias por semanas.
- Uso de archivo `.gitignore`.
- Control de versiones mediante Git.
- Publicación segura en GitHub.

---

## Archivos Incluidos

- README.md
- SISTEMAS_OPERATIVOS_SEMANA_14.pdf

---

## Conclusiones

1. Linux proporciona herramientas robustas para la administración de la seguridad.
2. La gestión adecuada de usuarios y grupos mejora el control de acceso.
3. Los algoritmos hash permiten verificar la integridad de los archivos.
4. Las ACL proporcionan un mecanismo flexible para asignar permisos.
5. El principio de mínimo privilegio reduce la superficie de ataque.
6. Git y GitHub permiten mantener evidencias organizadas y seguras mediante control de versiones.
