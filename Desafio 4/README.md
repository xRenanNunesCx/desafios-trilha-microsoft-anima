# Desafio 4

### Proposta do Desafio
Será que as notas no ENADE vão aumentar ou diminuir? Acesse os microdados das provas anteriores 2019, 2018, 2017, 2016 e 2015 e faça uma análise de regressão para verificar se a nota geral (NT_GER) tendem a aumentar ou a diminuir nos anos de 2020 e 2021. Você deverá mostrar a previsão das notas do ENADE para os anos de 2020 e 2021.

### Resolução
Neste exercicio foi utilizado uma serie de tratamento de dados conforme o pipeline abaixo mostra:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%204/images/Pipeline-Treinamento1.png" width="750">

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%204/images/Pipeline-Treinamento2.png" width="750">

Após todo o tratamento a IA foi treinada e foi possivel obter os seguintes resultados:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%204/images/Score-Model.png" width="750">

Após aplicar o modulo Evaluate Model o mesmo retornou:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%204/images/Evaluate-Model.png" width="750">

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%204/images/Evaluate-Model2.png" width="750">

Media da Notal Geral com base nos anos anteriores:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%204/images/NT_GER.png" width="750">

Segue o pipeline de inferencia:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%204/images/Pipeline-Inferencia.png" width="750">

Forma em que os anos foram inputados:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%204/images/Input-Ano.png" width="750">

Resultado de 2020:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%204/images/Nota_2020.png" width="750">

Nota de 2021:

<img src="https://github.com/xRenanNunesCx/desafios-trilha-microsoft-anima/blob/main/Desafio%204/images/Nota_2021.png" width="750">


### Resumo
Neste desafio foi realizados diversas transformações de dados, na parte de juntar os datasets, tratar valores nulos de outros anos, valores de erros também algo que tomou muito tempo durante o processo para descobrir quais tratamentos deveriam ser utilizados e qual a melhor forma de otimizar isso. Os modelos de treinamento utilizados estavam configurados com seus valores padrões e conforme o material base informou.

### Conclusão
Conforme visto nos resultados depois que foi feito o input do ano, as notas seguem uma tendencia de queda. Isso foi possivel notar através da media das notas de todos os outros anos.
