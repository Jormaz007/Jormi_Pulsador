/*
	Jormi_Pulsador.h
	Librería de manejo de pulsadores
	v0.1	20200820
	v0.2	20200906
	
	Version Pull Up - PU
			Pulsado = 0v
			GND > Pulsador > pinDigital > resistencia > 5V
	Version Pull Down - PD		
			Pulsado = 5v
			Pulsado = 5v
			GND > resistencia > pinDigital > Pulsador > 5V
*/

/*	Constructor
	int pin
*/
Jormi_Pulsador(byte pin, bool tipo);


/*
	Estado
	Lee estado del pulsador
	
	version PullUp (pulsado == LOW)
	return
		true, pulsado
		false, no pulsado
		
	version PullDown (pulsado == HIGH)
	return
		true, pulsado
		false, no pulsado
*/
bool estado();


/*
	Update
*/
void update();


/*
	Información
	Muestra en ventana de depuración info de las variables
*/
void informacion();



};
