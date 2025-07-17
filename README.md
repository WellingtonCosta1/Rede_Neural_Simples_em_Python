
# Algoritmo de Rede Neural Simples em Python

Este projeto implementa uma rede neural binária básica **sem uso de frameworks de Machine Learning como TensorFlow ou PyTorch**. A ideia é entender o funcionamento interno do treinamento de um modelo de classificação usando **regressão logística** e **função de ativação sigmóide** com o `NumPy`.

---

## 🧠 Objetivo

Prever se uma transação é ou não suspeita com base em dois atributos (ex: número de compras e valor da compra).

---

## ⚙️ Funcionalidades

- Implementação de uma rede neural de 1 camada com:
  - Inicialização de pesos e bias
  - Forward pass com função de ativação sigmóide
  - Cálculo de erro
  - Atualização dos pesos (backpropagation)
- Treinamento e avaliação do modelo
- Previsões com novos dados
- Código dividido em partes:
  - Definição da classe
  - Treinamento
  - Avaliação
  - Deploy

---

## 📦 Dependências

- Python 3.6+
- NumPy

Instale com:

```bash
pip install numpy

# Dados de treino
X_treino = np.array([[1, 2.5], [2, 3], [3, 5], [1, 4], [5, 6], [6, 7]])
y_treino = np.array([0, 0, 1, 0, 1, 1])

# Instanciando e treinando o modelo
modelo = AlgoritmoNeuralNetwork(taxa_aprendizado=0.01, num_iteracoes=1000)
modelo.fit(X_treino, y_treino)

# Dados de teste
X_teste = np.array([[1.5, 2], [4, 5.5]])
modelo.predict(X_teste)

├── algoritmo_rede_neural.py  # Código principal
├── README.md

