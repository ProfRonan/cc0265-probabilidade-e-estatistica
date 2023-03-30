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
   São 6 letras na palavra "POTATO", então $6! = 6 \times 5 \times 4 \times 3 \times 2 \times 1 = 720$.
   Contudo, a letra "O" aparece duas vezes, então devemos dividir por $2! = 2 \times 1 = 2$.
   Também temos que a letra "T" aparece duas vezes, então devemos dividir por $2! = 2 \times 1 = 2$.
   O resultado é $6! / (2! \times 2!) = 720/4 = 180$.
   </details>
2. De quantas maneiras diferentes podemos escolher uma comissão com 3 pessoas de um grupo de 7 membros?
   <details>
   <summary>Resposta</summary>
   Como a ordem não importa, a resposta será dada pela combinação de 7 3 à 3.
   O total é 35.
   </details>
3. Em quantas ordens diferentes podemos organizar uma fila com 5 pessoas?
   <details>
   <summary>Resposta</summary>
   Podemos organizar uma fila com 5 pessoas de 120 maneiras diferentes.
   Que é a a quantidade de permutações de um conjunto com 5 elementos.
   </details>
4. Quantas maneiras diferentes podemos escolher 2 cartas de um baralho de 52 cartas?
   <details>
   <summary>Resposta</summary>
   Contar as formas ee escolher 2 cartas de um baralho de 52 cartas usando a combinação de 52 2 à 2 que resulta em 1326.
   </details>
5. Quantos números de 4 dígitos podem ser formados usando os algarismos 0, 1, 2, 3 e 4, sem repetição?
   <details>
   <summary>Resposta</summary>
   Devemos escolher o primeiro número na sequencia.
   Temos 4 opções: 1, 2, 3 ou 4.
   Para cada uma dessas opções sobram 4 números para escolher o segundo número, o zero e todos os outros da opção anterior menos o que já foi escolhido.
   Para cada opção subsequente sobra um número a menos que na anterior.
   Ou seja, temos 4*4*3*2*1 = 96 opções.
   </details>
6. De quantas maneiras diferentes podemos distribuir 10 livros em duas prateleiras, sendo que a primeira prateleira deve ter 6 livros e a segunda prateleira deve ter 4 livros?
   <details>
   <summary>Resposta</summary>
   Temos que escolher 6 livros para ficar na prateleira de cima.
   São 10 6 à 6 opções que resulta em 210 formas diferentes.
   Os livros da prateleira de baixo são escolhidos automaticamente apos escolhermos os que ficam em cima.
   Agora temos que colocar os livros em cima em ordem que dá 6! maneiras e os livros que ficam em baixo que dá 4! maneiras.
   Ou seja ficamos com 210*6!*4! = 3.628.800
   </details>
7. Quantos anagramas podem ser formados usando as letras da palavra "MATHEMATICS"?
   <details>
   <summary>Resposta</summary>
   A quantidade de permutações assumindo todas as letras distintas é de 11! = 39.916.800.
   Contudo temos a letra M repetida 2 vezes, a letra A repetida 2 vezes, e a letra T repetida 2 vezes também, logo 11!/(2!2!2!) = 4.989.600
   </details>
8. De quantas maneiras diferentes podemos escolher uma equipe de 5 jogadores de um grupo de 10 jogadores?
   <details>
   <summary>Resposta</summary>
   Podemos escolher uma equipe de 5 jogadores de um grupo de 10 jogadores de 252 maneiras diferentes que é a combinação de 10 5 à 5.
   </details>
9. Em quantas maneiras diferentes podemos organizar uma fila com 3 homens e 2 mulheres?
   <details>
   <summary>Resposta</summary>
   Aqui teremos que assumir que os homens são diferentes das mulheres.
   Acho razoável assumir que homens são diferentes entre si e que mulheres são diferentes entre si... Logo 5! = 120 maneiras.
   Mas se você faz parte do grupo que acha que homem é tudo igual e que mulher é tudo igual, então a resposta é a combinação de 5 3 à 3, que são as posições ocupadas pelos homens nos 5 lugares da fila. Resultando em 10 maneiras nesse caso.
   </details>
