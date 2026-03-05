# Trabajo practico 0

## Actividad 2

### Objetivo

En este laboratorio, revisará las habilidades básicas de Linux, incluidas la navegación por comandos, la administración de archivos, las expresiones regulares y la administración del sistema.

#### Parte 1: Revisar exploración de sintaxis de comandos

![alt text](img/1.png)

![alt text](img/2.png)

![alt text](img/3.png)

![alt text](img/4.png)

#### Parte 2:

![alt text](img/5.png)

##### Preguntas:

- ¿Qué representa el guion inicial en la información de permisos?¿Qué representa el guion inicial en la información de permisos?

Este es el campo de tipo de archivo. El guion representa un archivo normal.

- ¿Qué habría en el lugar del guion si el elemento fuera un directorio?

Sería una "d" para "directorio".

- ¿Qué representan las tres letras o guiones siguientes en la información de permisos?

Estos representan los permisos del propietario del archivo sobre el archivo.

- ¿Qué representan las tres letras intermedias o guiones en la información de permisos?

Estos representan los permisos del grupo sobre el archivo.

- ¿Qué representan las tres últimas letras o guiones en la información de permisos?

Estos representan los permisos que otros usuarios tienen sobre el archivo.

- ¿Qué indica la primera instancia de "devasc" en la información de permiso?

Esto indica el usuario propietario del campo y que es el propietario del archivo.

- ¿Qué indica la segunda instancia de "devasc" en la información de permiso?

Esto indica el campo propietario del grupo y es el grupo del archivo.

- ¿Qué significa un tipo de permiso de "r"?

Esto significa un permiso de "leer". Esto permite leer o copiar el contenido del archivo.

- ¿Qué significa un tipo de permiso de "w"?

Esto significa un permiso de "escribir". Esto permite modificar o sobrescribir el contenido.
Permite agregar o eliminar archivos de un directorio.

- ¿Qué significa un tipo de permiso de "x"?

Esto significa un permiso de "ejecutar". Esto permite que un archivo se ejecute como un proceso,
aunque los archivos de script también requieren permiso de lectura.

![alt text](img/6.png)

#### Parte 3

![alt text](img/7.png)
![alt text](img/8.png)

#### Parte 4

![alt text](img/9.png)

![alt text](img/10.png)

![alt text](img/11.png)

##### Preguntas:
- ¿Cuál es el número mínimo de días que deben pasar antes de que se pueda cambiar la contraseña?

0

- ¿Cuál es el número de días después de la expiración de la contraseña que la cuenta permanece activa?

-1 indica que la contraseña nunca caduca debido a la inactividad.

#### Agregado por mi: Diferencia entre programas externos y builtin

Cuando se ejecuta un comando, la shell crea un proceso hijo para correrlo (si, un comando generalmente no es mas que un programa). Ese proceso hijo tiene su propio entorno, incluyendo su propio directorio de trabajo actual (dado que es un procesos separado del padre).

Con algunos comandos como `pwd` por ejemplo, eso no es problema: simplemente lee el directorio actual y lo imprime. No necesita modificar nada en el proceso padre.
Con `cd`, sí es un problema: si `cd` fuera un proceso hijo externo, cambiaría el directorio de ese proceso hijo, y cuando ese proceso terminara, el shell padre seguiría en el directorio original. Dado que el hijo no tiene forma (simple) de cambiar el directorio actual del padre, el comando es construido dentro del shell y su código ejecutable esta dentro del proceso shell.

Por eso cd debe ser un builtin: necesita modificar el estado interno del shell que lo invoca, no de un proceso hijo.

Builtins: `cd`, `export`, `exit`, `source`, `.`, `alias`, `unset`, `set`, `read`, `history`, `jobs`, `fg`, `bg`, `type`, `true`, `false`, `test`, `[`
Externos: `ls`, `cat`, `grep`, `find`, `sed`, `awk`, `cut`, `sort`, `wc`, `head`, `tail`, `cp`, `mv`, `rm`, `mkdir`, `chmod`, `chown`, `ps`, `top`, `htop`, `man`, `curl`, `wget`, `ssh`, `tar`, `date`, `whoami`, `grep`

## Actividad 3

### Objetivo

#### Creación y actualización de repositorios

##### 

(En mi caso ya usaba git desde antes, por lo tanto ya lo tenia configurado)

![alt text](img/12.png)

##### Ejercicio 1

![alt text](img/13.png)

##### Ejercicios 2-6

![alt text](img/14.png)

![alt text](img/15.png)

![alt text](img/16.png)

#### Historial de cambios

##### Ejercicio 1
![alt text](img/17.png)

![alt text](img/18.png)

##### Ejercicios 2-4

![alt text](img/19.png)

![alt text](img/20.png)

#### Deshacer cambios

##### Ejercicio 1

![alt text](img/21.png)

##### Ejercicio 2

![alt text](img/22.png)

##### Ejercicio 3

![alt text](img/23.png)

##### Ejercicio 4

![alt text](img/26.png)

Historial después de realizar el commit

![alt text](img/24.png)

Historial luego de deshacer el commit

![alt text](img/25.png)

#### Ramas

##### Ejercicio 1

![alt text](img/27.png)

![alt text](img/28.png)

##### Ejercicio 2

![alt text](img/29.png)

![alt text](img/30.png)

##### Ejercicios 3-4

![alt text](img/31.png)

![alt text](img/32.png)

##### Ejercicio 5

![alt text](img/33.png)

![alt text](img/34.png)

#### Repositorios remotos

##### Ejercicios 1-2

![alt text](img/36.png)

![alt text](img/35.png)

##### Ejercicio 4

![alt text](img/37.png)

![alt text](img/38.png)

![alt text](img/39.png)