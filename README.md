# scripts-utiles-bash
En este repositorio hay disponibles algunos scripts que facilitan el uso de la terminal de comandos.
Están escritos en Bash y hacen uso de comandos externos. 
A continuación se explica el funcionamiento de los scripts y se listan la/s dependencias requeridas.

## Descripción de los scripts y paquetes requeridos
### apaga-gpu
Apaga la GPU NVIDIA del sistema (si la hubiera) descargando previamente del kernel los módulos necesarios para compilar en CUDA.
De esta manera es posible apagar la GPU sin ningún problema después de acabar la compilación.
De otro modo, (comprobado en una GeForce 610M) es posible que la GPU permanezca encendida y consumiendo energía.

*Es necesario tener una tarjeta gráfica NVIDIA instalada junto a su gestor de energía Optimus para Linux (Bumblebee).*

### batt-level
Consulta el nivel de batería del equipo portátil, mostrando las estimaciones de porcentaje restante y tiempo restante.

*Es necesario disponer del comando **"acpi"**.*

*En sistemas operativos basados en **Arch** o **Ubuntu** se encuentra en el paquete **"acpi"**.* 

### gpu-status
Consulta el estado de la GPU NVIDIA (ON y OFF).

*Es necesario tener instalado el gestor de energía Optimus para Linux (bumblebee).*

### temp-cpu
Consulta la temperatura de los cores de la CPU.
La temperatura para cada core se indica con tres colores distintos dependiendo de si es "Fría" (temp < 35ºC), "Normal" (35ºC <= temp <= 60ºC)) o "Caliente" (temp > 60ºC).

*Es necesario disponer del comando **"sensors"**.*

*En sistemas operativos basados en **Arch** este comando se encuentra en el paquete **"i2c-tools"**.*

*En sistemas operativos basados en **Ubuntu** se localiza en el paquete "lm-sensors".*
