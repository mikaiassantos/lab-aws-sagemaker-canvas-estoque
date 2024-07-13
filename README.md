# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Bem-vindo ao desafio de projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas". Neste Lab DIO, você aprenderá a usar o SageMaker Canvas para criar previsões de estoque baseadas em Machine Learning (ML). Siga os passos abaixo para completar o desafio!

## 📋 Pré-requisitos

Antes de começar, certifique-se de ter uma conta na AWS. Se precisar de ajuda para criar sua conta, confira nosso repositório [AWS Cloud Quickstart](https://github.com/digitalinnovationone/aws-cloud-quickstart).

## 🎯 Objetivos Deste Desafio de Projeto (Lab)

![image](https://github.com/digitalinnovationone/lab-aws-sagemaker-canvas-estoque/assets/730492/72f5c21f-5562-491e-aa42-2885a3184650)

- Dê um fork neste projeto e reescreva este `README.md`. Sinta-se à vontade para detalhar todo o processo de criação do seu Modelo de ML para uma "Previsão de Estoque Inteligente".
- Para isso, siga o passo a passo descrito a seguir e evolua as suas habilidades em ML no-code com o Amazon SageMaker Canvas.
- Ao concluir, envie a URL do seu repositório com a solução na plataforma da DIO.

## 🚀 Passo a Passo

### 1. Selecionar Dataset

- Navegue até a pasta `datasets` deste repositório. Esta pasta contém os datasets que você poderá escolher para treinar e testar seu modelo de ML. Sinta-se à vontade para gerar/enriquecer seus próprios datasets, quanto mais você se engajar, mais relevante esse projeto será em seu portfólio.
- Escolha o dataset que você usará para treinar seu modelo de previsão de estoque.
- Faça o upload do dataset no SageMaker Canvas.

### 2. Construir/Treinar

- No SageMaker Canvas, importe o dataset que você selecionou.
- Configure as variáveis de entrada e saída de acordo com os dados.
- Inicie o treinamento do modelo. Isso pode levar algum tempo, dependendo do tamanho do dataset.

### 3. Analisar

- Após o treinamento, examine as métricas de performance do modelo.
- Verifique as principais características que influenciam as previsões.
- Faça ajustes no modelo se necessário e re-treine até obter um desempenho satisfatório.

### 4. Prever

- Use o modelo treinado para fazer previsões de estoque.
- Exporte os resultados e analise as previsões geradas.
- Documente suas conclusões e qualquer insight obtido a partir das previsões.

## 📊 Documentação das Conclusões e Insights

### Dataset Utilizado

Para este projeto, utilizei um dataset contendo 1000 registros com as seguintes colunas:
- `id_produto`: Identificação única do produto.
- `quantidade_estoque`: Quantidade de estoque do produto.
- `preco`: Preço do produto.
- `promocao`: Indicador de promoção (sim/não).
- `data_evento`: Data do evento de estoque.

### Principais Conclusões

1. **Previsão da Quantidade de Estoque**:
   - **Desempenho do Modelo**: O modelo apresentou um bom desempenho na previsão da quantidade de estoque, com uma precisão aceitável para a maioria dos produtos.
   - **Variáveis Influenciadoras**: As variáveis `preco` e `promocao` foram identificadas como influenciadores significativos nas previsões de estoque. Produtos em promoção tendem a ter um aumento na demanda, impactando diretamente a quantidade de estoque.
   - **Sazonalidade**: A `data_evento` ajudou a identificar padrões sazonais na demanda por certos produtos, permitindo ajustes mais precisos no planejamento de estoque.

2. **Ajustes e Re-treinamento**:
   - **Melhoria Contínua**: Baseado nas primeiras previsões, foram feitos ajustes nos dados de entrada, como normalização dos preços e inclusão de novos dados históricos. Isso resultou em uma melhoria significativa na precisão do modelo.

### Insights Obtidos

- **Promoções e Preços**: A promoção tem um impacto claro no aumento da demanda, sugerindo que estratégias de marketing e preços dinâmicos podem ser eficazes para otimizar os níveis de estoque.
- **Planejamento Sazonal**: Identificar e ajustar para a sazonalidade é crucial para evitar excesso ou falta de estoque durante diferentes períodos do ano.
- **Gestão Proativa de Estoque**: Com as previsões de quantidade de estoque, é possível implementar uma gestão proativa de reabastecimento, evitando rupturas de estoque e minimizando custos de armazenamento.
