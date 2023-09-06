# Análise de Perfil de Clientes

###
[![License: MIT](https://img.shields.io/badge/License-MIT-black.svg)](https://opensource.org/licenses/MIT) 

### Sobre:

Análise da base de dados em busca de identificar o perfil de cliente.

### Proposta:

Com informações extraídas de uma base de dados em formato **.csv**, será realizada uma análise de perfil, levando em consideração as informações que mais impactam na nota dos clientes.
###
Será feita uma análise com o objetivo de identificar os principais fatores que influenciam na nota dos clientes.
###
A solução final consistirá em um conjunto de gráficos, a partir dos quais serão extraídos insights baseados nessas análises.

### Estrutura do Repositório:
- <strong>data:</strong> Encontrará o arquivo **.csv** com os dados utilizados para a análise.
- <strong>img:</strong> Aqui será encontrado os prints obtidos na análise.
- <strong>notebook:</strong> Este diretório contém o notebook Jupyter onde a análise foi realizada e os resultados obtidos.
- <strong>readme_translated:</strong> This repository contains the **PDF** with the **report** translated into English.

### Linguagem Utilizada:
###
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=white&color=black)

### Bibliotecas Utilizadas:
###
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white&color=black) 	![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white&color=black)

### Metodologia:

Inicialmente, utilizamos a biblioteca **Pandas** para importar e ler a base de dados. Enfrentamos um problema de encoding, pois a base de dados contia algum caractere especial e ou acentuação, então resolvemos o problema utilizando a propriedade **encoding='latin'** e a propriedade **sep=';'** para organizar e melhor visualizar o DataFrame.
###
<img src="/img/dados.jpg">

###
O próximo passo foi realizar o tratamento e a limpeza dos dados. Utilizamos o método **.info** para verificar o tipo de dados com o qual estávamos trabalhando e identificamos a existência de **35 linhas** que continham valores nulos e a coluna **"Salário Anual (R$)"** que não estava no formato numérico. Realizamos a transformação dos dados, excluímos a coluna **"Unnamed: 8"** e por fim **eliminamos as linhas vazias**, que não continha valores relevantes.
###
<img src="/img/dados-info.jpg">

###
Em seguida, realizamos uma análise inicial e a criação dos gráficos. Utilizamos o método **.describe** para obter um resumo das informações e compreender o funcionamento da base de dados. Para a criação dos gráficos foi utilizado a biblioteca **Plotly** com o método de repetição **for**.
###
<img src="/img/describe-dados.jpg">

###
Tomaremos como base para a análise a nota média observada, que foi de **52**.

### Análise:
###
- No primeiro gráfico, comparamos a origem do cliente (orgânico ou por meio de promoção) com a nota:

<img src="/img/grafico-origem.png">

Podemos observar que existe pouca diferença nas notas entre clientes provenientes de origem orgânica ou por meio de promoção.
###
- No segundo gráfico, comparamos a idade dos clientes com suas notas:

<img src="/img/grafico-idade.png">

Observamos uma queda nas notas entre pessoas abaixo de 20 anos.
###
- No terceiro gráfico, comparamos o salarial anual dos clientes com suas notas:

<img src="/img/grafico-salario.png">

Pela análise desse gráfico, podemos concluir que a faixa salarial não é um fator relevante, pois, apesar de haver uma nota menor na faixa de salário entre 50 a 100 mil e acima de 150 mil, a diferença não é significativa em comparação com as outras faixas salariais.
###
- No quarto gráfico, comparamos a profissão dos clientes com suas notas:

<img src="/img/grafico-profissao.png">

Há uma diferença clara nas notas entre as profissões. Profissionais do entretenimento e artistas possuem notas mais elevadas, indicando que pessoas com essas profissões tendem a ter notas mais altas do que outras.
###
- No quinto gráfico, comparamos a experiência de trabalho dos clientes com suas notas:

<img src="/img/grafico-experiencia-trabalho.png">

Observamos informações relevantes, mostrando que clientes com experiência de trabalho entre 10 a 15 anos possuem notas superiores.
###
- Por fim, no último gráfico, observou-se que clientes com agregado familiar maior que 7 pessoas tendem a obter notas muito baixas, fornecendo informações sobre quais clientes têm maior probabilidade de obter notas baixas.

<img src="/img/grafico-agregado-familiar.png">

### Conclusão:

Após as análises realizadas, chegamos à conclusão de que o perfil de cliente é acima dos 20 anos, com profissão na área de entretenimento ou arte, experiência de trabalho entre 10 a 15 anos e um agregado familiar com menos de 7 membros. A origem do cliente e a faixa salarial não demonstrou ser um fator determinante para a análise.
###
Adicionalmente, verificamos que profissionais da área de construção e famílias com mais de 7 pessoas possuem a menor média de notas.
###

---
### Contato:

<div>
  <a href="https://linkedin.com/in/marcospontesjunior" target="_blank"><img src="https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white&color=black" target="_blank"></a>  
  <a href = "mailto:marcospntsjunior@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white&color=black" target="_blank"></a>
</div>
