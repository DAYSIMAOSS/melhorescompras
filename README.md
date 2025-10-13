# Análise de Centros de Distribuição — Melhores Compras (Atividade 2)

## Descrição do Projeto
Este projeto tem como objetivo determinar a melhor localização de centros de distribuição para a empresa **Melhores Compras**, utilizando **clusterização de dados geográficos** (latitude e longitude) e análise de valor de entregas.

O notebook realiza a análise da **base de dados logística fornecida**, contendo informações sobre latitude, longitude e preço das entregas, e sugere locais estratégicos para reduzir falhas de entrega e otimizar custos.

---

## Estrutura do Repositório
Atividade2/
├── assets.csv # Arquivo CSV com dados de latitude, longitude e preço
├── Atividade2_CentrosDistrib.ipynb # Notebook com todo o código
└── README.md # Este arquivo


---

## Descrição das Etapas
1. **Importação e inspeção dos dados**  
   - Carregamento do CSV em DataFrame.
   - Visualização das primeiras linhas e estatísticas descritivas.
   
2. **Limpeza e padronização**  
   - Conversão de vírgulas para ponto decimal.
   - Remoção de duplicatas e valores inválidos.
   
3. **Normalização das coordenadas**  
   - Latitude e longitude foram normalizadas usando `StandardScaler` para clusterização.

4. **Determinação do número ideal de clusters**  
   - Aplicação do método Elbow para escolher o número de centros de distribuição.

5. **Clusterização (K-Means)**  
   - Definição dos clusters.
   - Atribuição de cada entrega a um cluster.

6. **Cálculo do valor total de entregas por cluster**  
   - Soma do preço das entregas atendidas por cada centro.

7. **Visualização dos clusters**  
   - Scatter plot geográfico mostrando a distribuição dos centros de distribuição.

8. **Conclusão**  
   - Sugestão do número ideal de centros.
   - Avaliação da distribuição geográfica e do valor total das entregas.

---

## Como Executar
1. Faça upload do arquivo `assets.csv` no Colab.  
2. Abra o notebook `Atividade2_CentrosDistrib.ipynb`.  
3. Execute todas as células na ordem.  
4. Analise os gráficos do Elbow e do scatter plot para interpretar os clusters.  

---

## Tecnologias e Bibliotecas
- Python 3  
- pandas  
- scikit-learn (`KMeans`, `StandardScaler`)  
- matplotlib  
- seaborn  
- Google Colab
