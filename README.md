# Smartest
======================================================
Smartest v6.3  (Agosto, 2015)

______________________
Documentación
======================
 
 Este LEEME sirve para la configuración y uso de Smartest

______________________
Notas del Lanzamiento
======================

 Solo soporte para discos SATA.[#1](/eReuse/Smartest/issues/1)
 
_____________________
Instalación
======================

 Mover los siguientes archivos en "/usr/share/smartest/*".

   - smartest
                |- bin
                |    |- smartest
                |- etc
                     |- menu_ca.properties
                     |- menu_en.properties
                     |- menu_es.properties

 Smartest depende de `smartmontools`:
 
	En ubuntu:
		`sudo apt-get install smartmontools`

______________________
Uso de la aplicación
======================

 Para arrancar la aplicación se debe ejecutar el fichero `smartest` situado en el
 directorio bin de la instalación.

 El programa leerá las opciones del archivo **config.ini**, según la configuración:
 
*  Y = Preguntará al técnico que opción desea realizar.
*  1 = hará un chequeo rápido del disco duro primario.
*  2 = Hará un chequeo extendido del disco duro primario.
*  N = No se ejecutará.

 (El proceso de *DeviceInventory* esperará si el chequeo aún no ha finalizado)

 Una vez finalizado guardará la información en `/usr/share/donator/etc/data.ini`
 donde el programa `donator` importará el resultado del chequeo.
 
______________________
Soporte
======================

 Cualquier problema con esta versión puede ser reportado en la siguiente
 dirección de correo electrónico:
 adrias@ereuse.org
