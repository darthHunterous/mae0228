# Teoria das Probabilidades
---

* **Espaço de Probabilidade**: (Ω, F, P)
    * *Espaço Amostral (Ω)*: todos possíveis resultados do experimento
    * *σ−Álgebra* (F): coleção de eventos e operações sobre o Espaço Amostral
    * *Função Probabilidade(P)*: definida em F


* *Espaço de Probabilidade Discreto*: constituído de elementos contáveis ou
enumeráveis
    * F coleção de todos subconjuntos de Ω


* **Função de Probabilidade**: P: F -> [0,1]
    * *Axioma 1*: P(Ω) = 1
    * *Axioma 2*: A ∈ F, 0 ≤ P(A) ≤ 1
    * *Axioma 3*: σ-Aditividade
        * Para eventos mutuamente exclusivos (disjuntos), ou seja, que não
intersectam: P(<sup>&infin;</sup>U<sub>i=1</sub> A<sub>i</sub>) = <sup>&infin;</sup>&Sigma;<sub>i=1</sub> P(A<sub>i</sub>)
    * *Propriedades*
        1. P(&empty;) = 0
        2. Eventos mutuamente exclusivos &rArr; <br>
           P(<sup>n</sup>U<sub>k=1</sub> A<sub>k</sub>) =
           <sup>n</sup>&Sigma;<sub>k=1</sub> P(A<sub>k</sub>)
        3. P(A<sup>c</sup>) = 1 - P(A)
        4. B &sub; A &rArr; P(A) &ge; P(B)
        5. *Regra de Adição de Probabilidades*: <br>
           P(A &cup; B) = P(A) + P(B) - P(A &cap; B)
        6. *Fórmula da Inclusão-Exclusão / Teorema de Poincaré*:
            ![Fórmula da Inclusão-Exclusão](https://github.com/darthHunterous/notes/blob/master/mae0228/z-photo-01-poincare.png)<br>
            Problema dos Pareamentos/Coincidências
        7. *Sub-&sigma;-aditividade*:
            * P(<sup>&infin;</sup>U<sub>i=1</sub> A<sub>i</sub>) &le; <sup>&infin;</sup>&Sigma;<sub>i=1</sub> P(A<sub>i</sub>) <br>
            Também válido para uma quantidade finita de eventos