10. Quantos números ímpares de 3 dígitos podem ser formados usando os algarismos 0, 1, 2, 3, 4, 5 e 6, sem repetição?
    <details>
    <summary>Resposta</summary>
    Aqui temos que escolher um primeiro número que não pode ser zero.
    São 6 opções: 1, 2, 3, 4, 5 ou 6.
    O primeiro número pode ser par ou ímpar.
    No caso de par (3 opções), temos 3 opções para o último número (1, 3 ou 5) e sobram 4 opções para o segundo.
    No caso de ímpar (3 opções), temos 2 opções para o último número (1, 3 ou 5 menos o escolhido para o primeiro) e sobram 4 opções para o segundo.
    Logo temos 3*3*4 + 3*2*4 = 60 opções.
    </details>
11. Quantas formas temos de selecionar 5 cartas de dois baralhos de 52 cartas (assumindo dois baralhos diferentes)?
    <details>
    <summary>Resposta</summary>
      Temos que escolher 5 cartas de dois baralhos de 52 cartas (assumindo dois baralhos diferentes).
      Aqui podemos fazer logo a combinação de 104 5 à 5 que resulta em 91.962.520.
    </details>
12. Quantas formas temos de selecionar 5 cartas de dois baralhos de 52 cartas (assumindo dois baralhos iguais)?
    <details>
    <summary>Resposta</summary>
      Se os dois baralhos são iguais, significa que temos vários pares de cartas iguais.
      Nesse caso se fizermos a combinação simples que nem na questão anterior, estaremos contando várias mãos que são iguais, pois não seria possível distinguir se um às de copas veio de um baralho ou de outro.
      Nesse caso teremos que analisar com mais cuidado.
      Uma opção seria contar todos os arranjos de 5 cartas desses dois baralhos e dividir por 5! o resultado.
      Vendo a questão 13 a resposta é: 3.173.560
    </details>
13. Quantos arranjos com 5 cartas podemos fazer com dois baralhos idênticos de 52 cartas?
    <details>
    <summary>Resposta</summary>
    Sem repetição só temos 52 cartas distintas, logo teremos 52*51*50*49*48 = 311.875.200 formas diferentes de ordenar 5 cartas desses dois baralhos.

    Com um par de cartas iguais, teremos que escolher os dois locais do arranjo em que essas cartas vão aparecer que dá uma combinação de 5 2 à 2 = 10.
    Depois disso temos que escolher o par que será usado, temos 52 pares juntando os dois baralhos, depois sobram 51*50*49 = 124.950 formas diferentes de escolher as últimas 3 cartas tal que duas não sejam iguais.
    Assim terminamos com 10*52*51*50*49 = 64.974.000 formas de arranjar 5 cartas contendo exatamente um par.

    Com dois pares de cartas iguais, podemos primeiramente que escolher os 4 locais do arranjo em que esses pares vão aparecer, temos 5 formas de fazer isso.
    Depois podemos escolher quais pares vão aparecer, temos 52*51 formas de fazer isso.
    Agora, precisamos colocar as 4 cartas nos 4 lugares, contudo, temos cartas repetidas.
    Para calcular quantas formas temos de fazer isso basta escolher duas posições dentre as 4 para um dos pares pois o resto terá que se ajustar de uma única maneira.
    Assim temos 6 formas de fazer isso (4*3/2).
    Finalmente, temos que escolher a carta para ocupar a última posição livre, temos 50 formas de fazer isso.
    Assim temos 5*52*51*6*50 = 3.978.000 formas de arranjar 5 cartas contendo exatamente dois pares.

    Finalmente, podemos calcular o total 311.875.200 + 64.974.000 + 3.978.000 = 380.827.200
    </details>
