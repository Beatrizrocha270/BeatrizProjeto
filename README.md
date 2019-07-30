# Semáforo com 3 leds 
Com auxilio da placa ARDUINO UNO, simular o semáforo de trânsito com 3 leds. 
# Materiais Necessários 
- 01 Placa ARDUINO UNO.
- 03 Leds nas cores vermelho, amarelo e verde.
- 01 Resistor de 1K ohm. 
- Jumpers. 
# Procedimento 
- Monte o circuito conforme a figura anexada, denominada 'Figura1'.
-Na interface de programação de Sketches do Arduino, insira e compile o programa abaixo com a placa conectada ao seu computador através da porta USB. 
# Código 

// PROGRAMA SEMAFORO COM 3 LEDS 

void setup()

{ 

pinMode(13,OUTPUT);  // DEFINE O PINO 13 COMO OUTPUT, OU SEJA, UMA SAÍDA.  
pinMode(12,OUTPUT);  // DEFINE O PINO 12 COMO OUTPUT, OU SEJA, UMA SAÍDA.  
pinMode(11,OUTPUT);  // DEFINE O PINO 11 COMO OUTPUT, OU SEJA, UMA SAÍDA.

} 

void loop()  

{

digitalWrite(13,HIGH);  // COLOCA O PINO 13 EM NÍVEL "ALTO", OU SEJA, EM 5 V; O LED VERMELHO ACENDE.   
delay(5000);                   // TEMPO DE ESPERA DE 5 SEGUNDOS.   
digitalWrite(13,LOW);  // COLOCA O PINO 13 EM NÍVEL "BAIXO", OU SEJA, EM 0 V; O LED VERMELHO APAGA. 

digitalWrite(11,HIGH);  // COLOCA O PINO 11 EM NÍVEL "ALTO", OU SEJA, EM 5 V; O LED VERDE ACENDE.   
delay(5000);                   // TEMPO DE ESPERA DE 5 SEGUNDOS.    
digitalWrite(11,LOW);  // COLOCA O PINO 11 EM NÍVEL "BAIXO", OU SEJA, EM 0 V; O LED VERDE APAGA.  

digitalWrite(12,HIGH);  // COLOCA O PINO 12 EM NÍVEL "ALTO", OU SEJA, EM 5 V; O LED AMARELO ACENDE.   
delay(2000);                   // TEMPO DE ESPERA DE 2 SEGUNDOS.  
digitalWrite(12,LOW);  // COLOCA O PINO 12 EM NÍVEL "BAIXO", OU SEJA, 0 V; O LED AMARELO APAGA.  

} 
# Observações 
1) O programa executa uma única vez as funções "setup" e "pinMode", que fazem a configuração inicial do ARDUINO. Depois disso, o programa executa um número indeterminado de vezes o "loop" entre os colchetes, até que o programa seja desligado ou reconfigurado. 
2) Para que o programa funcione de maneira mais eficiente, faça uma medição dos tempos em segundos para os "delay"'s. Por exemplo, verifique se o valor de delay(5000) corresponde de fato a 5,0 segundos.
3) Observe que o tempo de funcionamento do led amarelo é menor que dos outros o que de fato ocorre em um semáforo real.
