## instala duas bibliotecas para representações vetoriais
!pip install imgbeddings huggingface-hub==0.25.2

#importando a bliblioteca
from imgbeddings import imgbeddings

## instala duas biliotecas para manipular imagens em python e seus vetores
from PIL import Image
from numpy import asarray

# transforma nossa imagem em vetor dimensional
ibed = imgbeddings()

# carrega a imagem ##aqui foi onde carreguei as imagens no colab para demonstracao em aula##
vazia = Image.open('./vazia.png')
meio = Image.open('./meio.jpg')
transito = Image.open('./transito.jpg')

#sistema para transformar a imagem em um vetor
vazia = ibed.to_embeddings(vazia)[0]
cam1 = ibed.to_embeddings(transito)[0]
cam2= ibed.to_embeddings(meio)[0]

#importando a bliblioteca numpy e calculando a distância entre os dois valores usando algebra linear
import numpy as np

câmera = np.linalg.norm(vazia-cam2)

## demonstrando se o resultado deu muito ou pouco trânsito
(câmera > 17)*'Muito trânsito' or 'Pouco trânsito'
