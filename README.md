# Projeto 2: Segmentação de Clientes

## 📝 Introdução
Este projeto tem como objetivo segmentar clientes com base em características demográficas e comportamentais para permitir uma atuação mais direcionada e estratégica por parte da área de marketing.

Utilizamos técnicas de **Clusterização com KMeans**, precedidas de **padronização dos dados e redução de dimensionalidade com PCA**, para identificar **grupos distintos de clientes** a partir de variáveis como idade, renda, score de gastos e região.

---

## 📊 Dados

Os dados utilizados estão contidos no arquivo `segmentacao.csv` e abrangem as seguintes variáveis:

- `customer_id` — Identificador único de cada cliente  
- `age` — Idade  
- `income` — Renda anual (em milhares de dólares)  
- `spending_score` — Índice de propensão ao consumo (1 a 100)  
- `region` — Região geográfica

### Etapas realizadas:
- Análise de valores faltantes  
- Verificação de outliers  
- Transformação de variáveis categóricas em dummies  
- Padronização com `StandardScaler`  
- Redução de dimensionalidade com PCA (mantendo 95% da variância dos dados originais)  
- Clusterização com `KMeans`

---

## 🤖 Modelagem com KMeans

A clusterização foi realizada com o algoritmo **KMeans**, utilizando como entrada os dados transformados por **PCA**. A definição do número ideal de clusters foi feita com base nas seguintes métricas:

- **Método do Cotovelo**
- **Índice de Silhueta**

📌 **Número ótimo de clusters**: **4**

Cada cliente foi classificado em um dos 4 clusters, permitindo a identificação de **padrões de comportamento e perfil demográfico**.

---

## 🔍 Características dos Clusters

| Cluster | Idade média | Renda média (k$) | Spending Score médio | Comportamento                       |
|---------|-------------|------------------|-----------------------|-------------------------------------|
| 0       | 25 anos     | 30               | 80                    | Jovens com alto consumo             |
| 1       | 45 anos     | 80               | 40                    | Renda alta, consumo moderado        |
| 2       | 32 anos     | 50               | 20                    | Clientes com baixo engajamento      |
| 3       | 60 anos     | 40               | 70                    | Mais velhos com consumo recorrente  |

---

## 📈 Visualizações

- Gráficos de distribuição (histogramas e boxplots) para entender variáveis como `age`, `income`, `spending_score`
- Gráfico de dispersão dos clusters no espaço de componentes principais (PCA)
- Gráficos do **método do cotovelo** e do **índice de silhueta** para definir o número ótimo de clusters

---

## 🛠️ Ferramentas Utilizadas

- **Python** – Linguagem principal  
- **Pandas** – Manipulação de dados  
- **Matplotlib / Seaborn** – Visualizações  
- **Scikit-learn** – Pré-processamento, PCA, KMeans, métricas  
- **Google Colab** – Ambiente de desenvolvimento

---

## ✅ Resultados

- Quatro segmentos distintos de clientes foram identificados.  
- O modelo permite ações de marketing mais direcionadas para perfis específicos.  
- A clusterização revelou padrões úteis de comportamento de consumo por faixa etária, renda e região.

---

## 🧠 Conclusões

O projeto demonstra como a clusterização pode:

- **Identificar padrões ocultos** em bases de clientes  
- **Melhorar estratégias de marketing** e personalização  
- Apoiar decisões de negócios baseadas em dados

---

## 🔄 Próximos Passos

- Adicionar variáveis comportamentais (frequência de compra, canais, etc.)  
- Testar algoritmos alternativos como DBSCAN ou Hierarchical Cluster 

---

🧑‍💻 **Autor e Contato**

Higor Roberto Coutinho Caetano  
**LinkedIn**: [https://www.linkedin.com/in/higor-caetano-049521136/](https://www.linkedin.com/in/higor-caetano-049521136/)  
**E-mail**: higorfct@gmail.com
