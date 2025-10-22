# 🧠 Comparação de Arquiteturas CNN no Dataset Fashion-MNIST

## 🎯 Objetivo
O objetivo deste projeto é **comparar duas arquiteturas diferentes de Redes Neurais Convolucionais (CNNs)** na tarefa de **classificação de imagens de roupas** utilizando o dataset **Fashion-MNIST**.  
A proposta busca analisar o impacto da profundidade da rede no desempenho do modelo, considerando acurácia, tempo de treinamento e capacidade de generalização.

---

## 🧩 Arquiteturas Implementadas

### 🧱 CNN Shallow (Rasa)
- **Descrição:** Modelo com **apenas uma camada convolucional**, porém mais larga.
- **Propósito:** Captar **padrões simples e locais** nas imagens, como bordas e linhas.
- **Camadas Principais:**
  - Conv2D (filtros amplos)
  - MaxPooling2D
  - Flatten
  - Dense (camada totalmente conectada)
  - Dropout (para evitar overfitting)

### 🏗️ CNN Deep (Profunda)
- **Descrição:** Modelo com **quatro camadas convolucionais**, tornando-se mais especializado.
- **Propósito:** Aprender **padrões hierárquicos e complexos**, como texturas, partes e objetos completos.
- **Camadas Principais:**
  - Múltiplas Conv2D + MaxPooling2D
  - Flatten
  - Dense
  - Dropout

---

## 📦 Dataset
**Fashion-MNIST**  
- Contém **70.000 imagens em tons de cinza (28x28 pixels)** de roupas e acessórios.
- **10 classes**: camiseta, calça, pulôver, vestido, casaco, sandália, camisa, tênis, bolsa e bota.
- O dataset é dividido em:
  - 60.000 imagens para treinamento  
  - 10.000 imagens para teste

---

## ⚙️ Tecnologias Utilizadas
- **Python 3.10+**
- **TensorFlow / Keras**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **time** (para medição de desempenho)

---

## 🚀 Execução do Projeto

### Pré-requisitos
Certifique-se de ter as bibliotecas instaladas:
```bash
pip install tensorflow numpy matplotlib seaborn
```

### Passos para execução
1. Abra o notebook `projeto2_Juliano_Joao_Felizardo.ipynb`.
2. Execute as células na ordem:
   - Importação das bibliotecas
   - Carregamento e normalização dos dados
   - Definição e compilação dos modelos (Shallow e Deep)
   - Treinamento e validação
   - Avaliação e comparação dos resultados
3. Observe os resultados impressos e os gráficos de acurácia, perda e tempo de execução.

---

## 📊 Resultados Obtidos

| Modelo       | Acurácia de Teste | Tempo de Treinamento (s) | Observações |
|---------------|-------------------|---------------------------|--------------|
| CNN Shallow   | 0.9151              | 34.91                        | Mais rápida, mas menos precisa |
| CNN Deep      | 0.9238             | 73.40                       | Melhor desempenho geral |

---

## 🧠 Conclusão
- A **CNN Shallow** apresentou bom desempenho para tarefas simples, com treinamento rápido.  
- A **CNN Deep** obteve **maior acurácia e melhor generalização**, embora com maior custo computacional.  
- O estudo demonstra como **a profundidade da rede influencia na capacidade de aprendizado** de padrões mais complexos.

---

## 👨‍💻 Autores
**João Victor de Mendonça Felizardo Silva**

**Juliano**

