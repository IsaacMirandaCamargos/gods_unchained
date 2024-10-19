# NFT Card Pricing for Gods Unchained Using Machine Learning

Este projeto utiliza **modelos de aprendizagem de máquina** para prever o valor das cartas NFT do jogo **Gods Unchained**. Usando dados históricos de preços e características das cartas, o modelo busca oferecer uma estimativa precisa dos preços de mercado dessas cartas, ajudando jogadores e investidores a tomar decisões informadas.

## Objetivo

O objetivo principal deste projeto é prever os preços de cartas de **Gods Unchained** no mercado NFT com base em atributos das cartas, como raridade, força e popularidade, além de dados do mercado de NFTs e criptomoedas.

## Dados Utilizados

Para construir o modelo de precificação, foram utilizados os seguintes tipos de dados:

- **Atributos das cartas**: Incluindo raridade (comum, rara, épica, lendária), mana, ataque, saúde, entre outros.
- **Preços históricos**: Preços de venda das cartas em diferentes marketplaces como **Immutable X** e **OpenSea**.
- **Tendências de mercado**: Fatores gerais do mercado de NFTs e o preço do **Ethereum**, que pode influenciar diretamente o valor das cartas.

## Modelos Utilizados

Diversos modelos de machine learning foram testados, incluindo:

- **Regressão Linear**: Para estabelecer uma base simples de comparação.
- **Random Forest**: Um modelo de ensemble para capturar relações mais complexas entre os dados.
- **XGBoost**: Um modelo de gradient boosting que apresentou o melhor desempenho entre as opções testadas.

## Como o Projeto Foi Desenvolvido

1. **Coleta de dados**: Os dados foram coletados por meio de APIs do **Immutable X** e **OpenSea**, juntamente com algumas fontes externas para análise do mercado de criptomoedas.
   
2. **Pré-processamento dos dados**: Os dados brutos foram limpos e transformados em um formato adequado para análise. Isso envolveu a normalização de atributos das cartas e a criação de novas variáveis, como médias móveis de preço e volatilidade.

3. **Treinamento do modelo**: Vários modelos foram treinados usando o conjunto de dados preparado. O desempenho foi avaliado com base em métricas como **Erro Médio Absoluto (MAE)** e **R²**.

4. **Avaliação**: O modelo **XGBoost** foi escolhido como o mais eficaz, com os melhores resultados de previsão de preço.