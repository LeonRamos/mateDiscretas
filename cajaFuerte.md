# Caja Fuerte

Este proyecto proporciona una plataforma interactiva y visual para que los estudiantes exploren los conceptos del álgebra booleana en un contexto práctico y relevante.

´´´
#include <LiquidCrystal.h>

// Pines para los pulsadores
const int buttonPins[4] = {2, 3, 4, 5};
// Pines para LEDs y buzzer
const int greenLedPin = 6;
const int redLedPin = 7;
const int buzzerPin = 8;
// Pines para LCD
LiquidCrystal lcd(12, 11, 10, 9, A0, A1);

// Variables para el estado de los botones
boolean buttonStates[4] = {false, false, false, false};

void setup() {
  // Configurar pines
  for (int i = 0; i < 4; i++) {
    pinMode(buttonPins[i], INPUT_PULLUP);
  }
  pinMode(greenLedPin, OUTPUT);
  pinMode(redLedPin, OUTPUT);
  pinMode(buzzerPin, OUTPUT);
  
  // Inicializar LCD
  lcd.begin(16, 2);
  lcd.print("Ingrese codigo:");
}

void loop() {
  // Leer estado de los botones
  for (int i = 0; i < 4; i++) {
    buttonStates[i] = !digitalRead(buttonPins[i]);
  }
  
  // Implementación de operaciones booleanas
  boolean andOperation = buttonStates[0] && buttonStates[1];
  boolean orOperation = buttonStates[2] || buttonStates[3];
  boolean xorOperation = buttonStates[0] ^ buttonStates[1];
  
  // Implementación de la ley de De Morgan
  boolean deMorganLaw = !(buttonStates[0] && buttonStates[1]) == (!buttonStates[0] || !buttonStates[1]);
  
  // Función booleana para el acceso (sin optimizar)
  boolean accessGranted = (buttonStates[0] && !buttonStates[1] && buttonStates[2] && !buttonStates[3]) ||
                          (!buttonStates[0] && buttonStates[1] && !buttonStates[2] && buttonStates[3]);
  
  // Función booleana optimizada (usando mapa de Karnaugh)
  boolean accessGrantedOptimized = (buttonStates[0] ^ buttonStates[1]) && (buttonStates[2] ^ buttonStates[3]);
  
  // Actualizar salidas
  digitalWrite(greenLedPin, accessGrantedOptimized);
  digitalWrite(redLedPin, !accessGrantedOptimized);
  
  // Actualizar LCD
  lcd.setCursor(0, 1);
  if (accessGrantedOptimized) {
    lcd.print("Acceso concedido");
    tone(buzzerPin, 1000, 100);
  } else {
    lcd.print("Acceso denegado ");
  }
  
  delay(100);
}
´´´

Este proyecto cubre los siguientes aspectos del álgebra booleana:

Fundamentos: Implementa operaciones AND, OR y XOR usando los estados de los botones.

Teoremas y postulados: Demuestra la ley de De Morgan.

Optimización de expresiones booleanas: Muestra una función de acceso sin optimizar y su versión optimizada.

Minitérminos: La función de acceso se basa en minitérminos específicos (combinaciones correctas).

Representación de circuitos lógicos: El sistema completo actúa como un circuito lógico combinacional.

Métodos de simplificación: La función optimizada simula el resultado de aplicar un mapa de Karnaugh.
