# Capítulo 3: Políticas y Mecanismos de Seguridad

## Actividad 1: Creación de Usuarios

### Comandos Ejecutados

```bash
sudo useradd estudiante1
sudo passwd estudiante1
cat /etc/passwd | grep estudiante1
```

### Resultado Obtenido

Se creó correctamente el usuario `estudiante1` y se verificó su registro dentro del sistema Linux.

### Pregunta

**¿Por qué es importante asignar cuentas individuales?**

Es importante asignar cuentas individuales porque permite identificar a cada usuario de manera única dentro del sistema. Esto facilita la auditoría de actividades, mejora la seguridad, permite aplicar permisos específicos y evita que varios usuarios compartan credenciales.

---

## Actividad 2: Configuración de Políticas de Contraseña

### Comando Ejecutado

```bash
sudo cat /etc/login.defs
```

### Parámetros Identificados

* PASS_MAX_DAYS
* PASS_MIN_DAYS
* PASS_WARN_AGE

### Explicación

**PASS_MAX_DAYS:** Define el número máximo de días que una contraseña puede utilizarse antes de requerir un cambio.

**PASS_MIN_DAYS:** Establece el número mínimo de días que deben transcurrir antes de que un usuario pueda cambiar nuevamente su contraseña.

**PASS_WARN_AGE:** Determina cuántos días antes del vencimiento de la contraseña el sistema comenzará a mostrar advertencias al usuario.

### Importancia

Estas políticas ayudan a fortalecer la seguridad del sistema al reducir el riesgo de uso prolongado de contraseñas comprometidas.

## Conclusión

La gestión adecuada de usuarios y las políticas de contraseñas constituyen una de las primeras barreras de protección en un sistema Linux.
