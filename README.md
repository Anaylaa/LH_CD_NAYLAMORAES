# LH_CD_NAYLAMORAES

# 🎬 Previsão de Notas do IMDb

Este projeto utiliza Machine Learning para prever a **nota do IMDb** de filmes a partir de características como duração, ano de lançamento, número de votos, bilheteria, certificado, descrição do enredo e outros atributos.

O modelo utilizado é um **Random Forest Regressor**, treinado com features numéricas, categóricas e de texto (TF-IDF no campo "Overview").

---

 🚀 Tecnologias utilizadas

- [Python 3.12+](https://www.python.org/)
- [pandas](https://pandas.pydata.org/)
- [numpy](https://numpy.org/)
- [scikit-learn](https://scikit-learn.org/stable/)
- [scipy](https://scipy.org/)
- [matplotlib](https://matplotlib.org/) 
- [google colab](https://colab.google/)

  
---

## 📄 requirements.txt

```txt
pandas==2.2.2
numpy==1.26.4
scikit-learn==1.5.1
scipy==1.14.1
matplotlib==3.9.2


---

## ⚙️ Instalação

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-projeto.git
   cd seu-projeto

2. Ambiente Virtual
python -m venv .venv
source .venv/bin/activate   # Linux/Mac
.venv\Scripts\activate      # Windows

3. Instalar dependências
pip install -r requirements.txt

4. Abra o notebook e rode as células para:
Fazer o pré-processamento dos dados
Treinar o modelo
Avaliar a performance
Prever a nota IMDb para novos filmes

5. Exemplo de como usar:
   from model import predict_movie_rating

movie = {
    'Series_Title': 'The Shawshank Redemption',
    'Released_Year': '1994',
    'Certificate': 'A',
    'Runtime': '142 min',
    'Genre': 'Drama',
    'Overview': 'Two imprisoned men bond over a number of years...',
    'Meta_score': 80.0,
    'Director': 'Frank Darabont',
    'Star1': 'Tim Robbins',
    'Star2': 'Morgan Freeman',
    'Star3': 'Bob Gunton',
    'Star4': 'William Sadler',
    'No_of_Votes': 2343110,
    'Gross': '28,341,469'
}

rating = predict_movie_rating(movie)
print(f"Nota prevista do IMDb: {rating:.2f}")

   






