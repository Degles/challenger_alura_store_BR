# Análise de Desempenho e Logística em Vendas (AluraStore)

Este repositório contém um projeto abrangente de análise de dados com foco no desempenho de vendas de múltiplas lojas e no impacto do custo do frete. 
O objetivo é fornecer insights claros e acionáveis para otimização de operações e melhoria da lucratividade.

## 🎯 Propósito da Análise Realizada

O principal propósito desta análise é:

  * **Consolidar e pré-processar dados de vendas** de múltiplas fontes para uma visão unificada.
  * **Avaliar o desempenho geral das lojas**, incluindo faturamento, volume de vendas, ticket médio e satisfação do cliente (avaliação da compra).
  * **Identificar os produtos de maior e menor desempenho** com base em faturamento e quantidade vendida.
  * **Analisar o impacto do frete nos custos operacionais**, quantificando sua participação no faturamento global.
  * **Investigar os fatores que influenciam o custo do frete**, como a loja de origem, a categoria do produto e a localização de entrega.
  * **Visualizar dados geográficos de frete** em um mapa real para identificar padrões regionais de custos.
  * Gerar **insights estratégicos** para decisões de negócio, como otimização logística, precificação de produtos e avaliação de desempenho de lojas.

## 📁 Estrutura do Projeto e Organização dos Arquivos

A estrutura do repositório é simples e direta:

```
.
├── notebooks/
│   └── AluraStoreBr (1).ipynb  # O notebook principal com toda a análise de dados.
├── .gitignore                  # Ignora arquivos temporários e específicos do ambiente.
└── README.md                   # Este arquivo, com a descrição do projeto e instruções.
```

  * `notebooks/AluraStoreBr (1).ipynb`: Contém o código Python completo, desde o carregamento dos dados (diretamente de URLs no GitHub) até o pré-processamento,
    análise detalhada e geração de todas as visualizações e relatórios textuais.
  * Os gráficos gerados pelo notebook (Matplotlib e Folium) serão salvos no diretório raiz do projeto (ou no diretório de execução no Colab) quando o notebook for executado.

## 📊 Exemplos de Gráficos e Insights Obtidos

A análise no notebook produz uma série de relatórios textuais e gráficos que abordam diferentes dimensões do desempenho e logística:

### Desempenho Geral das Lojas (Exemplo: Faturamento por Loja)

*(Os gráficos de desempenho geral das lojas serão gerados e exibidos ao executar o notebook, como Faturamento, Avaliação Média, Volume de Vendas e Ticket Médio por Loja.)*

  * **Insight:** A análise do faturamento, volume e ticket médio por loja permite identificar as unidades de maior e menor performance em termos de receita e volume de transações, sendo essencial para alocação de recursos e definição de metas.

### Desempenho por Produto (Exemplo: Top 10 Produtos por Faturamento)

*(Gráficos de barras horizontais para Top 10 produtos por faturamento e quantidade vendida.)*

  * **Insight:** A identificação dos produtos mais lucrativos ou mais vendidos auxilia na gestão de estoque, campanhas de marketing e desenvolvimento de novos produtos.

### Custo de Frete por Localização de Compra (Exemplo: Scatter Plot Matplotlib)

  * **Insight:** O scatter plot sem mapa de fundo já indica a dispersão dos custos de frete por coordenadas. Áreas com pontos maiores e mais quentes (amarelos) representam fretes mais caros.

### Mapa Interativo de Frete por Localização (Folium)

*(O mapa interativo em HTML não pode ser exibido diretamente no README, mas ao executar o notebook, ele será renderizado interativamente no Colab ou pode ser salvo como um arquivo `.html`.)*

  * **Insight:** A visualização do custo de frete sobre um mapa real é crucial. Ela revela que regiões como **Roraima (RR), com um frete médio de R$ 113,67**, e **Acre (AC), com R$ 49,36**, são significativamente mais caras para entregas, apontando para desafios logísticos em áreas mais distantes ou com infraestrutura limitada. Essas informações são valiosas para a otimização de rotas ou ajustes de estratégias de frete para essas localidades.

