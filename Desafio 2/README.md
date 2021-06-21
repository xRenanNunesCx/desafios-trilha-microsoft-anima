# Desafio 2

### Proposta do Desafio
Escolha um estado da federação e clusterize os estudantes do enade com base em suas respostas ao questionário socioeconômico.
Neste problema, você deverá selecionar alguns campos do questionário sócioeconomico Renda Mensal (Q006), acesso a internet (Q025) e a nota final da redação (NU_NOTA_REDACAO) e agrupar os estudantes. Você deverá mostrar a previsão do cluster de um estudante com base nos dados de Renda Mensal, acesso a internet e nota final da redação informados

### Resolução
Neste exercicio foi necessario utilizar um transformação em SQL para que eu pudesse filtrar os dados por uma UF especifica, neste caso utilizei SP:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%202/images/Config-SQL-1.png" width="750">

Após isso todo o tratamento dos dados necessarios e o treinamento foram realizados.Realizaei a separação em 3 pontos conforme no material base. Com o treinamento do cluster tive o seguinte resultado:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%202/images/Score-Data-To-Cluster.png" width="750">

Após a utilização do Evaluate Model tive os seguintes resultados:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%202/images/Evaluate-Model.png" width="750">

Este foi o pipeline utilizado para inferencia:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%202/images/Pipeline-Inferencia.png" width="750">

Esses foram os dados inputados:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%202/images/Data-Test.png" width="750">

E esse foi o resultado:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%202/images/Result-Cluster.png" width="750">

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%202/images/Result-2-Cluster.png" width="750">

### Resumo
Neste desafio foi necessario a utilização de um modulo para filtrar os valores pela UF escolhida, assim foi possivel tratar esses dados limpando os valores inexistentes e tratando novamente o restante. As configurações de treinamento ficaram todas configuradas por padrão e conforme o material base orientou.

### Conlusão
Através somente dos materiais disponiveis não foi possivel identificar se este treinamento teve um bom desempenho ou não, pois não sei o quão disperso os valores deveriam ficar para se tornar algo ideal. Aparentemente se comportou da maneira esperada.
