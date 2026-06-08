# Capítulo 4: Validación

## Actividad 1: Verificación de Integridad Mediante Hash

### Comandos Ejecutados

```bash
echo "Sistema Operativo" > archivo.txt
sha256sum archivo.txt

echo "Modificado" >> archivo.txt
sha256sum archivo.txt
```

### Resultado Obtenido

Se generó un hash SHA-256 del archivo original. Luego de modificar el contenido del archivo se volvió a generar el hash y se observó que el valor obtenido era diferente.

### Preguntas

**¿Cambió el hash?**

Sí. El hash cambió completamente después de modificar el archivo.

**¿Qué demuestra este resultado?**

Demuestra que los algoritmos hash son sensibles a cualquier modificación de los datos. Incluso un pequeño cambio en el archivo genera un valor hash totalmente diferente, permitiendo verificar la integridad de la información.

---

## Actividad 2: Validación de Usuarios

### Comandos Ejecutados

```bash
id
groups
```

### Resultado Obtenido

Se visualizó el identificador del usuario (UID), grupo principal (GID) y grupos secundarios a los que pertenece.

### Análisis

El comando `id` muestra la identidad completa del usuario actual, mientras que `groups` permite conocer todos los grupos asociados.

Ejemplo:

```text
uid=1000(usuario)
gid=1000(usuario)
groups=1000(usuario),27(sudo)
```

### Conclusión

La validación de usuarios permite verificar identidades y permisos dentro del sistema operativo.
