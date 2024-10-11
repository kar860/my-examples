int i;
int red = 12;
int blue = 13;
int green = 14;
void setup() {
  pinMode(2, OUTPUT);
  pinMode(red, OUTPUT);
}
void loop() {

  for (i = 0; i < 255; i++) {
    analogWrite(red, i);
    delay(4);
  }

   analogWrite(red, 0);
  
  
  for (i = 0; i < 255; i++) {
    analogWrite(blue, i);
    delay(4);
  }
 analogWrite(blue, 0);
  
  for (i = 0; i < 255; i++) {
    analogWrite(green, i);
    delay(4);

  }
  analogWrite(green, 0);
}

