# Variáveis Aleatórias Conjuntas
---

* **Função Distribuição Conjunta**:
    * F(x,y) = P(X &le; x, Y &le; y)<br>
    F(x,y) = &Sigma;{u<=x} &Sigma;{v<=y} P(X = u, Y = v)<br>
    F(x,y) = &Sigma;{u<=x} &Sigma;{v<=y} p<sub>X,Y</sub>(u,v)
    [X e Y discretas]<br>
    F(x,y) = <sub>-&infin;</sub>&int;<sup>y</sup> <sub>-&infin;</sub>&int;<sup>x</sup> f(u,v) du dv [X e Y contínuas]


* **Função Densidade de Probabilidade Conjunta - V.A. Contínuas**:
    * f<sub>X,Y</sub>(u,v) &ge; 0
    * &int;&int; f<sub>X,Y</sub>(u,v) du dv = 1
    * f<sub>X,Y</sub>(x,y) = &part;^2/&part;x&part;y F(x,y) =
    &part;^2/&part;y&part;x F(x,y)
    * **Densidades marginais**:
        * f<sub>X</sub>(x) = <sub>-&infin;</sub>&int;<sup>&infin;</sup>
        f(x,y) dy
        * f<sub>Y</sub>(y) = <sub>-&infin;</sub>&int;<sup>&infin;</sup>
        f(x,y) dx


* **Função Distribuição de Probabilidade Conjunta - V.A. Discretas**:
    * P(X = a, Y = b) = p<sub>X,Y</sub>(a,b) &ge; 0
    * &Sigma;{x} &Sigma;{y} p<sub>X,Y</sub> (x,y) = 1


* **Distribuição Condicional**:
    * P(Y = y | X = x<sub>0</sub>) = P(X = x<sub>0</sub>, Y = y) /
    P(X = x<sub>0</sub>)<br>
    * P(Y = y | X = x<sub>0</sub>) = p<sub>X,Y</sub>(x<sub>0</sub>, y) /
    p<sub>x</sub>(x<sub>0</sub>)


* **Densidade Condicional**:
    * f<sub>Y|X</sub> (y | x<sub>0</sub>) = f<sub>X,Y</sub>(x<sub>0</sub>,y)
    / f<sub>X</sub>(x<sub>0</sub>)


* **Independência Variáveis Aleatórias**:
    * *Discretas*: p<sub>X,Y</sub> = p<sub>X</sub>(x) &ast; p<sub>Y</sub>(y)
    * *Contínuas*: f<sub>X,Y</sub> = f<sub>X</sub>(x) &ast; f<sub>Y</sub>(y)
