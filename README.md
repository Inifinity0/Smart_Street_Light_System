# Smart_Street_Light_System
This system is designed to reduce the electricity consumption and increase efficiency of the lighting

 void setup()  
 {  
   Serial.begin(9600); // sensor buart rate  
   pinMode(8,INPUT);  // IR Sensor output pin connected  
   pinMode(9,INPUT);  // IR Sensor output pin connected  
   pinMode(10,INPUT);  // IR Sensor output pin connected  
   pinMode(11,INPUT);  // IR Sensor output pin connected  
   pinMode(12,INPUT);  // IR Sensor output pin connected  
   pinMode(13,INPUT);  // IR Sensor output pin connected
   pinMode(2,OUTPUT); // LED PIN  
   pinMode(3,OUTPUT); // LED PIN  
   pinMode(4,OUTPUT); // LED PIN 
   pinMode(5,OUTPUT); // LED PIN  
   pinMode(6,OUTPUT); // LED PIN  
   pinMode(7,OUTPUT); // LED PIN     
 }  
 void loop()   
 {  
   int s1 = digitalRead(8); // IR Sensor Sensor output pin connected  
   int s2 = digitalRead(9); // IR Sensor Sensor output pin connected  
   int s3 = digitalRead(10); // IR Sensor Sensor output pin connected  
   int s4 = digitalRead(11); // IR Sensor Sensor output pin connected  
   int s5 = digitalRead(12); // IR Sensor Sensor output pin connected  
   int s6 = digitalRead(13); // IR Sensor Sensor output pin connected     
   Serial.println(s1); // see the value in serial mpnitor in Arduino IDE  
   Serial.println(s2); // see the value in serial mpnitor in Arduino IDE  
   Serial.println(s3); // see the value in serial mpnitor in Arduino IDE  
   Serial.println(s4); // see the value in serial mpnitor in Arduino IDE  
   Serial.println(s5); // see the value in serial mpnitor in Arduino IDE  
   Serial.println(s6); // see the value in serial mpnitor in Arduino IDE   
   delay(20);  
  if(s1 == 0 )  
  {   
  digitalWrite(2,HIGH);// LED ON
   delay(20);  
  }  
  else  
  {  
   digitalWrite(2,LOW);  // LED OFF  
  }  
  if(s2 == 0 )  
  {  
   digitalWrite(3,HIGH);  // LED ON 
   analogWrite(3,255/5);
   delay(20);  
  }  
  else  
  {  
   digitalWrite(3,LOW);  // LED OFF 
  }  
  if(s3 == 0 )  
  {  
   digitalWrite(4,HIGH); // LED ON  
   delay(20);  
  }  
  else  
  {  
   digitalWrite(4,LOW); // LED OFF  
  
  }
  if(s4 == 0 )  
  {  
   digitalWrite(5,HIGH); // LED ON
   delay(20);  
  }  
  else  
  {  
   digitalWrite(5,LOW);  // LED OFF  
  }  
  if(s5 == 0 )  
  {  
   digitalWrite(6,HIGH); // LED ON
   delay(20);  
  }  
  else  
  {  
   digitalWrite(6,LOW);  // LED OFF  
  }  
  if(s6 == 0 )  
  {  
   digitalWrite(7,HIGH); // LED ON
   delay(20);  
  }  
  else  
  {  
   digitalWrite(7,LOW);  // LED OFF  
  } 
  }
