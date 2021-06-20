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
<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%201/images/Evalute-Model-Linear.png" width="750">
<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%201/images/Evalute-Model-2-Linear.png" width="750">

Conforme o material disponibilizado, esses valores do Evaluate Model todos os valores apresentados nesse modulo, exceto o Coeficiente de determinação(Ultimo valor), devem estar o mais proximo do zero para uma boa qualidade e previsão.

Pipeline de Inferencia utilizado para prever os valores:
<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%201/images/Pipeline-Inferencia.png" width="750">

Esses foram os dados inputados para a IA no teste somente com duas notas:
<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%201/images/Data-Test.png" width="750">

E esse foi o resultado:
<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%201/images/Python-Result.png" width="750">

Esses foram os dados utilizados para todas as colunas:
<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%201/images/Data-test-3.png" width="750">

E esses foram os resultados:
<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%201/images/Python-Result-2.png" width="750">

### Conlusão

Notei que para uma melhor acuracidade na previsão das notas seria necessario mais caracteristicas alem de somente as notas pelo menos considerando este modo de regressão linear, o melhor resultado foi quando teve mais de somente duas colunas de notas para realizar a previsão. Mas com este treinamento da IA foi possivel retornar valores bem aproximados do que realmente aconteceram.
Utilizei tambémn outros modos de regressão mas nenhum apresentou um resultado melhor que esse, talvez pela falta de conhecimento nas configurações e tempo para realizar os desafios.
