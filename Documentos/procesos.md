# Procesos WSL

## WSL 1
WSL 1 es la primera versión de WSL y actúa como una capa de compatibilidad que traduce las llamadas del sistema Linux a llamadas del sistema Windows. No incluye un núcleo de Linux completo.

### Procesos y Componentes de WSL 1:

**wsl.exe:** El ejecutable principal que se utiliza para iniciar y gestionar las distribuciones de WSL.

**lxssmanager.dll:** El servicio de administración de WSL, encargado de iniciar y detener las distribuciones.

**LxssManager Service:** Un servicio en Windows que se encarga de gestionar las instancias de WSL.

**Distribuciones de Linux:** Estos son los entornos de Linux que se instalan desde la Microsoft Store (por ejemplo, Ubuntu, Debian, etc.). Se ejecutan dentro de un contenedor de WSL.

## WSL 2
WSL 2 introduce un cambio significativo al usar una máquina virtual liviana basada en un kernel de Linux real. Esto proporciona una mayor compatibilidad y rendimiento en comparación con WSL 1.

### Procesos y Componentes de WSL 2:

**wsl.exe:** Igual que en WSL 1, este es el comando principal para gestionar las distribuciones de WSL.

**vmmem:** Proceso de administración de memoria virtual que representa la memoria utilizada por la máquina virtual de WSL 2.

**Virtual Machine Platform:** Una característica opcional de Windows que proporciona los servicios de máquina virtual necesarios para WSL 2.

**wsl2_vm:** La máquina virtual que aloja el kernel de Linux y las distribuciones de Linux.

**Kernel de Linux:** Un kernel de Linux real que se ejecuta dentro de la máquina virtual de WSL 2, lo que proporciona una mayor compatibilidad con las aplicaciones de Linux.
