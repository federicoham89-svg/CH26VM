# CH26VM
creación y seguridad de mi primer laboratorio 

# instalación de una VM con Virtualbox Oracle.

## 
* **Hipervisor:** Oracle VM VirtualBox (Versión 7.0 o superior recomendado para Windows 11)
* **Sistema Operativo Huésped:** ISO Oficial de Windows 11 (Standard Home Edition)
* **Hardware asignado en VirtualBox:**
  * **Memoria RAM:** 4 GB o más
  * **Procesadores:** 2 vCPUs
  * **Disco Duro:** 64 GB (Almacenamiento dinámico VDI)
  * **Seguridad:** TPM 2.0 y EFI habilitados (Requisitos nativos de Windows 11)

---

## 🚀 Paso a Paso del Proceso

### 1. Descarga e Instalación del Entorno
* Descarga de los instaladores oficiales desde las páginas de Oracle y la ISO de Windows 11 desde el sitio de Microsoft.
* Instalación de VirtualBox en el sistema operativo anfitrión aceptando los controladores de red necesarios.

### 2. Creación de la Máquina Virtual
* Inicialización del asistente en VirtualBox mediante el botón **Nueva**.
* Asignación del nombre de la máquina y selección de la ruta de la ISO de Windows 11 cargada.
* Configuración de la sección de "Instalación desatendida" o marcado de la casilla para saltarla.
* Asignación de memoria RAM (mínimo 4GB), procesadores (mínimo 2 vCPUs) y habilitación del check de **EFI**.
* Creación de un disco duro virtual en formato VDI con almacenamiento reservado dinámicamente de 64 GB.

### 3. Configuración Inicial e Instalación de Windows 11
* Arranque de la máquina virtual por primera vez.
* Selección de idioma, formato de hora y teclado en la pantalla de bienvenida.
* Selección de la edición instalada: **Windows 11 Home**.
* Creación de la cuenta de usuario local y configuración inicial de las opciones de privacidad de Microsoft.

### 4. Optimización del Sistema (Guest Additions)
* Despliegue del menú superior de VirtualBox en **Dispositivos > Insertar imagen de CD de las "Guest Additions"**.
* Ejecución del instalador desde el explorador de archivos dentro de Windows 11.
* Reinicio de la máquina para habilitar características críticas:
  * Ajuste automático de resolución de pantalla.
  * Portapapeles compartido bidireccional.

### 5. Actualización del Sistema Operativo (Windows Update)
* Navegación a **Configuración > Windows Update**.
* Clic en el botón **Buscar actualizaciones**.
* Descarga e instalación de todos los parches de seguridad, controladores de sistema y actualizaciones acumulativas.
* Reinicios sucesivos del sistema virtual hasta obtener el mensaje oficial: *"Todo está actualizado"*.

---

## 🔒 Conclusión y Buenas Prácticas de Ciberseguridad
* **Aislamiento:** La máquina virtual funciona en un entorno controlado (Sandbox), ideal para realizar pruebas de seguridad sin poner en riesgo el sistema operativo principal.
* **Línea base segura:** El sistema operativo ha quedado completamente actualizado, mitigando vulnerabilidades conocidas antes de comenzar con auditorías o laboratorios prácticos en el curso.

---