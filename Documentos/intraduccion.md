# ¿Qué es Windows Subsystem for Linux (WSL)?

El **Subsistema de Windows para Linux (WSL)** es una característica de Microsoft Windows que permite a los usuarios ejecutar un entorno GNU/Linux directamente en Windows, sin la necesidad de una máquina virtual o un arranque dual. Esta característica es especialmente útil para desarrolladores y administradores de sistemas que trabajan en entornos mixtos de Windows y Linux, ya que les permite ejecutar herramientas y aplicaciones de Linux junto con aplicaciones de Windows.

## Características principales de WSL

1. **Compatibilidad con binarios de Linux**:
   - WSL permite ejecutar binarios de Linux de forma nativa en Windows. Esto significa que puedes usar herramientas de línea de comandos de Linux, como `bash`, `grep`, `sed`, `awk`, y más, directamente en tu sistema Windows.

2. **Interoperabilidad**:
   - WSL permite compartir archivos y datos entre el entorno de Linux y Windows. Puedes acceder a los archivos del sistema de Windows desde Linux y viceversa.

3. **Facilidad de instalación**:
   - WSL se puede habilitar fácilmente desde la configuración de Windows o mediante PowerShell. Además, las distribuciones de Linux se pueden descargar e instalar directamente desde la Microsoft Store.

4. **WSL 1 y WSL 2**:
   - WSL tiene dos versiones principales:
     - **WSL 1**: Utiliza una capa de compatibilidad que traduce las llamadas del sistema Linux a llamadas del sistema Windows esto grata al subsistema gran velocidad con el resto de archivos del sistema ya que trabaja con ntfs.
     - **WSL 2**: Utiliza una máquina virtual liviana con un núcleo completo de Linux, lo que mejora significativamente el rendimiento y la compatibilidad con aplicaciones de Linux pero no trabaja bien con el sistema ntfs por que funciona con ext4.

![tabla](/img/tabla.png)

## Beneficios de usar WSL

- **Desarrollo en entornos mixtos**:
  - Facilita el desarrollo de aplicaciones que se ejecutan en Linux mientras se utiliza un entorno de desarrollo en Windows.
  
- **Reducción de la sobrecarga**:
  - A diferencia de las máquinas virtuales tradicionales, WSL consume menos recursos y se inicia mucho más rápido.
  

