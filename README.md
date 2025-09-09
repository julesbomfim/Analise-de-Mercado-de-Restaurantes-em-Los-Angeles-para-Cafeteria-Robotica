# Análise de Mercado de Restaurantes em Los Angeles para Cafeteria Robótica

Este repositório contém uma análise de mercado detalhada do setor de restaurantes em Los Angeles. O projeto foi desenvolvido para fundamentar a decisão de abrir uma cafeteria com garçons robôs e para preparar uma apresentação convincente para potenciais investidores, destacando as oportunidades e a viabilidade do negócio.

## 📄 Contexto do Projeto

A proposta é abrir uma cafeteria inovadora em Los Angeles, utilizando garçons robôs para criar uma experiência única. Sendo um projeto de alto investimento, é crucial analisar o mercado atual para entender a concorrência, identificar nichos e definir a melhor estratégia de entrada. Esta pesquisa de mercado, baseada em dados de código aberto, visa responder a perguntas chave sobre o cenário gastronômico da cidade para validar o plano de negócios.

## 🗂️ Conjunto de Dados

A análise utiliza o arquivo `/datasets/rest_data_us_upd.csv`, que contém dados sobre estabelecimentos de alimentação em Los Angeles. As colunas principais são:

-   `object_name`: Nome do estabelecimento.
-   `chain`: Indica se o estabelecimento pertence a uma rede (True/False).
-   `object_type`: Tipo de estabelecimento (ex: Restaurant, Cafe, Fast Food).
-   `address`: Endereço completo.
-   `number`: Número de assentos.

## 🎯 Objetivos da Análise

A pesquisa foi guiada para responder às seguintes questões de negócio:

1.  Qual a proporção dos diferentes tipos de estabelecimentos em LA?
2.  Qual a divisão do mercado entre estabelecimentos de rede e independentes?
3.  Quais as características típicas dos estabelecimentos de rede (tipo, tamanho, capacidade)?
4.  Qual o número médio de assentos por tipo de estabelecimento?
5.  Quais ruas possuem a maior concentração de restaurantes e qual a sua capacidade média?
6.  Existem oportunidades em ruas com menor densidade de estabelecimentos?

## 🛠️ Metodologia e Etapas da Análise

O projeto foi estruturado nas seguintes etapas:

### Passo 1: Carga e Preparação dos Dados
-   Carregamento do conjunto de dados utilizando a biblioteca Pandas.
-   Verificação e correção dos tipos de dados, com foco na coluna `chain`.
-   Tratamento de valores ausentes e verificação de duplicatas para garantir a qualidade dos dados.

### Passo 2: Análise Exploratória de Dados (EDA)
-   **Análise de Proporções**: Investigação da distribuição de tipos de estabelecimentos e da proporção entre redes e não redes, utilizando gráficos de barras e de pizza.
-   **Análise de Redes**: Análise aprofundada para identificar os tipos de estabelecimentos mais comuns em redes e a distribuição do número de assentos, comparando redes com estabelecimentos independentes através de boxplots.
-   **Análise de Capacidade**: Cálculo do número médio de assentos para cada tipo de estabelecimento para identificar os portes mais comuns.
-   **Análise de Localização**:
    -   Extração dos nomes das ruas da coluna `address`.
    -   Identificação das 10 ruas com maior número de restaurantes.
    -   Quantificação do número de ruas que possuem apenas um estabelecimento.
    -   Análise da distribuição de assentos nas ruas mais movimentadas.

### Passo 3: Conclusão e Apresentação
-   Consolidação dos insights em uma conclusão geral, com recomendações sobre o tipo de estabelecimento, número de assentos e estratégia de expansão.
-   Criação de uma apresentação em formato PDF para compartilhar os resultados com os investidores.

## 📈 Conclusões Principais e Recomendações

-   **Oportunidade de Mercado**: O mercado de LA é dominado por estabelecimentos independentes (**61,9%**), o que indica uma forte aceitação para conceitos únicos e inovadores, como uma cafeteria robótica.
-   **Tipo de Estabelecimento**: O formato de **Café** é uma escolha estratégica. Embora "Restaurant" seja a categoria mais numerosa, os cafés possuem um porte médio menor (média de 25 assentos), o que representa um investimento inicial mais baixo e menor risco.
-   **Estratégia de Localização**: Existe uma alta saturação em grandes avenidas como a Sunset Blvd. No entanto, a análise revelou que **2.450 ruas** possuem apenas um restaurante, representando uma grande oportunidade para se estabelecer em áreas com menor concorrência direta.
-   **Capacidade Ideal**: Recomenda-se um estabelecimento com **25 a 40 assentos**. Este porte está alinhado com a média para cafés, mas oferece uma capacidade ligeiramente superior para acomodar o fluxo gerado pela novidade dos robôs.
-   **Potencial de Rede**: O potencial para se tornar uma rede é viável, dado que este é um modelo comum em LA. No entanto, a recomendação inicial é focar em uma única loja-conceito para validar o modelo de negócio antes de planejar a expansão.

## 📊 Apresentação para Investidores

A apresentação com a síntese dos resultados da pesquisa pode ser acessada no link abaixo:

[Link para a Apresentação em PDF](https://docs.google.com/document/d/1SCGGBO_A32PO6Bsuuzip3Omj4a0YIz1mdT4jrPdO_ec/edit?usp=sharing)

## 💻 Tecnologias Utilizadas
-   Python 3
-   Pandas
-   Matplotlib
-   Seaborn
-   Jupyter Notebook
