# Contagem
---

* **Permutação**: arranjos ordenados de n elementos distintos
    * **P<sub>n</sub> = n!**
    * n &ast; (n-1) &ast; (n-2) &ast; ... &ast; 1
        * n possibilidades para o primeiro, n-1 para o segundo, subsequentemente
até o último a ser escolhido


* **Arranjo**: arranjos ordenados de k elementos distintos escolhidos dentre n
possíveis
    * **A<sub>n,k</sub> = n! / (n-k)!**
    * n &ast; (n-1) &ast; (n-2) &ast; ... &ast; (n-(k-1))
        * n possibilidades para o primeiro, n-1 para o segundo, subsequentemente
até (n-(k-1)) para o k-ésimo a ser escolhido


* **Combinação**: maneiras de dispor k elementos desordenados, ou seja, sem
importar a ordem (a,b,c) == (c,b,a), dentre n elementos possíveis
    * **C<sub>n,k</sub> = n! / [k! (n-k)!]**
        * C<sub>n,k</sub> = A<sub>n,k</sub> / k!
        * C<sub>n,k</sub> = (<sup>n</sup><sub>k</sub>)<br>
    * A<sub>n,k</sub> [ORDENADO] = C<sub>n,k</sub> [DESORDENADO] * k! [PERMUTAR]


* **Combinação Completa**: amostras desordenadas com reposição
    * Problema dos sorvetes
        * Comprar 4 sorvetes dentre 7 sabores possíveis
            * |&#95;&#95;|&#95;&ast;|&#95;&ast;|&#95;&ast;|&#95;&ast;|&#95;&#95;|&#95;&#95;|<br>
            Manter fixo as laterais e combinar as "r" bolas e os (n-1) paus
        * Permutação pau-bola
            * Número de soluções inteiras e não negativas de<br>
            x<sub>1</sub> + x<sub>2</sub> + ... + x<sub>r</sub> = n<br>
            C<sub>r-1+n, n</sub> = C<sub>r+n-1, r-1</sub>


* **Técnicas**:
    * Bolas e urnas: distribuição de n bolas em M urnas
        * Bolas idênticas ou iguais, urnas com exclusão (1 bola por urna) ou sem
    * Amostragem: seleção de n elementos de um conjunto de M elementos
        * Conjunto de elementos ORDENADO ou DESORDENADO, seleção COM ou SEM
reposição

|                     |**Bolas Distintas**|**Bolas Iguais**    |
|:-------------------:|:-----------------:|:------------------:|
|**Urna Sem Exclusão**|M<sup>n</sup>      |C<sub>M+n-1, n</sub>|
|**Urna Com Exclusão**|A<sub>M,n</sub>    |C<sub>M,n</sub>     |

|                           |**Amostras Ordenadas**|**Amostras Sem Ordenação**|
|:-------------------------:|:--------------------:|:------------------------:|
|**Retiradas Com Reposição**|M<sup>n</sup>         |C<sub>M+n-1, n</sub>      |
|**Retiradas Sem Reposição**|A<sub>M,n</sub>       |C<sub>M,n</sub>           |


* **Equivalência Analogia "Bolas e Urnas" e "Seleção de Amostras"**:
    * Bola i na urna k <---> i-ésima seleção é o elemento k do conjunto<br>
      Ou, se há uma bola na urna k <---> o elemento k está na amostra
    * **Equivalências**:
        * urna sem exclusão <---> retirada com reposição
        * urna com exclusão <---> retirada sem reposição
        * bolas distintas <---> amostra ordenada
        * bolas iguais <---> amostra desordenada


* **Permutação com elementos repetidos**: deve-se descontar as permutações que
resultarão idênticas
    * P = n! / (n<sub>1</sub>! &ast; n<sub>2</sub>! &ast; ... &ast; n<sub>r</sub>!)
