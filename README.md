# led-on-off-using-push-button
const int buttonPin = 4;     
const int ledPin =  12;      
int buttonState = 0;        

void setup() {
 
  pinMode(ledPin, OUTPUT);
  
  pinMode(buttonPin, INPUT);
}

void loop() {
  
  buttonState = digitalRead(buttonPin);

  if (buttonState == HIGH) {
    digitalWrite(ledPin, HIGH);
  } else {
    digitalWrite(ledPin, LOW);
  }
}
