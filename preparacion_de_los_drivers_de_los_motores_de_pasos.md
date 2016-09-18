# Preparación de los drivers de los motores de pasos (POLOLU)

Un punto importante es ajustar el límite de corriente de los drivers de los motores de pasos ( Pololus A4988) a las especificaciones del motor.

Para ello necesitamos conocer las características del motor. En mi caso los motores son LDO-42STH47-1684A.  En la wiki de RepRap tienen una buena lista de motores, este incluído. 

Las características de estos motores son:
Bobinas de 2.8mH, cuyo máximo a 2.8volts son 1,68A y pueden ejercer una fuerza de 50 N/cm.

![](https://lh3.googleusercontent.com/qr4t-L3AWtl8G_hmP9-kXqJKfQMWhdqTP8Oa5_8hupCPA4Be2AA8sIU95Xg1wSP19MOeyCEf3Q=w1920-h1080-rw-no)

Con esos datos nos vamos a la web de Pololu. Hay un excelente vídeo que explica como ajustar los Pololus. Con un montaje supersimple (un puente entre los pines 5 y 6 y alimentación entre los pines 9 (masa) y 10 (+5v). 

El vídeo lo teneis aqui: [](https://youtu.be/89BHS9hfSUk)

Pololu indica que el límite en Ampéres es igual a la mitad de la tensión de referencia. Como estos motores tienen un máximo de 1,68A  hemos de ajustar a 1,68/2 = 0,84Volt, entre el cursor del potenciómetro y masa.

![](https://lh3.googleusercontent.com/XTFNK3M4FGyngFdwKZ8Om9xFXkI5M2AK5_oRgX0AgBvIMADgMwSWUzcjlaW_72Uzb7wwWMN_jw=w1920-h1080-rw-no)

Procedemos con los cuatro Pololus.
![](https://lh3.googleusercontent.com/qTjQybk1dDO1Nm8Tb4jGq746WLkbPeck6mLu7OlxGuC7ykmX4XOZ72xc1jdYvHSzUUEtDkZNlA=w1920-h1080-rw-no)

 El siguiente paso será probar los motores uno a uno y el sentido de giro. Para ello he puesto la alimentación de los motores entre los pines 16 y 15 del Pololu (12v) y una tira de 4 pines para poder enchufar los motores con facilidad.
 
Después del ajuste de los Pololus A4988 y antes de colocarlos en la impresora, hay que  proceder a probarlos con los motores.
Para ello, el sencillo esquema que viene en la web de Pololu conectado a un Arduino, la patilla 7 del Pololu (step) al D3 del Arduino y la 8 (dir) al D4 del Arduino, 

![](https://a.pololu-files.com/picture/0J3360.600.png?d94ef1356fab28463db67ff0619afadf)

y este simple sketch de un colega de Mechatronics.

/*     Simple Stepper Motor Control Exaple Code
 *      
 *  by Dejan Nedelkovski, www.HowToMechatronics.com
 *  
 */
// defines pins numbers
const int stepPin = 3; 
const int dirPin = 4; 
 
void setup() {
  // Sets the two pins as Outputs
  pinMode(stepPin,OUTPUT); 
  pinMode(dirPin,OUTPUT);
}
void loop() {
  digitalWrite(dirPin,HIGH); // Enables the motor to move in a particular direction
  // Makes 200 pulses for making one full cycle rotation
  for(int x = 0; x < 200; x++) {
    digitalWrite(stepPin,HIGH); 
    delayMicroseconds(500); 
    digitalWrite(stepPin,LOW); 
    delayMicroseconds(500); 
  }
  delay(1000); // One second delay
  
  digitalWrite(dirPin,LOW); //Changes the rotations direction
  // Makes 400 pulses for making two full cycle rotation
  for(int x = 0; x < 400; x++) {
    digitalWrite(stepPin,HIGH);
    delayMicroseconds(500);
    digitalWrite(stepPin,LOW);
    delayMicroseconds(500);
  }
  delay(1000);
}


Un corto video del motor del extrusor moviéndose: [](https://youtu.be/0IE1dXPrINE)