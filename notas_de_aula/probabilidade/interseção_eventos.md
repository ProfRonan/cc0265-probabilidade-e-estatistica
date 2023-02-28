# Interseção de Eventos, Multiplicação e Regra da Probabilidade Total

## Regra da multiplicação

A regra da multiplicação é uma reescrita da equação que define a probabilidade condicional colocando a _interseção_ em evidência.

$$P(A \cap B) = P(B \mid A) P(A)  = P(A \mid B) P(B)$$

### Exemplo

Dado um baralho com 52 cartas, sendo 26 cartas vermelhas e 26 cartas pretas.
Retire aleatoriamente duas cartas do baralho, sem reposição.
Qual é a probabilidade de que a primeira carta retirada seja vermelha e a segunda carta também seja vermelha?

Podemos definir os eventos A e B da seguinte forma:

- $A$: a primeira carta retirada é vermelha;
- $B$: a segunda carta retirada é vermelha.

Precisamos calcular: $P(A \cap B) = P(A) \times P(B|A)$

- $P(A \cap B)$ é a probabilidade de que ocorram os eventos A e B simultaneamente;
- $P(A)$ é a probabilidade do evento A ocorrer;
- $P(B \mid A)$ é a probabilidade do evento B ocorrer dado que o evento A já ocorreu.

Então, a probabilidade de que a primeira carta retirada seja vermelha é de 26/52 = 1/2.

Em seguida, a probabilidade de que a segunda carta retirada seja vermelha, dado que a primeira carta retirada é vermelha, é de 25/51.
Assim, podemos calcular a probabilidade de que as duas cartas retiradas sejam vermelhas usando a regra da multiplicação:

$$
\begin{align*}
P(A \cap B) &= P(A) \times P(B \mid A)\\
P(A \cap B) &= (1/2) \times (25/51)\\
P(A \cap B) &= 25/102
\end{align*}
$$

Portanto, a probabilidade de que a primeira carta retirada seja vermelha e a segunda carta também seja vermelha é de aproximadamente 0,245 ou 24,5%.

## Regra da Probabilidade Total

A regra da probabilidade total é usada para calcular a probabilidade de um evento C a partir das probabilidades de outros dois eventos A e B, que [particionam](https://pt.wikipedia.org/wiki/Parti%C3%A7%C3%A3o_de_um_conjunto) o espaço amostral.

A fórmula para calcular a probabilidade de C usando a regra da probabilidade total é:

$$P(C) = P(A) \times P(C \mid A) + P(B) \times P(C \mid B)$$

Como $A$ e $A'$ sempre particionam o espaço amostral:

$$P(C) = P(A) \times P(C \mid A) + P(A') \times P(C \mid A')$$

### Exemplo

Suponha que um laboratório realize um teste $A$ para detectar uma doença.

- A sensibilidade do teste A é de 80%, o que significa que, se uma pessoa tem a doença, há uma probabilidade de 80% do teste A dar positivo.
- A especificidade do teste A é de 90%, o que significa que, se uma pessoa não tem a doença, há uma probabilidade de 90% do teste A dar negativo.

Suponha que a doença tenha uma prevalência de 5% na população.

Se uma pessoa faz o teste A e o resultado é positivo, qual é a probabilidade de que ela tenha a doença?

Vamos definir os eventos:

- $D$: a pessoa tem a doença
- $D'$: a pessoa não tem a doença
- $A$: o teste A é positivo
- $A'$: o teste A é negativo

$$P(D \mid A) = P(A) \times P(D \mid A) + P(A') \times P(D \mid A')$$

Das informações dadas podemos concluir:

- $P(A \mid D) = 0,8$ (sensibilidade do teste A)
- $P(A' \mid D') = 0,9$ (especificidade do teste A)
- $P(D) = 0,05$ (prevalência da doença)
- $P(D') = 0,95$ (complemento da prevalência da doença)

Substituindo esses valores na fórmula, temos:

$P(A) = 0,8 \times 0,05 + 0,1 \times 0,95 = 0,13$

$P(D \mid A) = (0,8 \times 0,05) / 0,13 = 0,31$

Portanto, se o resultado do teste A é positivo, a probabilidade de que a pessoa tenha a doença é de 31%.

## Independência (Interseção)

Dois eventos são considerados **independentes** se a ocorrência de um evento não afeta a probabilidade de ocorrência do outro evento.

Ou seja

$$
\begin{align*}
P(A \mid B) &= P(A)\\
&\text{ou}\\
P(B \mid A) &= P(B)\\
&\text{ou}\\
P(A \cap B) &= P(A) \times P(B)
\end{align*}
$$

Ou seja, a probabilidade de A ocorrer é igual tanto se B ocorreu quanto se B não ocorreu, e vice-versa.

É difícil dizer se eventos são independentes sem calcular antes as probabilidades deles e das suas interseções.

> Lançar duas moedas são eventos independentes?
>
> Os números voltados para cima no lançamento de dois dados e a soma desses números são eventos independentes?
