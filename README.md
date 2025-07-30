# 📊 Análise Estratégica de Vendas e Otimização Logística (AluraStore)

Bem-vindo ao repositório do projeto **AluraStore Analytics**! Este é um estudo aprofundado que mergulha no universo das vendas online, desvendando o desempenho das lojas e, crucialmente, o **impacto do custo do frete** na lucratividade e na logística. Nosso objetivo é transformar dados brutos em **insights acionáveis** que impulsionem a eficiência operacional e o crescimento do negócio.

---

## ✨ Destaques e Propósito da Análise

Este projeto nasceu da necessidade de otimizar a operação da AluraStore, focando em:

* **Visão 360º de Vendas:** Consolidar e pré-processar dados de múltiplas fontes para uma visão unificada e completa do faturamento, volume e comportamento de compra.
* **Performance por Loja:** Avaliar o desempenho individual de cada unidade, identificando forças e oportunidades de melhoria (faturamento, ticket médio, satisfação do cliente).
* **Mix de Produtos Otimizado:** Identificar os produtos de maior e menor desempenho para gestão estratégica de estoque e portfólio.
* **Frete: O Vilão Oculto?** Quantificar e analisar a participação do custo do frete no faturamento global e na margem de lucro.
* **Fatores do Frete:** Investigar como a loja de origem, categoria do produto e localização de entrega influenciam o custo do frete.
* **Geolocalização de Custos:** Visualizar dados de frete em um mapa interativo para identificar padrões regionais e gargalos logísticos.
* **Decisões Orientadas a Dados:** Gerar relatórios e gráficos que suportem decisões estratégicas em logística, precificação e avaliação de desempenho.

---

## 📁 Estrutura do Projeto

Nosso repositório está organizado de forma simples e intuitiva para facilitar o acesso e a compreensão:

A estrutura do repositório é simples e direta:

```
.
├── notebooks/
│   └── AluraStoreBrFinal.ipynb # O coração da análise: código completo, pré-processamento,
├── imagens                     # visualizações gráfica dos relatórios.
├── .gitignore                  # Regras para ignorar arquivos temporários e de configuração.
└── README.md                   # Este guia de projeto que você está lendo!
```
* `notebooks/AluraStoreBrFinal.ipynb`: Este é o arquivo principal onde toda a mágica acontece. Ele carrega os dados diretamente de URLs do GitHub, realiza o pré-processamento, executa análises detalhadas e gera todas as visualizações e insights textuais.
* **Nota:** Os gráficos gerados pelo notebook (Matplotlib e Folium) serão salvos no diretório raiz do projeto (ou no diretório de execução no Colab) quando o notebook for executado.

---

## 📊 Insights Chave e Visualizações

A análise detalhada no `AluraStoreBrFinal.ipynb` produz relatórios e gráficos impactantes, transformando números em narrativas.

### 📈 Desempenho Geral das Lojas

*(Ao executar o notebook, você verá gráficos detalhados de Faturamento, Avaliação Média, Volume de Vendas e Ticket Médio por Loja.)*

* **Insight:** Gráficos claros de faturamento, volume e ticket médio revelam as lojas mais e menos performáticas, crucial para alocação de recursos e definição de metas de crescimento.

### 🏷️ Desempenho por Produto

*(Visualizações como o Top 10 Produtos por Faturamento e Quantidade Vendida.)*

* **Insight:** Identificamos os produtos "estrelas" e os que precisam de atenção, auxiliando na gestão de estoque, estratégias de marketing e desenvolvimento de novos itens.

### 💰 Custo de Frete por Localização de Compra

*(Gráficos de dispersão (Scatter Plot) que mostram a relação entre coordenadas geográficas e o custo do frete.)*

* **Insight:** Pontos maiores e mais "quentes" (amarelos) indicam fretes mais caros, revelando a dispersão dos custos mesmo sem um mapa de fundo.

### 🗺️ Mapa Interativo de Frete por Localização (Folium)

*(O mapa interativo não pode ser exibido diretamente aqui, mas será renderizado de forma espetacular ao executar o notebook no Colab ou VS Code, ou pode ser salvo como um `.html`.)*

* **Insight Crucial:** A visualização em mapa é um divisor de águas! Regiões como **Roraima (RR), com um frete médio de R$ 113,67**, e **Acre (AC), com R$ 49,36**, são notavelmente mais caras para entrega. Isso destaca desafios logísticos em áreas distantes ou com infraestrutura limitada, guiando a otimização de rotas ou ajustes de estratégias de frete.

### 📝 Relatório de Análise do Impacto do Frete

