# Variáveis Aleatórias Contínuas
---

* **Variável Aleatória Contínua**:<br>
  F<sub>Y</sub>(y) = P (Y <= y) = <sub>-&infin;</sub>&int;<sup>y</sup> f(u)du


 * **Função Densidade de Probabilidade**: função f da variável aleatória
 <br> contínua Y
    * f(y) >= 0
    * <sub>-&infin;</sub>&int;<sup>+&infin;</sup> f(u)du = 1
    * f(y) = &part;F(y) / &part;y


1. Especificar suporte D &sube; &real;
2. f(y) > 0 para y &isin; D [Densidade positiva no suporte]
3. Verificar &int; f(u)du = 1    


* **Esperança Matemática**: de Variável Aleatória Contínua
    * &mu;<sub>Y</sub> = E(Y) = &int; y f(y) dy
* **Esperança Matemática**: de função de Y como V.A. contínua com f.d.p.
f(y)
    * E[g(Y)] = &int; g(y) f(y) dy
* **Esperança V.A. Contínua Não-Negativa**: P(X >= 0) = 1
    * E(X) = <sub>0</sub>&int;<sup>&infin;</sup> (1 - F(u)) du


* **Variância V.A. Contínua**:
    * &sigma;<sub>Y</sub>^2 = Var(Y) = E[(Y - &mu;<sub>Y</sub>)^2] = &int;
    (y - &mu;<sub>Y</sub>)^2 f(y) dy
    * *Expressão Alternativa*:<br>
    Var(Y) = E(Y^2) - [E(Y)]^2<br>
    Var(Y) = E(Y^2) - &mu;<sub>Y</sub>^2<br>
    Var(Y) = &int; y^2 f(y) dy - &mu;<sub>Y</sub>^2<br>


* **Modelo Uniforme**: Y ~ Uniforme[a,b], a < b
    * f.d.p -> f(y) = 1 / (b - a) &ast; indicadora [a,b] (y)
    * E(Y) = (a+b) / 2
    * Var(Y) = (b-a)^2/12


* **Modelo Exponencial**: Y ~ Exponecial(&lambda;), &lambda; > 0
    * f.d.p -> f(y) = &lambda; &ast; e^(-&lambda;y) &ast; indicadora (0, &infin;) (y)
    * E(Y) = 1 / &lambda;
    * Var(Y) = 1 / &lambda;^2
    * Parâmetro &lambda; -> taxa<br>
    Parâmetro &beta; -> média <br>
    &beta; = 1 / &lambda;


* **Propriedade da Falta de Memória**:
    * P(Y > s + t | Y > s) = P(Y > t), &forall; s,t >0
    * A distribuição Exponencial é a única contínua com tal propriedade


* **Modelo Gama**: Y ~ Gama(a, &lambda;), a, &lambda; > 0
    * f.d.p. -> f(y) = (1 / &Gamma;(a)) &ast; &lambda;^a &ast; y^(a-1) &ast;
    e^(-&lambda;y) &ast; indicadora (0, &infin;) (y)
        * **Função Gama**:
            * &Gamma;(a) = <sub>0</sub>&int;<sup>&infin;</sup> u^(a-1) &ast;
            e^(-u) du
                * &Gamma;(1) = 1
                * &forall; a &isin; &real;<sup>+</sup> -> &Gamma;(a) > 0 e
                &Gamma;(a+1) = a &ast;&Gamma;(a)
                * n &isin; &Nopf; -> &Gamma;(n) = (n-1)!
                * &Gamma;(1/2) = &radic;&pi;
                * Provar que a soma da f.d.p é 1 -> substituição u = &lambda;y
        * a &isin; &Nopf; -> Gama(a, &lambda;) = Erlang(a, &lambda;)
        * A substituição &lambda; = 1 / &beta; também é válida
        
