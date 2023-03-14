# Blink
Arduino 아두이노 실습
tinkercad


// C++ code
//
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(LED_BUILTIN, OUTPUT);
}

int x=1000; //전역변수를 써야함 
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);  // turn the LED on (HIGH is the voltage level)
  delay(x);                      // wait for a second
  digitalWrite(LED_BUILTIN, LOW);   // turn the LED off by making the voltage LOW
  delay(x);  
  x*=0.9;
  if(x<=10){
    x=1000;
  }
}
