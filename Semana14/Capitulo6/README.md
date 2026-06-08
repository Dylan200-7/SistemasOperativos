# Capítulo 6: Modelos Formales de Protección

## Actividad 1: Aplicación del Principio de Mínimo Privilegio

### Comandos Ejecutados

```bash
sudo useradd auditor

chmod 444 datos.txt

su auditor

echo "Prueba" >> datos.txt
```

### Resultado Obtenido

El usuario `auditor` no pudo modificar el archivo debido a que únicamente poseía permisos de lectura.

### Preguntas

**¿Se pudo modificar el archivo?**

No. El sistema negó la operación debido a la falta de permisos de escritura.

**¿Qué principio de seguridad se aplicó?**

Se aplicó el Principio de Mínimo Privilegio, el cual establece que un usuario debe poseer únicamente los permisos necesarios para realizar sus funciones.

---

## Actividad 2: Análisis de Privilegios

### Comando Ejecutado

```bash
ps -ef | grep root
```

### Procesos Analizados

#### 1. systemd

Es el proceso principal del sistema Linux. Se encarga de iniciar y administrar servicios durante el arranque.

#### 2. sshd

Servicio que permite conexiones remotas seguras mediante el protocolo SSH.

#### 3. cron

Servicio encargado de ejecutar tareas programadas automáticamente en horarios definidos.

### Importancia

Estos procesos requieren privilegios elevados para administrar recursos críticos del sistema.

### Conclusión

El Principio de Mínimo Privilegio reduce la superficie de ataque y limita el impacto de posibles incidentes de seguridad.
