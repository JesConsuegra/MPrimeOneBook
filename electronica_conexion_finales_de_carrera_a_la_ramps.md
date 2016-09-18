# Electrónica: Conexión finales de carrera y sensor inductivo a la RAMPS

Los conectores para los finales de carrera se encuentran en la parte inferior de la RAMPS (si la hemos montado con el botón de RESET hacia arriba).

Hay que conectar el final de carrera X al X-Max, el final de carrera Y al Y-Min y el sensor inductivo al Z-Min, según se indica en la foto.


![](https://lh3.googleusercontent.com/XrKql9-AAaqQObxrnBrpXzRFdoZs9uST8JmdOffrN7v4JtTNWl6IeMPV2NjdOQsUX-8oqkGipg=w1920-h1080-rw-no)

El sensor inductivo que utilicé yo es el PNP que funciona a 12Volt, con tres cables: +12V, masa y señal. (En la actualidad el sensor inductivo que viene con la M'One funciona a +5Volt y se puede conectar directamente a la RAMPS respetando las polaridades).

Para los sensores inductivos de 12V hay que colocar un diodo para evitar que los 12V del sensor dañen la electrónica de la RAMPS y hay que llevar el cable de alimentación a un pin de la RAMPs que suministra esos 12V.

El esquema lo teneis en [la web de la M'One](http://mprime.io/es/question/conexion-inductivo/), pero como es habitual lo incluyo aquí: 

![](http://mprime.io/wp-content/uploads/2015/09/Selection_003-141x300.png)
Así es como lo he puesto yo:

El diodo, hay que soldarlo al terminal negro del sensor inductivo, con el cátodo hacia el sensor (rayita negra en el cuerpo del diodo). Los otros dos cables, el azul es masa y el marrón es +12v.

Le he añadido un pequeño conector (de recuperación) para conectar a la RAMPs en los contactos correspondientes al final de carrera Zmin.

Y todas las soldaduras recubiertas con termorretráctil para evitar cruces y para hacer el conjunto mas resistente.

![](https://lh3.googleusercontent.com/MyiuX0yXlUf4ao82L7919I6C6MR7VxqKijs6fZ0rVm2rhQ_RaXMfyfW8CG4c2gP89h-772z0Rw=w1920-h1080-rw-no)

![](https://lh3.googleusercontent.com/iN3gBVRK_okOiIZnOIWh84CYONt-RVJ4aj-jj4AqallgDDymOdjPRQ6hJJMu9CvbR2elnkLKKQ=w1920-h1080-rw-no)
