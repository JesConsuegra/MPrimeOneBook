# Electrónica: Conexión del fusor

Los dos cables rojos del fusor, van a la toma D10 de la RAMPs.
Es conveniente estañarlos y ponerles un trozo de termorretráctil para evitar que se despeluche el cable.

![](https://lh3.googleusercontent.com/awVYv2OTRDo2Xk_xEv4xMJHKy5nwy0OEE6XZ8GFYMD1Qvrqw6tJeu84lzSSQszxqLeJEsTqllQ=w1920-h1080-rw-no)

![](https://lh3.googleusercontent.com/Oze9xwC94r_z5lyQ5wsj20HAqw3c2FxlJwDwNqfLHJVA_uh5poKxJeMUSTzjh8I9xWYKNyTjbQ=w1920-h1080-rw-no)

Hay que conectar también el sensor de temperatura (termistor, dos cables finos blancos) del fusor.

El termistor del fusor se conecta a la entrada T0 de la RAMPs, en la zona dedicada a ello. Si hubiera una base de impresiòn caliente, el termistor de la cama caliente se conectaría al T1.
Los termistores no tienen polaridad, por lo que es indiferente el sentido en el que se coloquen.

![](https://lh3.googleusercontent.com/CfCAqhKsGLFpXs5lf8nafbPsOMisVM0HoxEoeUTe176B7yr-HdUBqSKoq898KwWG5HI-O-09Ow=w1920-h1080-rw-no)

Por último hay que conectar el ventilador del fusor y el ventilador de capa. El ventilador del fusor va conectado permanentemente a +12V, y el de capa va controlado por la RAMPS y se conecta al D9 en la RAMPS.
