/*
  Proyecto: Blink configurable
  Descripción: Parpadeo de un LED en el GPIO 1
*/

const int LED_PIN = 1;

// Tiempos configurables (en milisegundos)
const int TIEMPO_ENCENDIDO = 1000;
const int TIEMPO_APAGADO = 500;

void setup() {
  pinMode(LED_PIN, OUTPUT);
}

void loop() {
  digitalWrite(LED_PIN, HIGH);
  delay(TIEMPO_ENCENDIDO);

  digitalWrite(LED_PIN, LOW);
  delay(TIEMPO_APAGADO);
}
