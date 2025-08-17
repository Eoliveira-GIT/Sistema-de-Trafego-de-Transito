# Análise de Trânsito com Representação Vetorial de Imagens

Este projeto demonstra como transformar imagens em vetores de alta dimensão usando a biblioteca **imgbeddings** e calcular a distância entre esses vetores para avaliar o nível de trânsito presente nas imagens.

## Como funciona

- **Conversão de imagens em vetores:** Através da biblioteca `imgbeddings`, cada imagem é convertida em um vetor numérico que representa suas características visuais.
- **Cálculo da distância:** Usamos a distância Euclidiana (`np.linalg.norm`) entre os vetores para medir a similaridade entre imagens. Quanto maior a distância, mais diferentes são as imagens.
- **Classificação simples:** Definimos um limiar para classificar se o trânsito está "muito" ou "pouco" presente na imagem, comparando a distância calculada.

## Tecnologias usadas

- Python 3.x
- Biblioteca [imgbeddings](https://github.com/roboflow/roboflow-python) para representação vetorial de imagens
- PIL (Python Imaging Library) para manipulação de imagens
- NumPy para cálculo matemático e álgebra linear
