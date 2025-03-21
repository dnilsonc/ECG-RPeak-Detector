# Análise de ECG com Detecção de Picos R e Classificação

Este projeto realiza a análise de sinais de ECG utilizando o dataset MIT-BIH, aplicando filtragem para remoção de ruído, detecção de picos R e uma classificação simples utilizando um Random Forest.

## 📌 Funcionalidades
- Download e visualização do sinal de ECG
- Filtragem passa-baixa para remoção de ruído
- Detecção automática de picos R
- Classificação básica de batimentos cardíacos

## 🚀 Como Executar
1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```
2. Instale as dependências:
   ```bash
   pip install wfdb numpy matplotlib scipy scikit-learn
   ```
3. Execute o script principal:
   ```bash
   python ecg_analysis.py
   ```

## 📊 Resultados
O projeto gera um gráfico do sinal de ECG com os picos R detectados e exibe a acurácia do modelo de classificação.

## 📁 Estrutura do Projeto
```
📂 projeto-ecg
 ├── ecg_analysis.py  # Código principal
 ├── README.md        # Documentação do projeto
 ├── requirements.txt # Dependências
```

## 📚 Referências
- [MIT-BIH Arrhythmia Database](https://physionet.org/content/mitdb/1.0.0/)
- [SciPy - Signal Processing](https://docs.scipy.org/doc/scipy/reference/signal.html)

---
⚡ **Dica:** Este projeto pode ser expandido com redes neurais para detecção de arritmias! 🔥

