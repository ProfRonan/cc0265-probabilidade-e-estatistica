# Técnicas de Contagem

Contar parece fácil, mas não é.

> One, two, many, lots
> -- Trolls counting, Terry Pratchett

Técnicas de contagem nos permitem contar elementos de um espaço amostral sem "realmente" contar eles.

## Princípio Multiplicativo

Uma operação pode ser realizada em $k$ passos:

- a quantidade de formas de se realizar o primeiro passo é $n_1$;
- a quantidade de formas de se realizar o segundo passo é $n_2$, qualquer que seja a forma escolhida para o $1$;
- a quantidade de formas de se realizar o segundo passo é $n_3$, qualquer que seja a forma escolhida para o $2$;
- a quantidade de formas de se realizar o segundo passo é $n_4$, qualquer que seja a forma escolhida para o $3$...
- a quantidade de formas de se realizar o segundo passo é $n_k$, qualquer que seja a forma escolhida para o $k - 1$.

A quantidade total de formas diferentes de realizar esse processo é dada por $n_1 \times n_2 \times n_3 \times \cdots \times n_k$.

### Exemplo

- Quantas sequencias diferentes de caras e coroas temos com 10 lançamentos de uma mesma moeda?
- Quantas formas diferentes é possível vestir uma calça e uma blusa usando o seu guarda-roupa?

## Permutações

Uma permutação é uma ordem específica dos elementos de um conjunto.

A quantidade de permutações de um conjunto com $n$ elementos é definida por $P^n = n!$.

> Lembrando
> $$n! = 1 \times 2 \times 3 \times \cdots \times (n - 1) \times n$$

## Arranjo

Um arranjo é uma ordem de parte dos elementos de um conjunto.

Se um conjunto tem $n$ elementos e queremos saber a quantidade de arranjos com $k$ elementos denotamos essa quantidade por

$$P^n_k = \frac{n!}{(n - r)!}$$

## Permutações com Repetição

Quando temos elementos repetidos em um conjunto e gostaríamos de ordenar os elementos, mas considerando que elementos iguais são indistinguíveis quando colocados nas mesmas posições podemos usar a permutação com repetição.

Se o número de elementos é dado por $n = n_1 + n_2 + n_3 + \cdots + n_r$, sendo $n_i$ é a quantidade de vezes que o elemento $i$ está repetido.

A quantidade de permutações do conjunto considerando essas repetições é definida por

$$\frac{n!}{n_1! n_2! n_3! \cdots n_r!}$$

## Combinações

Uma combinação é um subconjunto de um conjunto.

Quando dizemos combinações de $n$, $r$ à $r$ denotado por $\binom{n}{r}$ estamos nos referindo à quantidade de formas que existem de escolher um subconjunto de tamanho $r$ de um conjunto de tamanho $n$.

Nesse caso, a ordem relativa dos elementos de um subconjunto não importa.

$$ \binom{n}{r} = \frac{n!}{(n - r)! r!}$$
