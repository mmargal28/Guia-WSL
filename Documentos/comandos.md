## Comandos básicos para WSL

### Instalación

```wsl --install```
```wsl --install <Distribution Name>```

### Lista las distribuciones disponibles en línea.

```wsl --list --online```


### Enumeración de las distribuciones instaladas

```wsl --list --verbose```

Lista las distribuciones instaladas y su estado. Otras opciones:

--running: Solo distribuciones en ejecución.
### Establecimiento de la versión de WSL

```wsl --set-version <distribution name> <versionNumber>```

Cambia la versión de WSL (1 o 2) de una distribución.

### Establecimiento de la versión de WSL predeterminada

```wsl --set-default-version <Version>```

Establece la versión predeterminada de WSL (1 o 2).

### Establecimiento de la distribución predeterminada

```wsl --set-default <Distribution Name>```

Establece la distribución de Linux predeterminada.

### Cambio al directorio principal

```wsl ~```

Inicia en el directorio principal del usuario.

### Ejecución de una distribución específica

```wsl --distribution <Distribution Name> --user <User Name>```

Ejecuta una distribución específica con un usuario específico.

### Actualización de WSL

```wsl --update```

Actualiza WSL a la versión más reciente.

### Comprobación del estado de WSL

```wsl --status```

Muestra información sobre la configuración de WSL.

### Comprobación de la versión de WSL

```wsl --version```

Muestra la versión de WSL y sus componentes.

### Comando de ayuda
```wsl --help```
Lista las opciones y comandos disponibles con WSL.

### Ejecutar como usuario específico
```wsl --user <Username>```
Ejecuta WSL como un usuario especificado.

### Cambio del usuario predeterminado

```<DistributionName> config --default-user <Username>```

Cambia el usuario predeterminado de una distribución.

### Apagar WSL

```wsl --shutdown```

Finaliza todas las distribuciones en ejecución y la máquina virtual de WSL 2.

### Terminar una distribución

wsl --terminate <Distribution Name>

Finaliza la distribución especificada.

### Identificar la dirección IP

Muestra la IP de la distribución de Linux instalada.

```wsl (hostname) -i```

Muestra la IP de la máquina Windows desde WSL 2.

```cat /etc/resolv.conf```


### Exportar una distribución

```wsl --export <Distribution Name> <FileName>```

Exporta una distribución como un archivo tar.

### Importar una distribución

```wsl --import <Distribution Name> <InstallLocation> <FileName>```

Importa un archivo tar como una nueva distribución.

### Importación en contexto

wsl --import-in-place <Distribution Name> <FileName>

Importa un archivo .vhdx como una nueva distribución.

### Anular el registro de una distribución

```wsl --unregister <DistributionName>```

Anula el registro de una distribución para su reinstalación o limpieza.

### Montar un disco o dispositivo

```wsl --mount <DiskPath>```

Monta un disco físico en todas las distribuciones de WSL 2.

Opciones:

--vhd: Especifica un disco duro virtual.
--name: Nombre personalizado para el punto de montaje.
--bare: Conecta el disco sin montarlo.
--type <Filesystem>: Tipo de sistema de archivos.
--partition <Partition Number>: Número de partición a montar.
--options <MountOptions>: Opciones específicas del sistema de archivos.

### Desmontar discos

```wsl --unmount <DiskPath>```

Desmonta un disco especificado. Si no se especifica, desmonta todos los discos montados.
