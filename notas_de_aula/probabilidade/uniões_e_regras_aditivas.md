# Uniões e Regras Aditivas

Normalmente, estamos interessados não só em probabilidades de eventos, mas também na probabilidade das uniões e interseções de eventos.

> **Probabilidade da União**
>
> $$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$

Se $A \cap B = \emptyset$, logicamente, $P(A \cup B) = P(A) + P(B)$.

Quando estamos falando da união de mais conjuntos as coisas começam a ficar mais complicadas...

$$
\begin{align*}
P(A \cup B \cup C) &= P((A \cup B) \cup C)\\
                   &= P(A \cup B) + P(C) - P((A \cup B) \cap C)\\
                   &= P(A) + P(B) - P(A \cap B) + P(C) - P((A \cup B) \cap C)\\
                   &= P(A) + P(B) + P(C) - P(A \cap B) - P((A \cap C) \cup (B \cap C))\\
                   &= P(A) + P(B) + P(C) - P(A \cap B) - (P(A \cap C) + P(B \cap C) - P(A \cap B \cap C))\\
                   &= P(A) + P(B) + P(C) - P(A \cap B) - P(A \cap C) - P(B \cap C) + P(A \cap B \cap C)
\end{align*}
$$

Agora, se todos os eventos são mutuamente exclusivos 2 a 2, as coisas ficam bem mais simples...

Se $E_1, E_2, \ldots, E_n$ são eventos mutuamente exclusivos, então

$$P(E_1 \cup E_2 \cup \cdots \cup E_n) = \sum^n_{i = 1}P(E_i)$$
