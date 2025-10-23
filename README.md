Título: Controle de potência e velocidade para aspirador de pó inteligente com Perceptron

Esse projeto foi feito pra treinar um perceptron que controla um aspirador de pó inteligente.
As entradas do modelo são:

tipo de piso,

quantidade de poeira,

e número de obstáculos.

E as saídas são:

potência de aspiração (1 a 3),

velocidade de movimento (1 a 5).

A gente usou o modelo Perceptron da biblioteca scikit-learn, porque ele já implementa o algoritmo de forma eficiente e deixa o código mais limpo pra focar na lógica.

A função de ativação escolhida foi a função degrau (step), que é a padrão do perceptron. Ela funciona bem nesse caso porque as saídas são valores discretos (1, 2, 3...), e o modelo só precisa decidir qual classe melhor representa o resultado.

Durante o treinamento, o algoritmo ajusta os pesos até aprender o padrão entre as entradas e as saídas. A gente simulou o processo mostrando o gráfico de erro decaindo com o tempo, que representa o aprendizado do modelo.

Exemplo prático:
Quando o piso é cerâmico (3), tem poeira média (4) e poucos obstáculos (2), o modelo sugere potência 2 e velocidade 3, o que faz sentido porque o aspirador não precisa de força máxima nem andar devagar.

No geral, o resultado foi satisfatório e mostra como um perceptron simples pode ser aplicado em um problema real de controle automático.
Se fosse um sistema comercial, a gente usaria uma rede neural mais complexa (como MLP) pra lidar melhor com situações variadas.
