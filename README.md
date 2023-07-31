# Análise de Perfil de Clientes para Identificação do Cliente Ideal

### Sobre:

Análise da base de dados em busca de identificar o cliente ideal para a empresa com base no histórico de compras.

### Proposta:

Com informações extraídas de uma base de dados em formato .csv, será realizada uma análise de perfil, levando em consideração as informações que mais impactam na nota dos clientes.
###
Será feita uma análise exploratória com o objetivo de identificar os principais fatores que influenciam na nota dos clientes.
###
A solução final consistirá em um conjunto de gráficos, a partir dos quais serão extraídos insights baseados nessas análises.

### Linguagem Utilizada:
###
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=white&color=black)

### Bibliotecas Utilizadas:
###
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white&color=black) 	![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white&color=black)

### Metodologia:

Inicialmente, utilizamos a biblioteca **Pandas** para importar e ler a base de dados. Enfrentamos um problema de encoding, pois a base de dados estava em português, então resolvemos o problema utilizando a propriedade **encoding='latin'** e a propriedade **sep=';'** para organizar e melhor visualizar o DataFrame.
###
O próximo passo foi realizar o tratamento e a limpeza dos dados. Utilizamos o método **.info** para verificar o tipo de dados com o qual estávamos trabalhando e identificamos a existência de 35 linhas que não continham valores e a coluna "Salário Anual (R$)" que não estava no formato numérico. Realizamos a transformação dos dados, eliminamos as linhas vazias e, por fim, excluímos a coluna "Unnamed: 8", que não continha valores relevantes.
###
Em seguida, realizamos uma análise inicial e a criação dos gráficos. Utilizamos o método **.describe** para obter um resumo das informações e compreender o funcionamento da base de dados.
###
<img src="/img/describe-dados.jpg">

### Análise Exploratória:
###
- No primeiro gráfico, comparamos a origem do cliente (orgânico ou por meio de promoção) com a nota:

<img src="/img/grafico-origem.png">

Podemos observar que existe pouca diferença nas notas entre clientes provenientes de origem orgânica ou por meio de promoção.
###
- No segundo gráfico, comparamos a idade dos clientes com suas notas:

<img src="/img/grafico-idade.png">

Observamos uma queda nas notas entre pessoas abaixo de 19 anos, o que pode ser um eventual erro, uma vez que pessoas dessa idade não estariam realizando compras ou possuindo profissões.
###
- No terceiro gráfico, comparamos o salarial anual dos clientes com suas notas:

<img src="/img/grafico-salario.png">

Pela análise desse gráfico, podemos concluir que a faixa salarial não é um fator relevante, pois, apesar de haver uma nota menor na faixa de salário entre 50 a 100 mil, a diferença não é significativa em comparação com as outras faixas salariais.
###
- No quarto gráfico, comparamos a profissão dos clientes com suas notas:

<img src="/img/grafico-profissao.png">

Há uma diferença clara nas notas entre as profissões. Profissionais do entretenimento e artistas possuem notas mais elevadas, indicando que pessoas com essas profissões tendem a ter notas mais altas do que outras.
###
- No quinto gráfico, comparamos a experiência de trabalho dos clientes com suas notas:

<img src="/img/grafico-experiencia-trabalho.png">

Observamos informações relevantes, mostrando que clientes com experiência de trabalho entre 10 a 15 anos possuem notas superiores, enquanto clientes com 15 anos ou mais de experiência não apresentam notas tão interessantes.
###
- Por fim, no último gráfico, observou-se que clientes com agregado familiar maior que 7 pessoas tendem a obter notas muito baixas, fornecendo informações sobre quais clientes têm maior probabilidade de obter notas baixas.

<img src="/img/grafico-agregado-familiar.png">

### Conclusão:

Após as análises realizadas, chegamos à conclusão de que o cliente ideal para a empresa é uma pessoa com mais de 20 anos, com profissão na área de entretenimento ou arte, experiência de trabalho entre 10 a 15 anos e um agregado familiar com menos de 7 membros. A faixa salarial não demonstrou ser um fator determinante para a análise.
###
Adicionalmente, verificamos que profissionais da área de construção possuem a menor média de notas, sugerindo a possibilidade de implementar estratégias para melhorar sua satisfação e experiência com a empresa.