* **Custo Geral:** O **custo total de frete de R$ 312.930,66 representa 5,33% do faturamento global** – uma porcentagem significativa que impacta diretamente a margem de lucro e exige atenção estratégica.
* **Frete Médio por Loja:** As diferenças são pequenas! A Loja 1 (R$ 34,69) tem o frete médio mais alto, mas a Loja 4 (R$ 31,28) não está muito atrás. Isso sugere que os custos de frete não são o principal diferencial entre as operações das lojas.
* **Frete Médio por Categoria:** **Eletrodomésticos (R$ 81,69)** e **eletrônicos (R$ 66,56)** lideram nos custos de frete, provavelmente devido ao volume e peso. Isso indica que o mix de produtos vendidos é um fator chave no custo médio do frete.

---

## 🛑 Análise para Encerramento de Operação de Loja: Uma Perspectiva Data-Driven

É importante ser **cauteloso** ao tomar decisões tão impactantes como o encerramento de uma loja. Com base nas **análises de frete fornecidas**, **não há dados suficientes para justificar o encerramento da operação de nenhuma loja neste momento**.

### Justificativa Detalhada:

* **Marginalidade do Frete:** As diferenças nos custos de frete médio entre as lojas são **mínimas**. Uma variação de pouco mais de R$ 3,00 por frete não é, por si só, um indicador forte para o fechamento de uma operação, que acarreta custos fixos, perda de base de clientes e impacto estratégico.
* **Lacuna em Métricas Financeiras:** O relatório foca em frete. Não temos acesso a métricas cruciais como **faturamento total, volume de vendas, ticket médio ou, mais importante, a *margem de lucro líquida por loja***. Sem esses dados, é impossível determinar se uma loja está, de fato, gerando prejuízo que justifique um fechamento. Uma loja com frete ligeiramente mais alto pode compensar com um volume de vendas ou uma rentabilidade geral muito maior.
* **A Necessidade de uma Análise Holística:** A decisão de encerrar uma operação de loja deve ser baseada em uma visão 360º, que inclua:
    * **Rentabilidade (Lucro Líquido) por Loja:** Qual é o verdadeiro impacto financeiro de cada unidade após *todos* os custos (incluindo frete, produto, marketing, pessoal, etc.)?
    * **Volume e Retenção de Clientes:** Uma loja pode ter uma base de clientes leal e de alto valor, mesmo com pequenos desafios logísticos.
    * **Potencial de Crescimento:** Há alguma loja em uma região com alto potencial de expansão futura, apesar das métricas atuais?
    * **Custos Fixos e Variáveis Específicos:** Existem despesas inerentes a uma loja que a tornam mais cara de operar, independentemente do frete?

Em resumo, a análise de frete é uma ferramenta poderosa para otimização logística, mas o fechamento de uma loja exige uma investigação muito mais profunda e multidisciplinar de todas as suas métricas de desempenho econômico-financeiro e estratégico.

---

## 🚀 Como Executar o Notebook e Mergulhar na Análise!

Pronto para ver a análise em ação? É super fácil!

1.  **Acesse o Google Colab:**
    * Vá para [https://colab.research.google.com/](https://colab.research.google.com/).

2.  **Abra o Notebook diretamente do GitHub:**
    * No Colab, clique em `File` > `Open notebook`.
    * Na aba `GitHub`, cole o URL deste repositório: `https://github.com/Degles/challenger_alura_store_BR` (substitua `Degles/challenger_alura_store_BR` pelo seu nome de usuário e nome real do repositório, se diferente) e pressione `Enter`.
    * Navegue até `notebooks/AluraStoreBrFinal.ipynb` e clique em `Open`.

3.  **Execute as Células em Ordem:**
    * O notebook é sequencial. Basta clicar no ícone de "Play" (o triângulo) à esquerda de cada célula ou usar `Shift + Enter` para executar uma por uma.
    * **Atenção para as instalações:** A primeira célula do notebook pode conter comandos de instalação de bibliotecas (ex: `!pip install folium`). Se a biblioteca não estiver instalada em seu ambiente Colab, **descomente (`#` remove) e execute esta linha uma única vez** para instalá-la.
    * Observe o código em ação, os outputs de texto no console e os gráficos interativos que serão gerados diretamente no notebook.

---

## 🤝 Contribuições

Sinta-se à vontade para explorar, usar e aprimorar este projeto. Sugestões e contribuições são sempre bem-vindas!

---

**Observação:** Lembre-se de substituir `Degles/challenger_alura_store_BR` (ou `SEU_USUARIO/SEU_REPOSITORIO`) no `README.md` pelo seu nome de usuário e nome real do repositório no GitHub para que o link direto para o Colab funcione corretamente.