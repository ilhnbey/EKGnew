void setup() {
  Serial.begin (9600);
  pinMode(10,INPUT); // Pin L0 +
  pinMode(11,INPUT); // Pin L0 - 
  
  }
  
  void loop() {
  
    if((digitalRead(10) == 1) || (digitalRead(11) == 1)){
      Serial.println('!');
    }
    else{
        Serial.println(analogRead(A0));
    {
    delay(1);
    }
