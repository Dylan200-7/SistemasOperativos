\# Semana 14 - Seguridad en Sistemas Operativos Linux



\## Descripción



En esta semana se desarrolló una práctica de laboratorio enfocada en la implementación de mecanismos de seguridad en sistemas operativos Linux. Se realizaron actividades relacionadas con la gestión de usuarios, políticas de contraseñas, validación de integridad, control de acceso, aplicación del principio de mínimo privilegio y administración segura de evidencias mediante Git y GitHub.



\## Integrantes



\* Mathias Dylan Henry Quispe Charres

\* Josue Cristhian Mateo Mogollon Flores

\* Kevin Esty Carvallo Neciosup



\## Objetivos



\* Comprender los mecanismos básicos de seguridad en Linux.

\* Gestionar usuarios y grupos de forma segura.

\* Aplicar políticas de contraseñas.

\* Validar la integridad de archivos utilizando funciones hash.

\* Configurar permisos mediante ACL.

\* Aplicar el principio de mínimo privilegio.

\* Gestionar evidencias utilizando Git y GitHub.



\---



\## Actividades Realizadas



\### Capítulo 3: Políticas y Mecanismos de Seguridad



\#### Creación de Usuarios



Se creó el usuario `estudiante1` y se verificó su registro dentro del sistema mediante la consulta del archivo `/etc/passwd`.



\#### Configuración de Políticas de Contraseña



Se analizaron los parámetros:



\* PASS\_MAX\_DAYS

\* PASS\_MIN\_DAYS

\* PASS\_WARN\_AGE



Estos parámetros permiten controlar la vigencia, renovación y advertencias relacionadas con las contraseñas de los usuarios.



\---



\### Capítulo 4: Validación



\#### Verificación de Integridad Mediante Hash



Se utilizó el algoritmo SHA-256 para generar un hash de un archivo de prueba.



Posteriormente, se modificó el contenido del archivo y se generó nuevamente el hash, observándose que el valor cambió completamente.



Esto demuestra que cualquier modificación en un archivo altera su huella digital y permite verificar su integridad.



\#### Validación de Usuarios



Se emplearon los comandos:



```bash

id

groups

```



para identificar el usuario actual y los grupos a los que pertenece.



\---



\### Capítulo 5: Protección y Control de Acceso



\#### Gestión de Grupos



Se creó el grupo `seguridad` y se agregó el usuario `estudiante1` a dicho grupo.



Esta práctica permitió comprender la administración centralizada de permisos mediante grupos.



\#### Uso de ACL



Se instalaron y configuraron listas de control de acceso (ACL) para asignar permisos específicos sobre archivos.



Las ACL permiten una gestión más flexible que los permisos tradicionales de Linux.



\---



\### Capítulo 6: Modelos Formales de Protección



\#### Principio de Mínimo Privilegio



Se creó un usuario con permisos limitados y se comprobó que no podía modificar archivos protegidos.



Esto permitió aplicar el principio de mínimo privilegio, reduciendo riesgos de seguridad.



\#### Análisis de Privilegios



Se identificaron procesos ejecutados con privilegios elevados, entre ellos:



\* systemd

\* sshd

\* cron



Estos servicios son fundamentales para el funcionamiento y administración del sistema.



\---



\## Gestión Segura con Git y GitHub



Durante la práctica también se realizaron actividades relacionadas con el control de versiones y protección de evidencias:



\* Configuración de Git.

\* Creación de repositorio privado.

\* Organización de evidencias por semanas.

\* Uso de archivo `.gitignore`.

\* Gestión de commits.

\* Publicación segura en GitHub.



\---



\## Evidencias



Los resultados de esta práctica se encuentran documentados en el archivo:



\*\*SISTEMAS\_OPERATIVOS\_SEMANA\_14.pdf\*\*



\---



\## Conclusiones



1\. Linux proporciona herramientas robustas para la administración de la seguridad.

2\. La gestión adecuada de usuarios y grupos mejora el control de acceso.

3\. Los algoritmos hash permiten verificar la integridad de los archivos.

4\. Las ACL proporcionan un mecanismo flexible para asignar permisos.

5\. El principio de mínimo privilegio reduce la superficie de ataque.

6\. Git y GitHub permiten mantener evidencias organizadas y seguras mediante control de versiones.



