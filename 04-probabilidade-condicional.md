# Probabilidade Condicional
---

* **Probabilidade Condicional** de um evento A dado que o evento B ocorreu:
    * P(A|B) = <u>P(A&cap;B)</u><br>
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; P(B)


* **Regra do Produto**:
    <pre>P(A&cap;B) = P(A|B)&middot;P(B)
         = P(B|A)&middot;P(A)</pre>

    * *Caso Geral*:
        * P(A<sub>1</sub>&cap;A<sub>2</sub>&cap;...&cap;A<sub>m</sub>)
        = P(A<sub>1</sub>) &middot; P(A<sub>2</sub> | A<sub>1</sub>) &middot;
        P(A<sub>3</sub> | A<sub>2</sub>&cap;A<sub>1</sub>) &middot; &middot;
        &middot; P(A<sub>m</sub> | A<sub>1</sub>&cap; &middot; &middot;
        &middot; &cap; A<sub>m-1</sub>)


* **Teorema da Probabilidade Total**: sejam A<sub>i</sub> (com i de 1 até m)
partições do espaço amostral, ou seja, cuja intersecção de duas partições
diferentes seja sempre vazia. Segue que:
    * P(B) = <sup>m</sup> &Sigma; <sub>i=1</sub> P(B | A<sub>i</sub>) &middot;
    P(A<sub>i</sub>)
    * Exemplo:<br>
      P(B) = P(B &cap; A) + P(B &cap; A<sup>c</sup>)


* **Teorema de Bayes**:
    * P(A<sub>k</sub> | B) = <u>P(B | A<sub>k</sub>) &middot; P(A<sub>k</sub>
    )</u><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;P(B)


* **Eventos Independentes** &hArr; P(A&cap;B) = P(A) &middot; P(B) [sse]
    * *Conjuntamente independentes*: A, B e C independentes se:<br>
        P(A&cap;B) = P(A) &middot; P(B)<br>
        P(A&cap;C) = P(A) &middot; P(C)<br>
        P(B&cap;C) = P(B) &middot; P(C)<br>
        P(A &cap; B &cap; C) = P(A) &middot; P(B) &middot; P(C)<br>


* **Independência Condicional**: A e C são condicionalmente independentes dado B
se:
    * P(A&cap;C | B) = P(A | B) &middot; P(C | B) *com P(B) > 0 ou   <br>*
    P(A&cap;C | B) = P(A&cap;B) *com P(B) = 0*
