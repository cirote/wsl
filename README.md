# wsl
Guia para la instalacion de un aaPanel en WSL

## Instalación de WSL
En Windows buscar "Activar o desactivar las caractéristicas de windows" y activar "Hiper-V" y "Subsistema de windows para linux"

## Actualizar powershell
```
winget install --id Microsoft.Powershell --source winget
```

## Instalar linux
### Usando usando terminal de windows o porwershell listar las versiones instaladas y su estado
```
wsl -l -v
```

### Ver las versiones disponibles
```
wsl --list --online
```

### Instalar una versión
```
wsl --install -d <NombreDeLaDistribución>
```
Cuidado: Hay que desactivar el servidor de dns acrilyc ui antes de instalar. Caso contrario dará error https://github.com/microsoft/WSL/issues/4364
### Desinstalar una versión
```
wsl --unregister <NombreDeLaDistribución>
```

## Instalar aaPanel
### Ver https://www.aapanel.com/forum/ 

Descargar el archivo y copiar a la distribucion de linux usando el explorador de archivos de windowsen el directorio home
```
chmod +x nombre_del_archivo
```
Ejecutar el script de instalación
```
sudo ./nombre_del_archivo
```
Desactivar SSL
```
sudo bt 27
```
Cambiar puerto de escucha
```
sudo bt 8
```
Cambiar dirección
```
sudo bt 28
```
Cambiar usuario
```
sudo bt 6
```
Cambiar contraseña
```
sudo bt 5
```


