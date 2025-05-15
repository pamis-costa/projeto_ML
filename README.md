# **PretaLab - Inteligência Artificial - Ciclo 13**  

## **Projeto de Machine Learning - Classificação de Imagem**  

### 📌 **Sobre o Projeto**  

Este projeto foi desenvolvido durante a aula de Machine Learning do curso de Inteligência Artificial da Pretalab. O objetivo dele é aplicar técnicas avançadas para classificação de imagens, focando na identificação de rostos de mulheres pretas e de mulheres brancas.  

### 🔧 **Tecnologias Utilizadas**  
- Python → Linguagem base do projeto
- TensorFlow/Keras → Desenvolvimento dos modelos de deep learning
- OpenCV → Processamento de imagens
- Hugging Face Transformers → Modelos pré-treinados de classificação
- Pillow (PIL) → Manipulação de imagens
- NumPy → Cálculos numéricos eficientes
- Matplotlib → Visualização de dados e resultados
- Google Colab → Ambiente de execução principal

### **Como usar:**
**Instalação**
```bash
pip install torch torchvision matplotlib
```

**Execução**

1. Classificação com modelos pré-treinados:

```python
from transformers import pipeline
classifier = pipeline("image-classification", model="google/vit-base-patch16-224")
result = classifier("imagem.jpg")
```

2. Treinamento do modelo customizado:

- Organize as imagens em pastas `mulher-branca` e `mulher-preta`

- Execute o script de treinamento

- O modelo será salvo como `modelo_classificacao_racial.h5`


### 🚀 **Como Utilizar este repositório**  
1. Clone este repositório:
```bash
git clone https://github.com/pamis-costa/projeto_ML.git
```

2. Instale as dependências necessárias  
3. Execute o notebook para treinar e testar o modelo 


### 🚨 **Observações Importantes**

- Esse projeto foi desenvolvido considerando aspectos técnicos de classificação de imagens

- Para uso em produção, considere questões éticas e de privacidade, por favor!

- O desempenho do modelo depende da qualidade e quantidade dos dados de treinamento

- O código inclui exemplos tanto para execução local quanto em ambientes como Google Colab
