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

## Exemplos

1. Quantos anagramas podem ser formados com as letras da palavra "POTATO"?
   <details>
   <summary>Resposta</summary>
   720 anagramas podem ser formados com as letras da palavra "POTATO".
   </details>
2. De quantas maneiras diferentes podemos escolher uma comissão com 3 pessoas de um grupo de 7 membros?
   <details>
   <summary>Resposta</summary>
   Podemos escolher uma comissão com 3 pessoas de um grupo de 7 membros de 35 maneiras diferentes.
   </details>
3. Em quantas ordens diferentes podemos organizar uma fila com 5 pessoas?
   <details>
   <summary>Resposta</summary>
   Podemos organizar uma fila com 5 pessoas de 120 maneiras diferentes.
   </details>
4. Quantas maneiras diferentes podemos escolher 2 cartas de um baralho de 52 cartas?
   <details>
   <summary>Resposta</summary>
   Podemos escolher 2 cartas de um baralho de 52 cartas de 1.326 maneiras diferentes.
   </details>
5. Quantos números de 4 dígitos podem ser formados usando os algarismos 0, 1, 2, 3 e 4, sem repetição?
   <details>
   <summary>Resposta</summary>
   Podemos formar 120 números de 4 dígitos usando os algarismos 0, 1, 2, 3 e 4, sem repetição.
   </details>
6. De quantas maneiras diferentes podemos distribuir 10 livros em duas prateleiras, sendo que a primeira prateleira deve ter 6 livros e a segunda prateleira deve ter 4 livros?
   <details>
   <summary>Resposta</summary>
   Podemos distribuir 10 livros em duas prateleiras, sendo que a primeira prateleira deve ter 6 livros e a segunda prateleira deve ter 4 livros, de 210 maneiras diferentes.
   </details>
7. Quantos anagramas podem ser formados usando as letras da palavra "MATHEMATICS"?
   <details>
   <summary>Resposta</summary>
   Podemos formar 3.628.800 anagramas usando as letras da palavra "MATHEMATICS".
   </details>
8. De quantas maneiras diferentes podemos escolher uma equipe de 5 jogadores de um grupo de 10 jogadores?
   <details>
   <summary>Resposta</summary>
   Podemos escolher uma equipe de 5 jogadores de um grupo de 10 jogadores de 252 maneiras diferentes.
   </details>
9. Em quantas maneiras diferentes podemos organizar uma fila com 3 homens e 2 mulheres?
   <details>
   <summary>Resposta</summary>
   Podemos organizar uma fila com 3 homens e 2 mulheres de 30 maneiras diferentes.
   </details>
10. Quantos números ímpares de 3 dígitos podem ser formados usando os algarismos 0, 1, 2, 3, 4, 5 e 6, sem repetição?
    <details>
    <summary>Resposta</summary>
    Podemos formar 360 números ímpares de 3 dígitos usando os algarismos 0, 1, 2, 3, 4, 5 e 6, sem repetição.
    </details>
