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
