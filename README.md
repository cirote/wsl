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
