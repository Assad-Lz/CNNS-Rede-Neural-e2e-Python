# 🧠 LeNet-5: Implementação de Deep Learning com PyTorch

<p align="center">
  <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white" alt="PyTorch">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/MNIST-Data-blue?style=for-the-badge" alt="MNIST">
</p>

## 📌 Sobre o Projeto
Este repositório contém uma implementação moderna da clássica arquitetura **LeNet-5**, originalmente proposta por Yann LeCun. O objetivo é demonstrar o funcionamento de Redes Neurais Convolucionais (CNNs) aplicadas ao reconhecimento de dígitos manuscritos do dataset **MNIST**.

> [!NOTE]
> A implementação foi adaptada com técnicas modernas, utilizando **ReLU** como função de ativação e **Max Pooling** para melhor performance e convergência.

---

## 🚀 Funcionalidades Atuais
- [x] **Arquitetura LeNet-5**: Implementação completa usando PyTorch.
- [x] **Visualização de Filtros**: Inspeção dos pesos (weights) antes e depois do treinamento.
- [x] **Feature Maps**: Visualização da extração de características em tempo real.
- [x] **Pipeline de Treinamento**: Loop completo com otimizador Adam e CrossEntropyLoss.
- [x] **Análise de Erros**: Visualização detalhada das imagens onde a rede falhou.
- [x] **Checkpoint System**: Salvamento de pesos e estado do otimizador para retreino.

---

## 🏗️ Estrutura da Rede
A rede segue a lógica hierárquica para extração de padrões espaciais:

1.  **Conv1 (C1)**: 6 filtros 5x5 (Extração de bordas simples)
2.  **Max Pool1**: Redução de dimensionalidade
3.  **Conv2 (C3)**: 16 filtros 5x5 (Combinação de padrões)
4.  **Max Pool2**: Redução de dimensionalidade
5.  **Conv3 (C5)**: 120 filtros 5x5 (Características complexas)
6.  **Linear 1**: 84 neurônios
7.  **Output**: 10 classes (Dígitos de 0 a 9)

---

## 🎨 Visualizações Inclusas no Notebook
O notebook `LeNet5_Implementation.ipynb` fornece uma experiência visual rica para entender o que acontece dentro da rede:

### 🖼️ Mapas de Características
Visualize como a rede "enxerga" os números em diferentes canais após a primeira convolução.

### 🔍 Inspeção de Erros
Galeria dedicada a exibir os casos mais difíceis para a IA, facilitando o entendimento de ambiguidades nos dados.

---

## 🛠️ Como Executar
1. Instale as dependências com `uv`:
   ```bash
   uv sync
   ```
2. Abra o arquivo `LeNet5_Implementation.ipynb` em seu editor favorito.
3. Execute as células sequencialmente para ver o aprendizado em tempo real.

---

<p align="center">
Desenvolvido com ❤️ para estudos de Visão Computacional
</p>
