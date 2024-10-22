void setup()
{
  pinMode(10, OUTPUT);
  pinMode(8, OUTPUT);
  pinMode(9, OUTPUT);
  
  pinMode(7, OUTPUT);
  pinMode(6, OUTPUT);
  pinMode(5, OUTPUT);
}

void loop()
{
 digitalWrite(10, HIGH);//semafóro 1 vermelho LIG
  delay(0000);
  // Primeiro a ligar sem nenhum delay
  // Depois disso junto com o vermelho vai precisar ligar o VERD
  
  
 digitalWrite(5, HIGH);//Semafóro 2 Verd LIG
  delay(5000);
  //Semafóro verde vai desligar depois de 5 segundos
  // depois disso vai passar a acender o amarelo
  
  
 digitalWrite(6, HIGH);//semafóro 2 Amarelo LIG
  delay(2000);
  //
 digitalWrite(5, LOW);//semafóro 2 Verd DESL
  delay(2000);
  //
 digitalWrite(10, LOW);//semafóro 2 Vermelho DESL
  delay(0000);
  //
 digitalWrite(6, LOW);//semafóro 2 Amarelo DESL
  delay(2000); 
  //
 digitalWrite(7, HIGH);//semafóro 2 Vermelho LIG
  delay(2000);
  //
 digitalWrite(8, HIGH);//semafóro 1 Verde LIG
  delay(2000);
  //
 digitalWrite(7, LOW);//semafóro 2 Vermelho DESL
  delay(2000);
  //
 digitalWrite(8, LOW);//semafóro 1 Verde DESL
  delay(2000);
  //
 digitalWrite(9, HIGH);//semafóro 1 AMA LIG
  delay(2000);
  //
 digitalWrite(9, LOW);//semafóro 1 Amarelo DSL
  delay(2000);
  
}
