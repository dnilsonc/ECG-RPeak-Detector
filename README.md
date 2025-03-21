# Análise de ECG com Classificação de Batimentos Cardíacos

Este projeto realiza a análise de sinais de ECG utilizando o dataset **ECG5000**, aplicando filtragem para remoção de ruído e implementando dois modelos de classificação (**SVM** e **Random Forest**) para prever o tipo de batimento cardíaco.

## 📌 Funcionalidades
- Carregamento e visualização do dataset **ECG5000**
- Pré-processamento de sinais de ECG
- Classificação de batimentos cardíacos utilizando:
  - **SVM (Support Vector Machine)**
  - **Random Forest**
- Avaliação de desempenho com métricas de acurácia
- Comparação gráfica entre os modelos

## 🚀 Como Executar

### 1. Clone o repositório
```bash
git clone https://github.com/seu-usuario/projeto-ecg.git
cd projeto-ecg
```

### 2. Crie e ative o ambiente virtual
```bash
# Instale o virtualenv (se necessário)
pip install virtualenv

# Crie o ambiente virtual
python -m venv venv

# Ativação (Windows)
venv\Scripts\activate

# Ativação (MacOS/Linux)
source venv/bin/activate
```

### 3. Instale as dependências
```bash
pip install -r requirements.txt
```

### 4. Execute o Jupyter Notebook
```bash
jupyter notebook main.ipynb
```

## 📊 Resultados  
O projeto realiza as seguintes etapas:  

1. **Carregamento dos dados do ECG5000**  
   - Formato ARFF  
   - 5,000 amostras com 140 pontos por batimento  

2. **Pré-processamento e divisão de dados**  
   - Separação entre features (sinal ECG) e targets (classes)  
   - Divisão 80% treino / 20% teste  
   - Normalização dos dados  

3. **Treinamento dos modelos**  
   - *SVM*: Kernel linear com parâmetros padrão  
   - *Random Forest*: 100 árvores com critério Gini  

4. **Avaliação comparativa**  
   - Métrica principal: Acurácia  
   - Matriz de confusão para análise detalhada  

### Desempenho Esperado  
- **Acurácia do SVM**: `85-90%` (~85-90%)  
- **Acurácia do Random Forest**: `90-95%` (~90-95%)  
- Tempo de treinamento: SVM > Random Forest  

## 📁 Estrutura do Projeto

```bash
📂 projeto-ecg/
├── data/
│   └── 📁 ECG5000/          # Arquivos do dataset
├── 📄 main.ipynb            # Código principal
├── 📦 ECG5000.zip           # Dataset compactado
├── 📄 README.md             # Documentação
├── 📄 requirements.txt      # Dependências
└── 📁 venv/                 # Ambiente virtual
```


## 🛠️ Tecnologias Utilizadas
- **Python 3.9+**
- **Jupyter Notebook**
- **Bibliotecas**:
  - Pandas/Numpy (manipulação de dados)
  - Scikit-learn (modelos ML)
  - Matplotlib/Seaborn (visualização)
  - SciPy (processamento de sinais)
  - arff (leitura de arquivos)

## 🧩 Como Funciona
### 1. Carregamento de Dados
- Utiliza a biblioteca `arff` para ler arquivos .arff
- Extrai 5,000 amostras de ECG com 140 pontos por batimento

### 2. Pré-processamento
- Separa features (sinal de ECG) e targets (classes)
- Divisão 80/20 para treino/teste
- Normalização dos dados

### 3. Modelagem
- **SVM**: Parâmetros padrão
- **Random Forest**: 100 árvores de decisão
- Validação no conjunto de teste

### 4. Visualização
- Gráfico comparativo de acurácia
- Matriz de confusão para cada modelo

## 📚 Referências
- [ECG5000 Dataset](https://timeseriesclassification.com/description.php?Dataset=ECG5000)
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
- [SciPy Signal Processing](https://docs.scipy.org/doc/scipy/tutorial/signal.html)

## ⚡ Melhorias Futuras
- Implementar redes neurais convolucionais (CNN)
- Adicionar validação cruzada
- Desenvolver interface web para upload de ECG
- Implementar detecção de anomalias

> **Dica:** Experimente ajustar os hiperparâmetros dos modelos para melhorar a acurácia! 🔥

---

**Notas de Implementação:**  
1. Estrutura de diretórios otimizada para versionamento
2. Compatível com Python 3.9+ para garantir estabilidade
3. Dependências especificadas com versões exatas no `requirements.txt`

**Para Personalização:**
- Substituir `seu-usuario` no link de clone
- Atualizar métricas com resultados reais
- Adicionar créditos específicos do projeto