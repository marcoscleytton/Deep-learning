#  Classificação de Imagens com Keras

##  Descrição

Este projeto demonstra como utilizar um modelo treinado com **Keras (TensorFlow)** para realizar **classificação de imagens**. A aplicação carrega um modelo `.h5`, processa uma imagem de entrada, realiza a predição e retorna a **classe prevista** com sua **pontuação de confiança**.

---

##  Tecnologias Utilizadas

- [TensorFlow / Keras](https://www.tensorflow.org/)
- [Pillow (PIL)](https://pillow.readthedocs.io/)
- [NumPy](https://numpy.org/)

---

## 📂 Estrutura Esperada

- `keras_Model.h5` → modelo treinado salvo.  
- `labels.txt` → arquivo com os nomes das classes, uma por linha.  
- Imagem de entrada (substituir o caminho no código).  

---

##  Etapas do Código

1. **Importação das bibliotecas necessárias**
2. **Carregamento do modelo treinado (`keras_Model.h5`)**
3. **Leitura dos rótulos das classes (`labels.txt`)**
4. **Pré-processamento da imagem:**
   - Redimensionamento para 224x224 pixels
   - Conversão para RGB
   - Normalização dos valores de pixel
5. **Predição com o modelo**
6. **Exibição da classe prevista e pontuação de confiança**

---

##  Exemplo de Uso

```python
# Substitua pelo caminho da sua imagem
image = Image.open("caminho/para/sua/imagem.jpg").convert("RGB")
