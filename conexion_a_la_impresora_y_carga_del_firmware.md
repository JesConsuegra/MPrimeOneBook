# Conexión a la impresora y carga del firmware

Teniendo el firmware configurado, ya estamos en condiciones de conectar la impresora para cargarlo y hacer las primeras pruebas.

Conectamos el cable USB al PC/Mac que estemos utilizando. Eso es suficiente para alimentar el Arduino que lleva la impresora para cargar el firmware.

Antes de poder cargar el firmware, tenemos que hacer una pequeña configuración en el Arduino IDE para indicarle qué procesador estamos usando y en que puerto está conectado. En la barra de menús, seleccionamos "Herramientas" y en el desplegable hay que modificar "Placa", "Procesador" y "Puerto".

![](2016-09-24 10_32_56-Program Manager.png)

Placa y Procesador, según se indica en la imagen anterior.

Puerto: se activa si el PC detecta un Arduino. Si está en gris  indica que el PC no reconoce ningún Arduino conectado.

Una vez modificado "Configuration.h" pulsamos el botón de carga y Arduino IDE compila Marlin y lo envía a la tarjeta. Esto completa la configuración del firmware y podemos proceder a efectuar los ajustes finos y empezar las pruebas.