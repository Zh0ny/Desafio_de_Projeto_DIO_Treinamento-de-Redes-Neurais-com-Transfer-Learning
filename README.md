# Desafio_de_Projeto_DIO_Treinamento-de-Redes-Neurais-com-Transfer-Learning
Desafio de Projeto: Treinamento de Redes Neurais com Transfer Learning - BOOTCAMP BairesDev - Machine Learning Practitioner.

# Classificação de Imagens com Transfer Learning e Fine-tuning

Este projeto demonstra como usar Transfer Learning para criar um classificador de imagens com Keras, usando o modelo VGG16 pré-treinado. O objetivo é classificar imagens em duas classes: 'coruja_da_igreja' e 'arara_caninde'.


## Descrição

O código realiza as seguintes etapas:

1. **Carregamento e Pré-processamento de Dados:**
   - Carrega imagens de duas pastas: 'coruja_da_igreja_dataset_augmented' e 'Arara_caninde_dataset_augmented'.
   - Divide os dados em conjuntos de treinamento, validação e teste.
   - Pré-processa as imagens para o formato necessário para o modelo VGG16.

2. **Treinamento de um Modelo Base:**
   - Cria e treina um modelo de rede neural convolucional (CNN) simples do zero como linha de base.
   - Avalia o desempenho do modelo base.

3. **Transfer Learning com VGG16:**
   - Carrega o modelo VGG16 pré-treinado com pesos do ImageNet.
   - Remove a última camada de classificação do VGG16 e adiciona uma nova camada para as duas classes alvo.
   - Congela os pesos das camadas do VGG16 para usar como extrator de recursos.
   - Treina o modelo com os novos dados, ajustando apenas os pesos da nova camada de classificação.

4. **Avaliação e Previsão:**
   - Avalia o desempenho do modelo com Transfer Learning no conjunto de teste.
   - Demonstra como usar o modelo para prever a classe de uma nova imagem.

5. **Conjunto de Dados:"
   - Foram utilizadas 2 classes: Arara Canindé e Coruja da Igreja.
   - Cada Classe contém 100 imagens com licença creative commons.
   - Esse conjunto de dados utiliza técnicas de data augmentation.
   - Link para download: https://drive.google.com/drive/folders/1xq0g7YDThdUgcDaUpjTmQB1hOyDEycQK?usp=sharing

## Dependências

- Python 3.x
- TensorFlow/Keras
- NumPy
- Matplotlib
- Google Colab
- ZipFile
