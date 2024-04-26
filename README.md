
# Checkpoint 2 Edge Computing & Computer Systems

Projeto desenvolvido para auxiliar os funcionario da Vinheria Agnello, a não perder o estoque de vinho com variações de temperatura, luminosidade ou umidade, projeto desenvolvido em um Arduino.


## Link do projeto no tinkercad
https://www.tinkercad.com/things/8wEWBZN2uqL-sensor-de-luz


## Como reproduzir

Após clicar em "Iniciar simulação", clique no fotorresistor (LDR) para alterar a exposição a luz. Caso o nível de luminosidade seja considerado alarmante para a integridade dos vinhos, o led amarelo acende e o buzzer toca durante 3 segundos, caso o nível luminosidade esteja muito elevado, o led veremelho acende e o buzzer toca até que a condição ideal seja atendida.

Observação: Alterando o nível da luz, o buzzer provavelmente será ativado em um volume elevado, então cuidado.


## Autores

- [Leonardo Taschin](https://www.github.com/leotaschin)
- [Gustavo Berlanga](https://github.com/berla1)
- [Vinicius Gardim](https://www.github.com/gardim1)
- [Camila Feitosa](https://github.com/camfeitosa)
- [Gabriel Matiolli](https://www.github.com/m4tiolli)
## Dependências

- Arduino Uno R3

- Leds vermelho, amarelo e verde

- Placa de Ensaio

- 4 Resistores de 1000 ohm

- Fotorresistor

- Buzzer Piezo

- Jumper Cables
## Demonstração

(Inserir foto do ThinkerCad)

## Lógica

Os vinhos agradecem lugares com penumbra, especialmente os brancos e espumantes, que sofrem mais com o contato com a luz. Em função disso, o sistema monitora a luminosidade do ambiente com LED’s da seguinte maneira:

Led verde: caso a luminosidade esteja baixa, em condição ideial, acende. Led amarelo: Em caso de alerta, onde a luminosidade não está ideal, acende e um buzzer soa durante 3 segundos, se a luminosidade permanecer em níveis de alerta o buzzer continuará soando. O led vermelho: se acende quando a luminosidade está excessivamente alta e o buzzer é ativo, que toca até que as condições ideias sejam reestabelecidas.


## Principais requisitos

- Enquanto o ambiente estiver escuro, o LED Verde deve ficar aceso.
- Enquanto o ambiente estiver a meia luz, o LED Amarelo deve ficar aceso com uma mensagem de "Ambiente a meia luz" deve ser mostrado no display LCD.
- Enquanto o ambiente estiver totalmente ilumindado, o LED Vermelho deve ficar aceso e a mensagem "Ambiente muito claro" deve ser mostrado no display LCD.
- Enquanto o ambiente estiver totalmente ilumindado, o Buzzer deve ficar ligado continuamente.
- Enquanto o ambiente estiver com uma temperatura entre 10ºC a 15ºC, o display LCD deve informar "Temperatura OK" e também mostrar o valor da temperatura.
- Enquanto o ambiente estiver com uma umidade entre 50% e 70%, o display deve informar "Umidade OK", e também mostrar o valor da umidade.
- Os valores representados no display devem ser a média de pelo menos 5 leituras dos sensores, e os valores devem ser apresentados a cada 5 segundos.
- Enquanto a temperatura estiver fora da faixa ideal, o LED Amarelo deve ficar aceso e o Buzzer deve ligar continuamente.
- Enquanto a temperatura estiver fora da faixa ideal, o display deve informar "Temperatura Alta", para valores acima de 15ºC e também mostrar a temperatura.
- Enquanto a temperatura estiver fora da faixa ideal, o display deve informar "Temperatura Baixa", para valores abaixo de 10ºC e também mostrar a temperatura.
- Enquanto a umidade estiver fora da faixa ideal, o LED Vermelho deve ficar aceso e o Buzzer deve ligar continuamente.
-Enquanto a umidade estiver fora da faixa ideal, o display deve informar "Umidade Alta" para valores acima de 70% e também mostrar  a umidade.
- Enquanto a umidade estiver fora da faixa ideal, o display deve informar "Umidade Baixa", para valores abaixo de 50%. 