### Relatório de Análise do Impacto do Frete

  * **Insight Geral do Frete:** O **custo total de frete de R$ 312.930,66 representa 5,33% do faturamento global**, uma porcentagem que exige atenção, pois afeta diretamente a margem de lucro.
  * **Frete Médio por Loja:** A **Loja 1 tem o frete médio mais alto (R$ 34,69)**, mas a diferença entre as lojas é marginal (Loja 4 com R$ 31,28). Isso sugere que os custos de frete não são drasticamente diferentes entre as operações das lojas.
  * **Frete Médio por Categoria de Produto:** **Eletrodomésticos (R$ 81,69)** e **eletrônicos (R$ 66,56)** são as categorias com fretes mais altos, provavelmente devido ao volume/peso. Isso indica que a composição do mix de vendas pode influenciar o custo médio do frete.

## 🚀 Como Executar o Notebook

Para executar a análise completa e visualizar todos os gráficos e relatórios:

1.  **Acesse o Google Colab:**
      * Vá para [https://colab.research.google.com/](https://colab.research.google.com/).
2.  **Abra o Notebook no Colab:**
      * Clique em `File` \> `Open notebook`.
      * Na aba `GitHub`, cole o URL deste repositório (ex: `https://github.com/SEU_USUARIO/SEU_REPOSITORIO/`) e pressione `Enter`.
      * Selecione o arquivo `notebooks/AluraStoreBr (1).ipynb` e clique em `Open`.
3.  **Execute as Células em Ordem:**
      * O notebook está estruturado em células. Execute cada célula sequencialmente, clicando no ícone de "Play" (triângulo) à esquerda de cada célula ou pressionando `Shift + Enter`.
      * **Atenção para a instalação de bibliotecas:** A primeira célula do notebook pode conter uma linha comentada como `!pip install folium`. Se a biblioteca não estiver instalada em seu ambiente Colab, **descomente e execute esta linha uma única vez** para instalá-la.
      * Observe os outputs de texto no console e os gráficos que serão gerados e exibidos diretamente no notebook.

## ⛔ Análise para Encerramento de Operação de Loja

Com base nas análises apresentadas no relatório, **não há dados suficientes para justificar o encerramento da operação de nenhuma loja neste momento**.

**Justificativa fundamentada em dados (do relatório disponível):**

  * **Frete Médio por Loja:** As diferenças nos custos de frete médio entre as lojas são **marginais**. A Loja 1 tem o maior frete médio (R$ 34,69), enquanto a Loja 4 tem o menor (R$ 31,28). Uma variação de pouco mais de R$ 3,00 por frete não é, por si só, um indicador forte o suficiente para o encerramento de uma operação, que envolve custos fixos, base de clientes, e impacto estratégico.
  * **Ausência de Métricas de Desempenho Financeiro Comparativo:** O relatório fornecido não detalha métricas cruciais como o **faturamento total, volume de vendas, ticket médio ou margem de lucro por loja**. Sem esses dados, é impossível determinar se uma loja está, de fato, performando abaixo do esperado ou gerando prejuízo que justifique seu fechamento. Uma loja pode ter um frete médio ligeiramente mais alto, mas compensar isso com um volume de vendas ou faturamento significativamente maior, tornando-a valiosa para o negócio.
  * **Necessidade de Análise Holística:** A decisão de encerrar a operação de uma loja deve ser baseada em uma análise holística que considere múltiplos fatores financeiros e operacionais, como:
      * **Rentabilidade (Lucro Líquido) por Loja:** Qual loja está gerando mais ou menos lucro após todos os custos (incluindo frete, mas também custos de produto, marketing, pessoal, etc.)?
      * **Volume de Clientes e Retenção:** Uma loja com frete ligeiramente mais alto pode ter uma base de clientes leal e de alto valor.
      * **Crescimento Potencial:** Alguma loja está em uma região com alto potencial de crescimento futuro, apesar dos desafios atuais?
      * **Custos Fixos e Variáveis Específicos da Loja:** Existem despesas que tornam uma loja intrinsecamente mais cara de operar, independentemente do frete?

Em suma, o relatório de frete é um excelente ponto de partida para otimização logística, mas a decisão de fechar uma loja exige uma investigação mais aprofundada de todas as suas métricas de desempenho econômico-financeiro e estratégico.

-----

**Observação:** Lembre-se de substituir `SEU_USUARIO/SEU_REPOSITORIO` no `README.md` pelo seu nome de usuário e nome real do repositório no GitHub.
