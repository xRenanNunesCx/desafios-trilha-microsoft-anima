# Desafio 1

### Proposta do Desafio
Você deverá realizar uma análise de regressão para descobrir se é possível prever a nota da prova de Ciências da Natureza caso se saiba a nota de outra.
Você deverá mostrar a previsão de uma nota de Ciências da Natureza com base em uma nota da prova de Matemática.

### Resolução

Segue abaixo o pipeline utilizado para realização desse desafio:
<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%201/images/Pipeline-Geral.png" width="750">

Como o enunciado ficou um pouco aberto, realizei dois tipos de treinamento. Primeiro passei os campos NU_NOTA_CN e NU_NOTA_MT para treinamento e tive o seguinte resultado:
<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%201/images/Score-Model-Single-Value.png" width="750">

Após isso realizei o treinamento passando as demais notas e tive o seguinte resultado:
<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%201/images/Score-Model-Other%20Values.png" width="750">

Ao avaliar os dois modelos com o modulo Evaluate Model os dois apresentaram uma pequena diferença nos resultados, mas percebi que ao passar todas as notas e não somente so duas ela apresentou um resultado mais satisfatorio.

Segue imagens do resultado do Evaluate Model:
<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%201/images/Evalute-Model-Linear.png" width="500">
<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%201/images/Evalute-Model-2-Linear.png" width="500">
