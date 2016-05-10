# c2000
Microcontrolador TMS320F28377S de Texas Instruments, en kit de desarrollo Launchxl-f28377s
Ejemplos de programación en Matlab2016a-simulink
1) test_led_azul.slx  prende y apaga el led azul (gpio13) del kit
2) test_serial.slx hace un loopback por puerto serie
3) test_adc.slx mide con un conversor ADC se mide temperatura con un LM35
4) test_adc_y_serial.slx Mide temperatura con un LM35 y la transmite por puerto serie

Notas de instalación: Además de Matlab y el paquete de soporte de los micros C2000 
(>>supportPackageInstaller), hay que tener instalado el compilador CodeComposer de 
TI y el PowerSuite que dan soporte a cada micro en particular (headers y configuración 
del debugger XDS100v2).
Desde la consola de Matlab >>checkEnvSetup('ccsv5','f28069','list')
Lista las opciones para el F377S y la versión 6 del CodeComposer (sic), y
 >>checkEnvSetup('ccsv5','f28069') 
permite definir los accesos (paths) al compilador y las herramientas.
La versión a usar de los headers (punto 5) es la 1.60.

Ultima actualización: 2016-may-10
