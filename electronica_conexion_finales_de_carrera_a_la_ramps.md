# Electrónica: Conexión finales de carrera y sensor inductivo a la RAMPS

Los conectores para los finales de carrera se encuentran en la parte inferior de la RAMPS (si la hemos montado con el botón de RESET hacia arriba).

Hay que conectar el final de carrera X al X-Max, el final de carrera Y al Y-Min y el sensor inductivo al Z-Min, según se indica en la foto.


![](https://lh3.googleusercontent.com/XrKql9-AAaqQObxrnBrpXzRFdoZs9uST8JmdOffrN7v4JtTNWl6IeMPV2NjdOQsUX-8oqkGipg=w1920-h1080-rw-no)

El sensor inductivo que utilicé yo es el PNP que funciona a 12Volt, con tres cables: +12V, masa y señal. (En la actualidad el sensor inductivo que viene con la M'One funciona a +5Volt y se puede conectar directamente a la RAMPS respetando las polaridades).

Para los sensores inductivos de 12V hay que colocar un diodo para evitar que los 12V del sensor dañen la electrónica de la RAMPS y hay que llevar el cable de alimentación a un pin de la RAMPs que suministra esos 12V.

El esquema lo teneis en [la web de la M'One](http://mprime.io/es/question/conexion-inductivo/), pero como es habitual lo incluyo aquí: 

![](http://mprime.io/wp-content/uploads/2015/09/Selection_003-141x300.png)
Así es como lo he puesto yo:

El diodo (he usado un pequeño diodo de señal 1N4148), hay que soldarlo al terminal negro del sensor inductivo, con el cátodo hacia el sensor (rayita negra en el cuerpo del diodo). Los otros dos cables, el azul es masa y el marrón es +12v.

Le he añadido un pequeño conector (de recuperación) para conectar a la RAMPs en los contactos correspondientes al final de carrera Zmin.

Y todas las soldaduras recubiertas con termorretráctil para evitar cruces y para hacer el conjunto mas resistente.

![](https://lh3.googleusercontent.com/MyiuX0yXlUf4ao82L7919I6C6MR7VxqKijs6fZ0rVm2rhQ_RaXMfyfW8CG4c2gP89h-772z0Rw=w1920-h1080-rw-no)

![](https://lh3.googleusercontent.com/iN3gBVRK_okOiIZnOIWh84CYONt-RVJ4aj-jj4AqallgDDymOdjPRQ6hJJMu9CvbR2elnkLKKQ=w1920-h1080-rw-no)

El cable que nos quedaba suelto proveniente del sensor inductivo lo tenemos que llevar a la RAMPs y conectarlo a +12V.

Justo delante del conector de alimentación, hay una ubicación para conectar un ventilador para la propia RAMPs. En la RAMPs que tengo para hacer pruebas no viene conectorizado por lo que  hay que soldarle un par de pines.

![](https://lh3.googleusercontent.com/zYF5IyRwmG1PR7psYIkwjdNcLVb0fhKc9rAPByxDh1B7fv_BNxXExp4m3NswcNMFq0DOLKUZgA=w1920-h1080-rw-no)

![](https://lh3.googleusercontent.com/oYH8152PT1MCNrm6QJSZzqcoQfqKa3CdKu5kHd1MPg9RNpmYeDpUvaLONcTCTJeOqzZhggiCIA=w1920-h1080-rw-no)

![](https://lh3.googleusercontent.com/0hc9Bg-OawAuy-rqcOzgoNJURkoaipvypKFY6bGabs_9S41mEvBxwafDq5p9eIbvjylvz96q0A=w1920-h1080-rw-no)

![](https://lh3.googleusercontent.com/N5WP5Y0eM6ShIblWrob3pmbZ5Zw6HdDSs7XFsucSQbPys4LsxDtaf5PeztzwBB8wp9IzAUJ0SQ=w1920-h1080-rw-no)

![](https://lh3.googleusercontent.com/eHBp8isJf6fbUz0ejjp1EfCEO7IDzpwDY4s9YzLRWNWzX33L5ovN2F3h-ljTITnFQxtEaeglbA=w1920-h1080-rw-no)

![](https://lh3.googleusercontent.com/9msN2M5zrGxPjQvGmknKWaqLp3ct0hPJLx0ZtvjI1akNIrbNUXJeDdCjZbcPxYMDacKE6e1zMA=w1920-h1080-rw-no)

![](https://lh3.googleusercontent.com/J9wbBCxolpDmE0jusOKPgboIFB6sRzxcZsQ3LD6NfR2YCk-ZigYUedQSucHe2jBOhOtAv_Evbg=w1920-h1080-rw-no)

![](https://lh3.googleusercontent.com/_9T8Mb2rpyO8viczkZGnAyChZfe6Dyqe20me7Xlkgoe2SLS0GDO5_9jZ13TKUH_xxT8_nAOkNw=w1920-h1080-rw-no)

![](https://lh3.googleusercontent.com/TnABQ6J239Zk3S5Yxezp2n_RQOK053hDZS0uckAsyyuZMtABTYXfXRDfBHraLfPwYDQy3PqyjQ=w1920-h1080-rw-no)
