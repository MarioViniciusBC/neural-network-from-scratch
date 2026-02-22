# 🧠 Rede Neural Multi-Layer Perceptron (MLP) do Zero

## 📌 Sobre o Projeto
Este projeto é uma implementação educacional de uma Rede Neural Artificial construída puramente com **Python** e **NumPy**. O objetivo principal é desmistificar a "caixa preta" das bibliotecas de Machine Learning, traduzindo o cálculo e a álgebra linear do algoritmo de **Backpropagation** diretamente para o código.

A rede foi treinada para resolver o clássico **Problema da porta lógica XOR** (Ou Exclusivo), um marco histórico na Inteligência Artificial que prova a necessidade matemática de camadas ocultas (Hidden Layers) para solucionar problemas não-linearmente separáveis.

## ⚙️ Arquitetura e Implementação
Neste notebook, construí toda a arquitetura de aprendizado sem o uso de frameworks como TensorFlow ou scikit-learn. O projeto contempla:

* **Arquitetura:** 2 neurônios de entrada, 1 camada oculta com 3 neurônios e 1 neurônio de saída.
* **Função de Ativação:** Sigmoide ($y = \frac{1}{1 + e^{-x}}$).
* **Feedforward:** Multiplicação de matrizes (produto escalar) iterando sobre os registros para a propagação do sinal.
* **Backpropagation:** Aplicação da regra da cadeia para calcular os gradientes intermediários (Deltas) e mapear a "parcela de culpa" de cada neurônio no erro final.
* **Otimização:** Uso do **Gradiente Descendente em Lote (Batch Gradient Descent)** com o parâmetro de **Momento** para acelerar a convergência e evitar mínimos locais.

## 📊 Resultados e Curva de Aprendizado
O modelo foi treinado por 10.000 épocas. Graças ao acúmulo de gradientes e à taxa de aprendizagem configurada, a Média do Erro Absoluto (Função de Custo) convergiu com sucesso, provando que a rede mapeou o espaço não-linear do problema.

*(Imagem do gráfico)*

## 🛠️ Tecnologias Utilizadas
* Python 3
* NumPy (para operações matriciais vetorizadas)
* Matplotlib (para visualização de dados da Função de Custo)
* Jupyter Notebook / Google Colab

## 🚀 Como Executar
1. Clone este repositório: `git clone https://github.com/SEU_USUARIO/NOME_DO_REPO.git`
2. Instale as dependências: `pip install numpy matplotlib`
3. Execute as células do notebook sequencialmente para observar o fluxo de treinamento e a atualização manual das matrizes de peso.
