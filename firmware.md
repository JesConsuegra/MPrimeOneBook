# Firmware: Instalación de Arduino


Para poder realizar las primeras pruebas hay que configurar el firmware y cargarlo en la impresora. Si estás montando la M'Prime One estándar, puedes bajarte una versión del Firmware (Marlin) ya configurada desde el GitHub de la M'One:

  [Marlin](https://github.com/M-Prime/M_Prime_One/tree/master/firmware/Marlin)
  
Pero en mi caso no puedo usar directamente ese firmware porque mi extrusor lleva un impulsor MK7, de diámetro diferente al estándar.

En cualquier caso, hay que cargar el Marlin en la impresora y para eso hace falta instalar Arduino en un PC o un Mac. Arduino en los PC está soportado tanto bajo Linux como bajo Windows e incluso hay algún clone que funciona en tablets bajo Android. Yo prefiero usar el software original bajo Linux o Windows (uso normalmente Linux, una distro basada en Debian que se llama "BunsenLab Hydrogen"). La instalación tanto bajo Linux como bajo Windows es muy sencilla. Arduino instala también los drivers USB para la conexión con la impresora, con lo que al final del proceso de instalación deberíamos tener conexión con la impresora.

Arduino se puede bajar de su web, la versión en el momento de escribir este tutorial es la 1.6.11:

  [Arduino](https://www.arduino.cc/en/Main/Software)
  
 El modelo de Arduino que lleva la impresora es el **2560 R3**. 