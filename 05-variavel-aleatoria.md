# Variáveis Aleatórias
---

* **Variável Aleatória Y**: função Y: &Omega; &rArr; &real;, Y(&omega;) &isin; &real;
    * *Variável Aleatória Discreta*: assume valores em um conjunto enumerável
        1. **Suporte**: valores *y<sub>i</sub>* que a variável assume no intervalo
        2. **Atribuição de probabilidade** para cada valor que a variável assume:<br>
        p(y<sub>i</sub>) = P(Y = y<sub>i</sub>)
        3. Verificar que &Sigma; <sub>i</sub> p(y<sub>i</sub>) = 1
    * *Variável Aleatória Contínua*: assume valores em intervalos de &real;


* **Esperança Matemática - V.A. Discreta**:
    * &mu;<sub>Y</sub> = E(Y) = &Sigma;<sub>i</sub> (y<sub>i</sub> * P(Y = y<sub>i</sub>))
* **Esperança Matemática - Função**: Y é variável aleatória discreta
    * E[g(Y)] = &Sigma;<sub>i</sub> (g(y<sub>i</sub>) * p(y<sub>i</sub>))
* **Variância - V.A. Discreta**:
    * &sigma;<sup>2</sup><sub>Y</sub> = Var(Y) = E[(Y - &mu;<sub>Y</sub>)<sup>2</sup>]
    = &Sigma;<sub>i</sub>(y<sub>i</sub> - &mu;<sub>Y</sub>)<sup>2</sup> * P(Y =
    y<sub>i</sub>)
    * Var(Y) = E(Y^2) - [E(Y)]^2<br>
      Var(Y) = E(Y^2) - &mu;<sub>Y</sub><sup>2</sup><br>
      Var(Y) = &Sigma;<sub>i</sub>(y<sub>i</sub>^2 * p(y<sub>i</sub>)) - &mu;<sub>Y</sub><sup>2</sup>


* **Função Indicadora**: 1l<sub>A</sub>(x) = {0 se x &notin; A; 1 se x &isin; A}
    * 1l<sub>A<sup>c</sup></sub>(x) = 1 - 1l<sub>A</sub>(x)


* **Modelo Bernoulli**: Y ~ Bernoulli(p)
    * p(k) = P(Y = k) = p^k * (1-p)^(1-k) &ast; indicadora
    * p é a probabilidade de Sucesso
    * E(Y) = p e Var(Y) = p * (1-p)


* **Modelo Binomial**: **n** ensaios de Bernoulli independentes, com mesma
probabilidade **p** de sucesso. Com X = número de sucessos nos **n** experimentos:
    * X ~ Binomial (n,p)
    * p(k) = P(X = k) = Cn,k &ast; p^k * (1-p)^(n-k) &ast; indicadora
    * E(Y) = np e Var(Y) = np * (1-p)


* **Modelo Hipergeométrico**: população **N**, com **r** de característica especial,
selecionando **n** elementos sem reposição.
    * Definindo Y como número de elementos com determinada característica especial
    * Y ~ Hipergeométrica(N,r,n)
    * P(Y = k) = C(r,k) * C(N-r, n-k)/ C(N,n)
    * **n** ensaios de Bernoulli de probabilidae de sucesso **p = r/N**
    * E(Y) = n * r / N
    * Var(Y) = n &ast; r / N &ast; (1 - r / N) &ast; (N-n / N-1)


* **Modelo Poisson**: &lambda; &Rarr; taxa de ocorrência de evento em determinado tempo,
comprimento, área ou volume.
    * Y &rArr; número de ocorrências nesse dado intervalo
    * Y ~ Poisson(&lambda;)
    * P(Y = k) = e^(-&lambda;) &ast; (&lambda;^k / k!) &ast; indicadora
    * E(Y) = Var(Y) = &lambda;<br>
    * Exemplo: 3000 metros de fita com ocorrência de 1 defeito a cada 2000 metros
        * &lambda; = (1 / 2000) * 3000 = 1,5


* **Modelo Geométrico**: sequência de ensaios de Bernoulli **independentes** e
de mesma probabilidade **p** de sucesso.
    * Y = número de ensaios até obter o primeiro sucesso<br>
    Y ~ Geométrica(p)
    * p(k) = P(Y = k) = (1 - p)^(k-1) &ast; p &ast; indicadora
    * E(Y) = 1/p e Var(Y) = (1-p)/p^2
    * Sendo X = número de fracassos até obter o primeiro sucesso, ou seja,
    Y = X + 1 (excluindo-se o sucesso)<br>
    X ~ Geométrica(p)
    * p(x) = P(X = x) = (1 - p)^x &ast; p &ast; indicadora
    * E(X) = (1 - p)/p e Var(X) = (1 - p)/p^2


* **Modelo Binomial Negativa**: ensaios de Bernoulli independentes de mesma
probabilidade **p** de sucesso
    * Y = número de ensaios até obter o r-ésimo sucesso<br>
      Y ~ Binomial Negativa(r, p)
    * p(y) = P(Y = y) = C<sub>y-1, r-1</sub> &ast; (1 - p)^(y-r) &ast; p^r *
    indicadora
    * E(Y) = r &ast; 1/p e Var(Y) = r &ast; (1-p)/p^2
    * X = número de fracassos até obter o r-ésimo sucesso, ou seja, Y = X + r<br>
      X ~ Binomial Negativa(r, p)
    * p(x) = P(X = x) = C<sub>x+r-1, x</sub> &ast; (1-p)^x &ast; p^r * indicadora
    
