int minutes = 5;  // Exemple : 5 minutes
int secondes;

void setup() {
  Serial.begin(9600);  // Initialisation de la communication série
}

void loop() {
  secondes = minutes * 60;  // Conversion des minutes en secondes
  Serial.print(minutes);
  Serial.print(" minutes correspondent à ");
  Serial.print(secondes);
  Serial.println(" secondes.");
  
  delay(1000); // Attente de 1 seconde avant la prochaine exécution
}
