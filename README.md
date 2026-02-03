# Tarea-1-Entorno-de-Virtualizacion-e-Infraestructura-Base
Entorno de Virtualización e Infraestructura Base
Objetivo:
El estudiante montará un entorno de red virtualizado compuesto por tres nodos funcionales, garantizando la comunicación interna, el aislamiento de red y la preparación de los sistemas operativos para la automatización.
Requerimientos Técnicos:Hipervisor: VirtualBox o VMware.Nodo 1 (Servidor Linux): Ubuntu Server (22.04 LTS o superior) o alguna otra distribución asignada. Sin entorno gráfico (CLI).Nodo 2 (Servidor Windows): Windows Server (2019 o 2022). Instalación "Desktop Experience" permitida, pero se evaluará el uso de PowerShell.Nodo 3 (Cliente): Windows 10/11 o Linux Desktop (Para pruebas de conectividad).Configuración de Red:
  Adaptador 1: NAT (Para salida a internet y descarga de paquetes).
  Adaptador 2: Red Interna (Nombre: red_sistemas). Aquí se asignarán las IPs estáticas más adelante.
Actividades a Realizar:
  Instalación: Configurar nombres de host (hostname) descriptivos (ej. Srv-Linux-Sistemas, Srv-Win-Sistemas).Actualización: Ejecutar comandos de actualización inicial en ambos    
  SO.Snapshots: Crear un "Estado Base" (Instantánea) de las máquinas recién instaladas.Prueba de Conectividad: Realizar un ping entre las tres máquinas usando las IPs de la Red
  Interna.Script de Bienvenida: Crear un script simple (check_status.sh / check_status.ps1) que al ejecutarse muestre: Nombre del equipo, IP actual y espacio en disco.

Entregables:Carpeta de Scripts: tarea1_diagnostico.sh y tarea1_diagnostico.ps1.Documento PDF:
  Tabla de direccionamiento IP propuesto.
  Captura de pantalla del comando ping exitoso entre los 3 nodos.
  Captura de los "Snapshots" creados en el hipervisor.
Enlace al repositorio de GitHub: Con el primer commit inicial.
La evaluación de esta primera actividad se regirá bajo criterios estrictos de funcionalidad y orden técnico. 
Se otorgará el 40% de la nota a la configuración de red, donde es indispensable que los tres nodos mantengan comunicación bidireccional mediante ping a través de una red interna aislada, sin perder el acceso a internet para la gestión de repositorios. 
Un 20% corresponderá a la optimización de recursos, valorando positivamente el uso de versiones de servidor sin interfaz gráfica en Linux y el ajuste correcto de hardware virtual para evitar el desbordamiento de la memoria física. 
Otro 20% se asignará a la calidad de los scripts de diagnóstico inicial, los cuales deben demostrar una lógica clara, sin errores de sintaxis y una salida de datos organizada en consola. 
Finalmente, el 20% restante evaluará la documentación técnica y el uso de Git, exigiendo un registro histórico de comandos coherente, capturas de pantalla que validen los snapshots de respaldo y un repositorio estructurado profesionalmente desde el primer día.
