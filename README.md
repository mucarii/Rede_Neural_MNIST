# Análise e Treinamento de Modelo em MNIST

## Descrição

Este projeto implementa um modelo de rede neural para classificar imagens de dígitos manuscritos usando o conjunto de dados MNIST. O modelo é construído com PyTorch e inclui etapas de carregamento de dados, pré-processamento, treinamento e validação.

## Dependências

Certifique-se de que você tenha as seguintes bibliotecas instaladas:

- `numpy`
- `torch`
- `torchvision`
- `matplotlib`

Você pode instalar as dependências necessárias usando pip:

  ```bash
  pip install numpy torch torchvision matplotlib
   ```
Estrutura do Código
Importações: As bibliotecas necessárias são importadas.
Transformações e Carregamento de Dados:
O conjunto de dados MNIST é carregado e transformado em tensores.
Dados de treinamento e validação são criados com DataLoader.
Visualização: Uma imagem de exemplo do conjunto de dados é exibida.
Definição do Modelo:
Uma classe Modelo é definida, que contém três camadas lineares com funções de ativação ReLU.
Treinamento:
A função treino é responsável por treinar o modelo em 200 épocas, calculando a perda a cada época.
Validação:
A função validacao calcula a precisão do modelo em um conjunto de dados de validação.
Como Executar
Certifique-se de que você tenha o Python e as bibliotecas necessárias instaladas.
Copie o código fornecido em um arquivo Python ou execute em um Jupyter Notebook ou Google Colab.
Execute as funções de treinamento e validação, conforme necessário:
 ```bash
  modelo = Modelo()
device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
modelo.to(device)

treino(modelo, trainloader, device)  # Inicie o treinamento
validacao(modelo, valloader, device)  # Realize a validação

   ```
Resultados
Após o treinamento, a precisão do modelo será exibida junto com a perda média por época. O modelo será capaz de classificar dígitos manuscritos do conjunto de dados MNIST.

Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.
