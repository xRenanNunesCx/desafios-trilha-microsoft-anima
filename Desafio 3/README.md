# Desafio 3

### Proposta do Desafio
Entender quais fatores influenciam na nota dos estudantes do ENADE pode oferecer insights sobre os grupos sociais e suas notas. Neste desafio, você deverá utilizar os algoritmos de clusterização para agrupar os estudantes em torno da sua renda (QE_I08), suas horas de estudo (QE_I23) e sua nota geral (NT_GER). Você deverá mostrar a previsão do cluster de um estudante com base nos dados de Renda Mensal, suas horas de estudo e sua nota geral

### Resolução
Este foi o pipeline utilizado para realizar o treino da IA:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%203/images/Pipeline-Treino.png" width="750">

Foi necessario utilizar duas transformação de SQL para filtrar dados nulos e em sequencia que estavam apresentando erro na hora de realizar a importação:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%203/images/SQL-Config1.png" width="750">

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%203/images/SQL-Config-2.png" width="750">

Após realizar o tratamento dos dados foi também realizado o treino da IA resultando nos seguintes valores:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%203/images/Result-Test-Treino.png" width="750">

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%203/images/Result-Test-Treino2.png" width="750">

Este foi o resultado da avaliação:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%203/images/Avaliacao-Model.png" width="750">

Este foi o pipeline utilizado de inferencia:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%203/images/Pipeline-Inferencia.png" width="750">

Estes foram os dados inputados:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%203/images/Data-Input.png" width="750">

Estes foram os resultados obtidos:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%203/images/Data-Input-Result.png" width="750">

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%203/images/Data-Input-Result2.png" width="750">

### Resumo
Neste exercicio foi necessario a utilização de um modulo SQL para que pudesse filtrar os valores nulos que vinham com os dados base. As configurações de treinamento ficaram todas configuradas por padrão e conforme o material base orientou.

### Conlusão
Conforme o desafio 2, através somente dos materiais disponiveis não foi possivel identificar se este treinamento teve um bom desempenho. Mas, neste caso o interessante foi utilizar as transformações de dados para que a IA pudesse aprender de uma forma correta.
