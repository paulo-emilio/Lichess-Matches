# Análise de Partidas de Xadrez (Lichess)

## Visão Geral
Este projeto realiza a limpeza e análise de dados de partidas de xadrez coletadas do site Lichess.org. O objetivo é explorar as características das partidas e identificar os fatores chave que influenciam os resultados dos jogos, com foco em entender as relações entre as classificações dos jogadores, o tempo de jogo e as decisões estratégicas.

![Chess](figures/chess.png)  <!-- Adicione uma imagem relevante do seu projeto aqui -->

## Tecnologias Utilizadas
- Python
- Jupyter Notebook
- Pandas, NumPy
- Matplotlib, Plotly

## Dataset
### Fonte
- [Kaggle: Lichess Dataset](https://www.kaggle.com/datasets/datasnaek/chess/data)

### Descrição dos Dados
O dataset contém aproximadamente 20.000 partidas de xadrez com as seguintes características:

- `id`: ID da Partida
- `rated`: Partida Ranqueada (Sim/Não)
- `created_at`: Hora de Início
- `last_move_at`: Hora de Término
- `turns`: Número de Movimentos
- `victory_status`: Status da Partida
- `winner`: Vencedor
- `increment_code`: Incremento de Tempo
- `white_id`: ID do Jogador Branco
- `white_rating`: Rating do Jogador Branco
- `black_id`: ID do Jogador Preto
- `black_rating`: Rating do Jogador Preto
- `moves`: Todos os Movimentos em Notação Padrão de Xadrez
- `opening_eco`: ECO da Abertura (Código Padronizado para cada abertura)
- `opening_name`: Nome da Abertura
- `opening_ply`: Número de Movimentos na Fase de Abertura

## Estrutura do Projeto
1. **Importação de Bibliotecas**: Importação das bibliotecas necessárias para o projeto.
2. **Carregamento e Visualização dos Dados**: Leitura do dataset e visualização inicial dos dados.
3. **Pré-processamento dos Dados**: Limpeza e preparação dos dados para análise.
4. **Análise Exploratória dos Dados (EDA)**: Análise gráfica e estatística das características dos dados.

## Notebooks
### 1. Limpeza de Dados (`1-data_cleaning.ipynb`)
- **Objetivo**: Limpar e preparar os dados para a análise.
- **Principais Tarefas**:
  - Importação das bibliotecas necessárias.
  - Carregamento e visualização inicial dos dados.
  - Limpeza e tratamento dos dados ausentes ou inconsistentes.

### 2. Análise Exploratória (`2-eda.ipynb`)
- **Objetivo**: Explorar os dados limpos e identificar padrões e insights.
- **Principais Tarefas**:
  - Análise gráfica e estatística das características dos dados.
  - Identificação dos fatores que influenciam os resultados das partidas.

## Insights Importantes
Aqui estão alguns insights importantes obtidos a partir da análise exploratória dos dados:

1. **Movimentos**: O número de movimentos pode indicar a complexidade da partida.
2. **Rating dos Jogadores**: A diferença de rating entre os jogadores influencia fortemente o resultado da partida.
3. **Aberturas**: Certas aberturas podem ter uma maior taxa de sucesso dependendo do rating dos jogadores.
4. **Tempo de Jogo**: Partidas com diferentes incrementos de tempo podem ter dinâmicas e resultados variados.

### Distribuição dos Movimentos

![Histograma Movimentos](figures/hist_movimentos.png)

### Impacto do Rating no Resultado

![Rating](figures/rating.png)

### Aberturas mais Comuns

![Aberturas](figures/aberturas.png)

## Como Utilizar
### Notebook de Limpeza de Dados
1. Abra o notebook "1-data_cleaning.ipynb".
2. Execute todas as células do notebook para realizar a limpeza e preparação dos dados.

### Notebook de Análise Exploratória
1. Abra o notebook "2-eda.ipynb".
2. Execute todas as células do notebook para realizar a análise exploratória dos dados e obter insights.

## Contribuições
Contribuições são bem-vindas! Se você encontrar algum problema ou tiver sugestões para melhorias, sinta-se à vontade para abrir uma issue ou enviar um pull request.
