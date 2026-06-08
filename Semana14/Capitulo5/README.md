# Capítulo 5: Protección y Control de Acceso

## Actividad 1: Gestión de Grupos

### Comandos Ejecutados

```bash
sudo groupadd seguridad
sudo usermod -aG seguridad estudiante1
groups estudiante1
```

### Resultado Obtenido

El usuario `estudiante1` fue agregado correctamente al grupo `seguridad`.

### Pregunta

**¿Qué ventajas ofrece el control por grupos?**

El control por grupos permite administrar permisos de manera más eficiente. En lugar de asignar permisos usuario por usuario, se asignan a un grupo completo, simplificando la administración y mejorando la seguridad.

---

## Actividad 2: Uso de ACL

### Comandos Ejecutados

```bash
sudo apt install acl

touch informe.txt

setfacl -m u:estudiante1:rwx informe.txt

getfacl informe.txt
```

### Resultado Obtenido

Se otorgaron permisos de lectura, escritura y ejecución al usuario `estudiante1` sobre el archivo `informe.txt` mediante ACL.

### Ejemplo de Salida

```text
# file: informe.txt
# owner: usuario
# group: usuario

user::rw-
user:estudiante1:rwx
group::r--
mask::rwx
other::r--
```

### Análisis

Las ACL permiten definir permisos más específicos que los permisos tradicionales de Linux, ofreciendo mayor flexibilidad en el control de acceso.

### Conclusión

Las ACL mejoran significativamente la administración de permisos y la protección de recursos críticos.
