# Apuntes - Héctor Moreno

## Comandos Windows

### Eliminar una carpeta

`rmdir` -> Para eliminar una carpeta

`rmdir /s` -> para eliminar carpeta con contenido dentro

### Cambiar nombre a un archivo

`ren "archvio.txt" "nuevonombre.txt"`

### Listar todos los procesos activos

`tasklist`

### Para eliminar procesos

`taskkill`

`taskkill /f` -> para que no te pregunte si estás seguro de eliminar el proceso.

### Listar todos los servicios encendidos

`sc query`

### Ver contenido de un archivo

`type nombre_archivo.txt`

## Comandos de redes

### Mostrar la interfaz de red

`ipconfig`

`ipconfig /all` -> lo muestra todo más detallado.

### Comprobar la conectividad con otro equipo

`ping direccion_ip`

`ping nombre_de_dominio`

**Ejemplo**

`ping 192.168.1.20`

`ping www-jerez.es`

### Saber la dirección ip de un servidor de dominio

`nslookup nombre_de_dominio`

### Sitios por donde pasa la petición que se manda

`tracert www.jeres.es`

## Variables de entorno

`%USERNAME%` -> Usuario actual

`%COMPUTERNAME%` -> Nombre del equipo

`USERPROFILE` -> Carpeta personal

`%WINDIR%` -> Carpeta del sistema

`%PATH%` -> Ruta a los archivos ejecutables "importantes" a los que quiero acceder "rápidamente" desde la consola.

## Crear variables de entorno

### Para crear variables de entorno ponemos:

`set nombre=resultado`

**Ejemplo**

![alt text](image-1.png)

### Para eliminar la variable

`set nombre=`

### Listar todas las variables

`set`

**Ejemplo**

![alt text](image-2.png)

## Condicionales con IF-ELSE

Un condicional permite ejecutar unas instrucciones cuando se cumple una condición.

### Ejemplo de condicional

```
@echo off

echo Quieres continuar? (si/no)

set respuesta

if respuesta==si(
    echo Has elegido continuar
)
else(
    echo Has elegido no continuar
)
pause
```


