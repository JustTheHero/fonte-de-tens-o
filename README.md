# fonte-de-tensao


# Componentes:
---
| Quantidades   | Componentes   | Preço |
| ------------- |:-------------:| -----:|
| 1      | Capacitor (1000uF x 25V)      | R$1,40  |
| 1      | LED 5mm vermelho              | R$0,60  |
| 1      | Chave - 3 terminais           | R$1,10  |
| 1      | Ponte retificadora (2A)       | R$2,90  |
| 1      | Potenciômetro 5K - linear     | R$7,00  |
| 1      | Transistor 2N2222 (1A)        | R$1,00  |
| 1      | Diodo Zener 1N4743 (13V / 1W) | R$0,48  |
| 10     | Resistor 1K - (1/2W)          | R$0,70  |
| 10     | Resistor 4.7K - (1/2W)        | R$0,70  |
| 10     | Resistor 2.2K - (1/2W)        | R$0,70  |
|        | Total                         | R$16,58 |



# Explicação da função de cada componente: 
---
⋅⋅*Resistor: Os resistores limitam a corrente que passa pelo sistema, evitando que ela ultrapasse os valores limites de funcionamento dos outros componentes e os prejudique permanentemente.  

⋅⋅*Diodo Zenner: O diodo zenner é um componente fundamental do circuito. Ele funciona como um regulador de tensão máxima no sistema, permitindo a passagem de corrente somente quando a tensão for menor do que o seu valor nominal. Nesse caso, o diodo zenner só permite a passagem de corrente com tensões até 13V, limitando, dessa forma, a tensão resultante. 

⋅⋅*Capacitor: O capacitor também é outro componente de extrema importância. Ele é responsável por armazenar corrente durante a alternância dos ciclos de corrente e a libera quando a sua tensão interna é maior que a tensão do sistema. Desse modo, o capacitor controla o ripple (queda da tensão) do circuito. 

⋅⋅*Transformador: O transformador é responsável por reduzir os 127V fornecidos por uma tomada padrão de 110V para os 17V de alimentação do circuito, não interferindo na corrente. 

⋅⋅*Potenciômetro: O potenciômetro desse circuito é responsável por variar a resistência do sistema e, com isso, a tensão resultante do circuito no intervalo de 3 a 12V. 

⋅⋅*Transistor: O transistor nesse circuito atua de forma a permitir que a corrente passe pelo aparelho acoplado à fonte sem que ela passe pelo diodo zenner e o queime, dado que o mesmo suporta apenas correntes mínimas (nesse circuito, cerca de 10mA). Ele precisa de 0,7V para funcionar. 

⋅⋅*Ponte de diodo: A ponte de diodo permite que mesmo com a alteração do ciclo da corrente alternada, que se trata de uma senoide, o circuito continue recebendo corrente. Ela precisa de 1,4V para funcionar, acarretando uma queda de tensão de 24V(Vmax) para 22,6V. 
