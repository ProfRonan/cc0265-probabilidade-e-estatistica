# Teorema de Bayes

O teorema de Bayes é uma fórmula matemática que nos permite atualizar as probabilidades de um evento ocorrer com base em novas evidências. Ele foi desenvolvido pelo matemático britânico Thomas Bayes no século XVIII e é usado em muitos campos, incluindo estatística, ciência da computação, inteligência artificial e medicina.

A fórmula do teorema de Bayes é a seguinte:

$$
P(A \mid B) = \frac{P(B \mid A) P(A)}{P(B)}
$$

Onde:

- $P(A \mid B)$ é a probabilidade condicional de $A$ ocorrer dado que $B$ ocorreu;
- $P(B \mid A)$ é a probabilidade condicional de $B$ ocorrer dado que $A$ ocorreu;
- $P(A)$ é a probabilidade de $A$ ocorrer;
- $P(B)$é a probabilidade de $B$ ocorrer.

## Exemplo

Suponha que uma empresa produza um produto em duas fábricas diferentes: a Fábrica A e a Fábrica B.
No entanto, devido a um erro de rotulagem, não é possível distinguir os produtos produzidos por uma fábrica daqueles produzidos pela outra.
A empresa sabe que $60\%$ dos produtos são produzidos na Fábrica A e $40\%$ são produzidos na Fábrica B.

Agora, suponha que um produto selecionado aleatoriamente é defeituoso.
A empresa sabe que a Fábrica A produz $3\%$ de produtos defeituosos, enquanto a Fábrica B produz $5\%$ de produtos defeituosos.
Qual é a probabilidade de que o produto defeituoso selecionado tenha sido produzido na Fábrica B?

Usando o Teorema de Bayes, podemos calcular a probabilidade de que o produto defeituoso selecionado tenha sido produzido na Fábrica B da seguinte maneira:

- $B$ o produto defeituoso selecionado é produzido na Fábrica B
- $D$ o produto selecionado é defeituoso
- $P(B) = 0.4$ (probabilidade de que o produto seja produzido na Fábrica B)
- $P(D \mid B) = 0.05$ (probabilidade de que um produto produzido na Fábrica B seja defeituoso)
- $P(D \mid B') = 0.03$ (probabilidade de que um produto produzido na Fábrica A seja defeituoso)

Agora podemos usar a fórmula do Teorema de Bayes para calcular a probabilidade de que o produto defeituoso selecionado tenha sido produzido na Fábrica B:

$$
\begin{align*}
P(B \mid D) &= \frac{P(D \mid B) P(B)}{P(D)}\\
&= \frac{P(D \mid B) P(B)}{P(D \mid B)P(B) + P(D \mid B')P(B')}\\
&= \frac{0.05 \times 0.4}{0.05 \times 0.4 + 0.03 \times 0.6}\\
&= 0.4\\
\end{align*}
$$

Portanto, a probabilidade de que o produto defeituoso selecionado tenha sido produzido na Fábrica B é de $40\%$.

## Exercícios de Fixação sobre Probabilidade

1. Uma urna tem 5 bolas vermelhas e 3 bolas brancas.
   Se duas bolas são sorteadas sem reposição, qual a probabilidade de que ambas sejam vermelhas?
2. Uma moeda é lançada três vezes consecutivas.
   Qual é a probabilidade de obter exatamente duas caras?
3. Uma máquina de venda automática fornece pacotes com 1 brinquedo dentro.
   Em uma certa compra, uma pessoa compra 4 pacotes.
   Qual a probabilidade de ela receber pelo menos 1 brinquedo raro, sabendo que há um brinquedo raro em cada 5 pacotes?
4. Uma empresa tem um total de 100 funcionários, dos quais 60 são homens e 40 são mulheres.
   Se 5 funcionários são selecionados aleatoriamente para formar uma comissão, qual é a probabilidade de que pelo menos duas mulheres sejam selecionadas?
5. Uma caixa contém 4 bolas vermelhas, 3 bolas brancas e 2 bolas azuis.
   Duas bolas são sorteadas sem reposição. Qual é a probabilidade de que a primeira bola sorteada seja vermelha?
6. Uma pessoa tem uma moeda viciada que cai cara com probabilidade 0,7 e coroa com probabilidade 0,3.
   A pessoa lança a moeda 5 vezes.
   Qual é a probabilidade de que ela obtenha exatamente 3 caras?
7. Uma cidade tem 3 hospitais.
   O hospital A tem 40% dos pacientes, o hospital B tem 35% e o hospital C tem 25%.
   Se um paciente é selecionado aleatoriamente, qual é a probabilidade de ele ser atendido no hospital B ou C?
8. Uma pessoa tem duas moedas, uma viciada que cai cara com probabilidade 0,6 e coroa com probabilidade 0,4, e outra moeda honesta.
   A pessoa escolhe uma das moedas ao acaso e a lança 3 vezes.
   Qual é a probabilidade de que ela tenha escolhido a moeda viciada, sabendo que ela obteve 2 caras e 1 coroa?
9. Uma empresa de engenharia produz duas peças de um mesmo tipo.
   A probabilidade de que a primeira peça seja defeituosa é 0,1 e a probabilidade de que a segunda peça seja defeituosa é 0,2.
   Qual é a probabilidade de que ambas as peças sejam defeituosas?
10. Uma determinada doença é detectada em 90% dos casos em que está presente.
    O teste de diagnóstico tem uma taxa de falsos positivos de 10%.
    A doença ocorre em 1% da população.
    Se uma pessoa testa positivo para a doença, qual é a probabilidade de que ela realmente tenha a doença?
11. Suponha que você tenha dois sacos, cada um contendo uma mistura de bolas vermelhas e brancas.
    No primeiro saco, há 2 bolas vermelhas e 3 bolas brancas.
    No segundo saco, há 4 bolas vermelhas e 1 bola branca.
    Um saco é escolhido aleatoriamente e, em seguida, uma bola é retirada do saco escolhido.
    Se a bola for vermelha, qual é a probabilidade de que ela tenha sido retirada do segundo saco?
12. Uma fábrica produz parafusos em duas máquinas, A e B.
    A máquina A produz 60% dos parafusos e tem uma taxa de defeito de 2%.
    A máquina B produz 40% dos parafusos e tem uma taxa de defeito de 5%.
    Se um parafuso escolhido aleatoriamente for defeituoso, qual é a probabilidade de que ele tenha sido produzido pela máquina B?
13. Suponha que um dado de seis faces é lançado.
    A probabilidade de que o resultado seja um número par é de 1/2.
    Se o resultado for um número par, qual é a probabilidade de que seja um 4?
