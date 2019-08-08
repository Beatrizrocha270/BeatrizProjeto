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

# Observações 
1) O programa executa uma única vez as funções "setup" e "pinMode", que fazem a configuração inicial do ARDUINO. Depois disso, o programa executa um número indeterminado de vezes o "loop" entre os colchetes, até que o programa seja desligado ou reconfigurado. 
2) Para que o programa funcione de maneira mais eficiente, faça uma medição dos tempos em segundos para os "delay"'s. Por exemplo, verifique se o valor de delay(5000) corresponde de fato a 5,0 segundos.
3) Observe que o tempo de funcionamento do led amarelo é menor que dos outros o que de fato ocorre em um semáforo real.
