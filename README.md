# Análise de Livros em Tendência e Avaliações de Clientes 📈📖

Este projeto utiliza **Streamlit**, **Pandas** e **Plotly** para criar uma interface web interativa que permite visualizar e analisar os livros em tendência e suas respectivas avaliações.

## Funcionalidades

- Exibição interativa dos 100 livros mais populares.
- Controle de faixa de preço para filtragem dos livros exibidos.
- Visualização gráfica da quantidade de livros por ano de publicação.
- Distribuição dos preços dos livros por meio de um histograma.

## Como o código funciona

### Bibliotecas Utilizadas:
- **Streamlit**: Cria a interface web interativa.
- **Pandas**: Manipula os dados de livros e avaliações.
- **Plotly**: Gera os gráficos interativos.

### Passo a Passo do Código:

1. **Configuração da Página**:
   - A interface é configurada para ocupar toda a largura da página com `st.set_page_config(layout="wide")`.

2. **Leitura dos Dados**:
   - Dois conjuntos de dados são lidos a partir de arquivos CSV:
     - `customer reviews.csv`: Contém as avaliações dos clientes.
     - `Top-100 Trending Books.csv`: Contém informações sobre os 100 livros mais populares.

3. **Filtragem por Preço**:
   - O código identifica o valor máximo e mínimo dos preços dos livros e oferece um controle deslizante na barra lateral para que o usuário defina a faixa de preço que deseja visualizar.
   - Os livros que têm o preço menor ou igual ao valor selecionado são exibidos na interface.

4. **Gráficos Interativos**:
   - Dois gráficos são gerados para auxiliar na análise dos livros:
     - **Gráfico de Barras**: Mostra a quantidade de livros publicados por ano.
     - **Histograma**: Exibe a distribuição dos preços dos livros.

5. **Layout**:
   - Dois gráficos são exibidos lado a lado, utilizando o método `st.columns(2)`.

## Como Executar o Projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/francielesevilha/Dashboard_Reviews_Books

2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   
3. Execute o projeto:
   ```bash
	streamlit run MeuApp.py

### Estrutura dos Dados

- `customer reviews.csv`
**Contém as avaliações dos clientes sobre os livros.**
  
- `Top-100 Trending Books.csv`
- **Contém informações como:**
-	Nome do livro.
-	Ano de publicação.
-	Preço do livro.

## Requisitos
- Python 3.x
- Bibliotecas:
- Streamlit
- Pandas
- Plotly

### Contribuições
Sinta-se à vontade para contribuir com este projeto, enviando pull requests ou reportando problemas.
