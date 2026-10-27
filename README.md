1. Creación de la Máquina Virtual
Se creó una máquina virtual Windows 11 utilizando Oracle VirtualBox como plataforma de virtualización. La virtualización permite disponer de entornos aislados para pruebas y aprendizaje sin afectar al sistema operativo anfitrión.

2. Configuración de Red en Modo NAT
Se configuró el adaptador de red en modo NAT. Esta configuración permite el acceso a Internet desde la máquina virtual manteniendo el aislamiento respecto de la red local, reduciendo la superficie de exposición.

 <img width="1587" height="877" alt="Red NAT" src="https://github.com/user-attachments/assets/871e2acc-a047-4081-ace4-965c0149f963" />
 
 3. Instalación del Sistema Operativo
Se realizó la instalación de Windows 11 utilizando una imagen ISO oficial. Una vez completada la instalación se verificó el correcto inicio y funcionamiento del sistema operativo.

4. Configuración de Usuarios
Se configuró la cuenta LOCAL1 con privilegios administrativos para tareas de mantenimiento y configuración. Asimismo, se creó la cuenta Alumno2026 como usuario con privilegios limitados, aplicando el principio de mínimo privilegio.

 <img width="1007" height="837" alt="Local1 administrador" src="https://github.com/user-attachments/assets/fc871d1e-ddfc-45ac-ba9b-412ba038567f" />
 <img width="1008" height="842" alt="Alumno2026 local standar" src="https://github.com/user-attachments/assets/a5aa73ac-af72-4638-ba61-e77aac4d9e17" />
 
 . Actualización del Sistema Operativo
Se ejecutó Windows Update hasta alcanzar el estado “Todo está actualizado”. Esta acción permite incorporar correcciones de seguridad, mejoras de estabilidad y mitigación de vulnerabilidades conocidas.

 <img width="1003" height="771" alt="WU actualizado" src="https://github.com/user-attachments/assets/51945a59-7e06-4ea9-a21a-24a6ba76f73a" />
 
 6. Instalación de VirtualBox Guest Additions
Se instalaron las Oracle VirtualBox Guest Additions para mejorar la integración entre el sistema anfitrión y el sistema invitado. Entre los beneficios obtenidos se incluyen integración del ratón, resolución dinámica y mejor experiencia de usuario.
 
 7. Snapshot Hardening Inicial
Se creó una instantánea denominada Hardening Inicial para preservar un estado estable y seguro del entorno virtual, permitiendo una recuperación rápida ante incidencias o cambios no deseados.

 <img width="1579" height="881" alt="historial de snpashots co hardening inicial" src="https://github.com/user-attachments/assets/2716e9f1-7ded-4f7c-a1f2-fe7dc3b71be2" />
 
Conclusiones
Durante la práctica se implementó correctamente una máquina virtual Windows 11 utilizando Oracle VirtualBox. Se configuró la conectividad mediante NAT, se instalaron las actualizaciones de seguridad disponibles, se creó una cuenta administradora y una cuenta con privilegios limitados, se instalaron las Guest Additions y se generó una instantánea de recuperación denominada Hardening Inicial. Como resultado se obtuvo una máquina virtual estable, actualizada y preparada para futuras prácticas de ciberseguridad. Cabe destacar que la red se establecera como interna y solaente se modificará a NAT en casos requeridos para dichas practicas. Esto disminuye el riesgo de accesos indeseados o la creacion de puentes a la maquina real(host) que comprometan la integridad de mis activos primordiales.





