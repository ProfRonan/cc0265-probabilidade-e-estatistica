# Probabilidade Condicional

As vezes, probabilidades podem ser reavaliadas quando informações adicionais são obtidas.

As vezes, queremos calcular probabilidade assumindo que algumas coisas vão, ou não vão, acontecer.

## Motivação

A probabilidade de infartar sendo jovem atlético é baixa, cerca de 0.001 (Fonte: imaginação).

A probabilidade de um eletrocardiograma dar um falso positivo (detectar um infarto quando na realidade o paciente está saudável) é de 0.01 (Fonte: a mesma anterior).

A probabilidade de um eletrocardiograma dar um falso negativo (não detectar um infarto quando você está de fato infartando) também é de 0.01 (Fonte: Comics Sans).

Você recebeu o resultado do exame e é **POSITIVO**, desespero!? É pra se preocupar ou não!?

Calma, vamos tentar de novo depois de estudar mais probabilidade condicional.

## Definição: Probabilidade Condicional

Definimos a probabilidade de $B$ dado $A$ como sendo

$$P(B \mid A) = \frac{P(A \cap B)}{P(A)}$$

Em outras palavras, a probabilidade condicional de $B$ dado $A$ é a probabilidade de $B$ acontecer sabendo ou assumindo que $A$ aconteceu.

### Continuando a Motivação

Vamos começar falando do espaço amostral...
Ele é composto por todos os jovens atléticos com infarto ou sem, apesar de ser muito complicado descrever ele explicitamente, ou até mesmo implicitamente, não precisamos dessa descrição minuciosa, a princípio, para trabalhar com os eventos e probabilidades deles.

Vamos dar nome para os eventos de interesse:

- $I$ o evento que um jovem atlético infarta.
- $P$ o evento em que o exame dá positivo.
- $I \cap P$ é o evento em que um jovem atlético infarta e o exame dá positivo.
- $I \cap P'$ é o evento em que um jovem atlético **infarta** e o exame dá **negativo**.
- $I' \cap P$ é o evento em que um jovem atlético **não infarta** e o exame dá **positivo**.
- $I' \cap P'$ é o evento em que um jovem atlético não infarta e o exame dá negativo.

Sabemos as probabilidades de:

- $P(I) = 0.001$ Jovem infartou
- $P(I') = 0.999$ Jovem não infartou ($P(A') = 1 - P(A)$)
- $P(P \mid I') = 0.01$ (Falso positivo)
- $P(P' \mid I) = 0.01$ (Falso negativo)

Também sabemos que o evento $P$ aconteceu!

O que queremos mesmo é saber a probabilidade de ter o infarto sabendo que o exame deu positivo que denotamos por $P(I \mid P)$.

Ainda não temos ferramentas suficientes para resolver isso...

## Exercício Probabilidade Condicional

Um equipamento produz peças de automóvel.
Pegamos um lote dessa máquina para fazer uma análise minuciosa.
São 400 peças ao total.
Dentre essas 400 peças, temos 360 sem defeitos visíveis e 40 com defeitos visíveis.
Dentre essas 400 peças, temos 28 que não funcionam e 372 que funcionam.

Dispondo todas essas categorias em uma tabela ficamos com

| Funciona  | Defeito | Sem Defeito | **Total** |
| --------- | ------- | ----------- | --------- |
| Sim       | 10      | 18          | 28        |
| Não       | 30      | 342         | 372       |
| **Total** | 40      | 360         | 400       |

Seja o experimento aleatório em que selecionamos aleatoriamente uma peça do lote de maneira uniforme.

Seja $F$ o evento em que a peça funciona e $D$ o evento em que ela apresenta defeitos visíveis.

Para evitar jogar peças que funcionam fora e como analisar minuciosamente todas elas é impraticável...
Vamos tentar responder quantas peças boas vão ser jogadas fora se simplesmente olharmos os defeitos superficiais.
E também quantas peças ruins vamos deixar passar se só jogarmos fora as com defeitos superficiais.

Queremos calcular:

- $P(F \mid D)$ (Probabilidade da peça funcionar, sabendo que ela tem defeito superficial)
- $P(F' \mid D')$ (Probabilidade da peça não funcionar, sabendo que ela parece perfeita)

Pela regra da probabilidade condicional

$$P(F \mid D) = \frac{P(D \cap F)}{P(D)}$$

Sabemos que $P(D \cap F) = 10 / 400$ que é a chance de obter uma peça funcionando com defeito visível dentre todas as peças do lote.

Sabemos que $P(D) = 40 / 400$ que é a chance de obter uma peça funcionando com defeito visível dentre todas as peças do lote.

Logo,

$$P(F \mid D) = \frac{P(D \cap F)}{P(D)} = \frac{10/400}{40/400} = \frac{10}{40} = 0.25$$

Baseado nessa análise, _"poderíamos"_ concluir que se fossemos jogar fora toda peça com defeito visível _uma delas em cada 4_ ainda funcionaria...

Fazendo a análise da outra parte temos

$$P(F' \mid D') = \frac{P(D' \cap F')}{P(D')} = \frac{342/400}{360/400} = \frac{342}{360} = 0.05$$

Jogando todas as peças com defeitos visíveis fora, estaríamos colocando em funcionamento _"apenas"_ 5% de peças com defeito.
