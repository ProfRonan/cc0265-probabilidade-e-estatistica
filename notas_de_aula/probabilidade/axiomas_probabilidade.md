# Interpretações e Axiomas de Probabilidade

Probabilidade para espaços amostrais **discretos**.

> Discreto na matemática significa um conjunto finito ou idempotente ao conjunto dos números naturais.

**Probabilidade** é uma forma de mensurar _certeza_.

> Tem 50% de chance de dar certo.
> Ou dá certo, ou não dá certo!
> -- Alguém muito otimista se estiver falando de ganhar na mega sena.

A **probabilidade** de um evento ocorrer é um número no intervalo $[0, 1]$ aonde $1$ ou $100%$ é certeza absoluta em que ele ocorre e $0$ ou $0%$ é a certeza absoluta em que ele **não** ocorre.

A **probabilidade** pode ser obtida de forma _subjetiva_ aonde alguém usando a _intuição_ mensura a possibilidade de um evento ocorrer.

> Se não chover até o dia 19 de Março, então é um ano sem chuvas.
>
> Isso não é probabilidade pois não indica o _valor_ dessa certeza.

> Existe 90% de chance de errar o bind (Q) da Morgana jogando LoL
>
> [Gif do Bind da Morgana](https://gfycat.com/popularimportantamericangoldfinch)
>
> Isso é uma probabilidade _subjetiva_ pois é baseada na minha intuição quando joguei o jogo nas últimas vezes.

A **probabilidade** pode ser obtida de forma _empírica_ aonde um experimento é realizado à _"exaustão"_ e a frequência relativa dos eventos é calculada formado a base da probabilidade.

> Pegue um dado de 6 lados e jogue ele 10.000 vezes.
>
> Anote quantas vezes saiu cada um dos números $1$, $2$, $3$, $4$, $5$, $6$.
>
> A probabilidade de sair o número $i$ pode ser vista como a quantidade de vezes que saiu de fato $i$ dividida por 10.000.
>
> Essa é uma probabilidade _empírica_ baseada nos resultados de um experimento aleatório.

## Definição Formal

Uma função $P$ que associa subconjuntos de um espaço amostral $\Omega$ à um número no intervalo $[0, 1]$ é uma **função de probabilidade** se e somente se:

- $P(\Omega) = 1$;
- $0 \leq P(E) \leq 1$ qualquer que seja o evento $E$;
- Dados dois eventos $A$ e $B$ com $A \cap B = \emptyset$:
  - $P(A \cup B) = P(A) + P(B)$.

## Observações

Não existe uma forma _perfeita_ e _universal_ de associar um modelo matemático à um fato/evento do mundo real.
Sempre será necessária a criatividade humana e observação para criar um modelo probabilístico (_Espaço Amostral e Função de Probabilidade_) para representar um fenômeno real.

Experimentos controlados são uma das maneiras que tentamos construir modelos probabilísticos realistas.

Escrutínio e criatividade também é uma das maneiras de se fazer isso.

A _melhor maneira_ é aquela que funciona para resolver o problema em questão.

## Função de Probabilidade Equiprovável

Dizemos que um espaço aleatório com $N$ elementos é equiprovável se para cada evento unitário a função de probabilidade desse evento é dada por $1/N$.

## Exemplo e Notação

Seja o modelo probabilístico que _tenta_ modelar o lançamento de dois dados para analisar o valor da **SOMA** dos números das faces voltadas para cima quando esses dois dados param de se mover.

Podemos definir o espaço amostral como:

$$\Omega_1 = \\{(x,y) \mid x \in \\{1, 2, 3, 4, 5, 6\\} \quad y \in \\{1, 2, 3, 4, 5, 6\\}\\}$$

que faria diferença entre os números dos dois dados, poderíamos obter a soma somando o $x$ e $y$.

Outro espaço amostral poderia ser:

$$\Omega_2 = \\{2, 3, 4, \ldots, 12\\}$$

### Escolher a Função de Probabilidade

Uma opção, usando o espaço amostral $\Omega_1$, seria escolher uma função de probabilidade equiprovável.

Ou seja, cada evento $\\{(x, y)\\}$ receberia probabilidade $1/36$.

> **Notação** para eventos unitários, $E = \\{e\\}$, é mais fácil escrever $P(e)$ do que $P(\\{e\\})$.
> Portanto, vamos escrever simplesmente $P(e)$ quando for um evento unitário.

Podemos escrever o evento em que a soma dos dados dá $7$ como o evento

$$E_7 = \\{(1, 6), (2, 5), (3, 4), (4, 3), (5, 2), (6, 1)\\}$$

Assim, $P(E_7) = P((1, 6)) + P((2, 5)) + P((3, 4)) + P((4, 3)) + P((5, 2)) + P((6, 1)) = 6/36$.

Parece razoável?

Se usarmos uma função de probabilidade equiprovável para $\Omega_2$, concluiríamos que a probabilidade de sair a soma $7$ é de $1/12$, como $1/12 \neq 6/36$ obviamente um dos dois não representa fielmente a realidade, qual estaria certo? Podemos tentar simular isso [usando um computador](soma_dois_dados.ipynb).
