# c2000
Ejemplos de programación en Matlab2016a-Simulink del microcontrolador TMS320F28377S de Texas Instruments, en kit de desarrollo Launchxl-f28377s (http://www.ti.com/tool/launchxl-f28377s).

1) test_led_azul.slx    Prende y apaga el led azul (gpio13) del kit

2) test_serial.slx    Hace un loopback por puerto serie

3) test_adc_y_serial.slx    Mide temperatura con un LM35 y la transmite por puerto serie

Notas de instalación: 
Además de Matlab 2016a y el paquete de soporte de los micros C2000 
(Mtlb>>supportPackageInstaller), hay que tener instalado el compilador Code Composer de 
TI (http://www.ti.com/tool/ccstudio-c2000) y el PowerSuite (http://www.ti.com/tool/powersuite) que da soporte a cada micro en particular (headers y configuración del debugger XDS100v2).

Desde la consola de Matlab >>checkEnvSetup('ccsv5','f28069','list')
Lista las opciones para el F377S y la versión 6 del CodeComposer (sic), y
Mtlb>>checkEnvSetup('ccsv5','f28069') 
permite definir los accesos (paths) al compilador y las herramientas.
La versión a usar de los headers (punto 5) es la 1.60.

Ultima actualización: 2016-sep-07
