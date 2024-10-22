// C++ code
//
void setup()
{
  pinMode(10, OUTPUT);
  pinMode(8, OUTPUT);
  pinMode(9, OUTPUT);
  pinMode(2, OUTPUT);
  pinMode(3, OUTPUT);
  pinMode(4, OUTPUT);
}
void loop()
{
   //semaforo 1
  digitalWrite(10, HIGH);//ligar o led vermelho do semaforo 1
  //semaforo 2
  digitalWrite(4, LOW);//desligar o vermelho
  digitalWrite(2, HIGH);//ligar o verde do semaforo 2
  ////////////////////////////////////
  delay(2000); // Wait for 2000 millisecond(s)
  ///////////////////////////////////
  //semaforo 1
  
  //semaforo 2
  digitalWrite(2, LOW); // desliga o led verde
  digitalWrite(3, HIGH);//liga o led amarelo
  delay(1000); // Wait for 2000 millisecond(s)
  //sEMAFORO 1
  digitalWrite(10, LOW);//DESLIGA O VERMELHO
  digitalWrite(8, HIGH);//LIGA O VERDE
  //semaforo 2
  digitalWrite(4, HIGH);
  digitalWrite(3, LOW);//liga o led amarelo
  
  delay(2000); // Wait for 1000 millisecond(s)
  //SEMAFORO 1
  digitalWrite(8, LOW); //DESLIGA O VERDE
  digitalWrite(9, HIGH);// LIGA O AMARELO
  delay(1000);
  digitalWrite(9, LOW);//desliga o amarelo
}
