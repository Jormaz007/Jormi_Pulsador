	Jormi_Pulsador.h
	Librería de manejo de pulsadores
	v0.2	20200906
	
	Version Pull Up - PU
			Pulsado = 0v
			GND > Pulsador > pinDigital > resistencia > 5V
	Version Pull Down - PD		
			Pulsado = 5v
			Pulsado = 5v
			GND > resistencia > pinDigital > Pulsador > 5V

	---------------------------------

Constructor
	int pin		pin conectado al pulsador
	bool tipo	pull up = true	/ pull down = false (habitual)
Jormi_Pulsador(byte pin, bool tipo);


Lee estado del pulsador
	version PullUp (pulsado == LOW)
	version PullDown (pulsado == HIGH)
	return
		true, pulsado
		false, no pulsado
bool estado();


Update en el loop
void update();

Información, Muestra en ventana de depuración info de las variables
void informacion();
