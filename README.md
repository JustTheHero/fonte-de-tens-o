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
* Resistor: Os resistores limitam a corrente que passa pelo sistema, evitando que ela ultrapasse os valores limites de funcionamento dos outros componentes e os prejudique permanentemente.  

* Diodo Zenner: O diodo zenner é um componente fundamental do circuito. Ele funciona como um regulador de tensão máxima no sistema, permitindo a passagem de corrente somente quando a tensão for menor do que o seu valor nominal. Nesse caso, o diodo zenner só permite a passagem de corrente com tensões até 13V, limitando, dessa forma, a tensão resultante. 

* Capacitor: O capacitor também é outro componente de extrema importância. Ele é responsável por armazenar corrente durante a alternância dos ciclos de corrente e a libera quando a sua tensão interna é maior que a tensão do sistema. Desse modo, o capacitor controla o ripple (queda da tensão) do circuito. 

* Transformador: O transformador é responsável por reduzir os 127V fornecidos por uma tomada padrão de 110V para os 17V de alimentação do circuito, não interferindo na corrente. 

* Potenciômetro: O potenciômetro desse circuito é responsável por variar a resistência do sistema e, com isso, a tensão resultante do circuito no intervalo de 3 a 12V. 

* Transistor: O transistor nesse circuito atua de forma a permitir que a corrente passe pelo aparelho acoplado à fonte sem que ela passe pelo diodo zenner e o queime, dado que o mesmo suporta apenas correntes mínimas (nesse circuito, cerca de 10mA). Ele precisa de 0,7V para funcionar. 

* Ponte de diodo: A ponte de diodo permite que mesmo com a alteração do ciclo da corrente alternada, que se trata de uma senoide, o circuito continue recebendo corrente. Ela precisa de 1,4V para funcionar, acarretando uma queda de tensão de 24V(Vmax) para 22,6V. 

# Circuito no Falstad:
---

![imagem_2023-07-03_201700964](https://github.com/JustTheHero/fonte-de-tensao/assets/114316462/3dfda506-8051-4b8c-b7dd-0cc1cde6453f)
Link do circuito [aqui](https://www.falstad.com/circuit/circuitjs.html?ctz=CQAgjCAMB0l3BWEB2WZIICxgEwGZMA2QgDmRMJEwE4QlM86BTAWjDACgBnEHHTECUgg8CHIOGSQAMwCGAGy5MOAN179whYXwF4cUiFvBCopmAg4B3dbv28SJEXchX7jvcNHiPUDgRAAJgCWAPYBTAC2YUzypmDQDvBJyZB4rI4wkDgUvFRwvgF02RIghAiUJuLB0VHh8hyFZZQ+Yu524mAAcphwmA2l5U7CrSUd3b39Iz5No4FMcgCu8gAuHAAqecImU85UUNBgeHgUiSTlyFp4yEgs5oQ4yNTU7EdPOM+0bNBihKKiYMhILgENQEKxkPsntQOGB7ihSCULo4cIMqvNZEtlix5ExChApJlOAAneHIwZIoamTCAlzWHSjDSwySuLyUnqeZyuGYmQjIcQmWkDZp2UhtZnWXn84SikouADGpQcJRlPkksCB6mgr0g1EwQj4qSy+zgnGsJD0lKEHOZAHNFWL7SIxGZXNRigDKG7kZAMjDkAIvbwfSBA-xhBAEPBIaCUikIAAlJhcIJcZayAB2cuUJNDPRDxTwkAE2n0gsDhYDBc51nLdgotnFIcwAnp1AuNl8yxD7dbbo74ZAbBI0EIuvI1DIoLw1AwSBgvJIOFIcCuWWnE-A+XCixWrr7+kcbxDlBcOf3eaPqvA+j33jstcbR5MR+oJ9c5rvW0IDd8Nfd7cDMBm18fwAC8mHTJgiTYPAWHEcNoGQICvBIMAvXQOAcHBUwOkYThQMEb9LSIj1cnAyDoMOOD33yEx61ld8iOfPsBVdd1gPooDi0YgRSM44DT0IgQ6JIgTNzgFlnRMdkGIAD0EQYETIcQkL2Q4QHjTh5NHXiZxQGhwGoRheMYABhWQAAdZDlIJlhCIkOHkttvGOTd3hEbA1MYeMLKJIJMyCKz6ic-x9HECckH0ehBBAAAFEJlggmyABeIiYZYiRCRzBELXgwEcEhQXUCBeOEAARAAdLgAC0IIoqqYIANWy65aCORxkGuDySvAbycGyt1PGnEM8GaTBxBMjS8AGp51CQdBUWKSa1iJDNk1TezXApHwrUpQVtpFJVVS5JUTApVjrHOrZaOZeSsAhAhDH8AgBEm+L00Sqrwi+0IAiy+SHmlXRIAhXkvJAUyAAtZBUZQAaIXhPNeRHXt6kAADEQg+pgvpx1MIK4ABj-68ghf06D1FAIWW1b0y4aR7IiWQ-qJKrcGQBqAWakJeFB4s8lm5xoHg3IHhEDgeYtIjhB6QW1SyebcgtaagA)

# Circuito no Eagle:
---
![WhatsApp Image 2023-07-04 at 20 24 59](https://github.com/JustTheHero/fonte-de-tensao/assets/114316462/f704cd7e-6f38-4732-9db9-a02e829140e8)




# Cálculos:
---
* Capacitância: Ripple = Vs / f x C x R 

* Vs = Vpico = 17. √2 = 24V  

* F = 60x2 = 120Hz 

* Requivalentemax = 22,6V / 40mA = 565 Ω 
* Ripple: (Vmax – Vponte diodo) - (Vmin)  =  (24 – 1,4) - 21,6 = 0,7 

* 0,7 = 24/120xCx565 == 500uF 
 
* Diodo Zenner: 12V de saida + 0,7V do transistor + coeficiente de erro = 13V

# Vídeo no YouTube:
---
[link](https://www.youtube.com/watch?v=ehXos4eMNOw&pp=ygUrdW0gZXhwZXJpbWVudG8gcXVlIGRldSBjZXJ0bywgbyBsZWQgYWNlbmRldQ%3D%3D)





# Projeto-Arduino:

# Introdução:
O projeto é sobre um dispositivo que detecta a presença de água no sensor e com esse sinal recolhe a estrutura do varal para um local protegido, evitando assim que as roupas tomem chuva.


# Código fonte:
---
![WhatsApp Image 2023-07-05 at 11 28 33](https://github.com/JustTheHero/fonte-de-tensao/assets/114316462/402d12a5-f2c1-4d6a-9ada-916b67569630)


# Vídeo no YouTube:
---
[link](https://youtu.be/J3WtUEaTZNA)





# Participantes:
---
#### Juan Marques Jordão (hero)

#### Augusto Cavalcante Barbosa Pereira (lixeira)

#### Gabriel Hyppolito (gabirula)

#### Vinicius Gustierrez Neves (vicininho)
