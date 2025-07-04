# Análise de Dados de Vendas com Python

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Este projeto realiza uma análise exploratória de um conjunto de dados de vendas de uma empresa familiar de produção e venda de bolos artesanais, utilizando a linguagem de programação Python e suas poderosas bibliotecas para análise de dados e visualização. O objetivo principal é extrair insights valiosos sobre o comportamento das vendas, identificar padrões e tendências nos dados fornecidos.

## 🚀 Visão Geral da Análise

Um dos gráficos principais da análise, mostrando a distribuição ou a relação entre variáveis importantes dos seus dados de vendas:

<p align="center">
  <img src="img/visao_geral_vendas.png" alt="Visão Geral da Análise de Vendas" width="800"/>
</p>

## Descrição do Projeto

O projeto envolve as seguintes etapas principais:

1.  **Carregamento e Inspeção Inicial dos Dados**: Utilização da biblioteca Pandas para carregar o arquivo de dados (`dados/dados_vendas_amor_cakes.xlsx`) e realizar uma inspeção inicial para entender a estrutura, os tipos de dados e a presença de valores ausentes.
2.  **Limpeza e Preparação dos Dados (Se Necessário)**: Aplicação de técnicas de limpeza para garantir a qualidade dos dados, como tratamento de valores ausentes, correção de tipos de dados e resolução de inconsistências.
3.  **Criação de Novas Colunas (Opcional)**: Desenvolvimento de novas colunas a partir dos dados existentes para facilitar a análise, como o cálculo do valor total da venda ou a identificação do valor do desconto.
4.  **Análise Exploratória Detalhada**: Utilização de métodos estatísticos e visualizações para explorar as relações entre as variáveis e identificar padrões importantes nos dados de vendas.
5.  **Visualização de Dados**: Criação de gráficos informativos para representar a distribuição dos dados e as relações entre as variáveis, facilitando a compreensão dos insights extraídos.

## 💻 Tecnologias Utilizadas

As seguintes tecnologias e bibliotecas Python foram utilizadas neste projeto:

* **Python**: A linguagem de programação principal para a análise de dados e desenvolvimento do script.
* **Pandas**: Uma biblioteca poderosa para manipulação e análise de dados, fornecendo estruturas de dados como DataFrames para trabalhar com os dados de forma eficiente.
* **Matplotlib**: Uma biblioteca fundamental para a criação de gráficos e visualizações estáticas em Python.
* **Seaborn**: Uma biblioteca de visualização de dados construída sobre o Matplotlib, fornecendo uma interface de alto nível para criar gráficos estatísticos atraentes e informativos.
* **Jupyter Notebook**: Um ambiente de desenvolvimento interativo que permite combinar código Python, visualizações e texto explicativo (Markdown) em um único documento, facilitando a exploração e a comunicação dos resultados da análise.
* **Openpyxl**: Necessário para ler e escrever arquivos `.xlsx` com Pandas.
* **Formato de Dados**: O projeto foi desenvolvido utilizando dados em formato **XLSX** (Excel).
* **Markdown**: Utilizado para a formatação do texto explicativo dentro do Jupyter Notebook e para a criação deste arquivo README.

## 🚀 Como Executar

Para executar este projeto em seu ambiente local, siga os passos abaixo:

1.  **Clone o repositório**:

    ```bash
    git clone [https://github.com/SeuNomeDeUsuario/Projeto_Analise_de_Vendas.git](https://github.com/SeuNomeDeUsuario/Projeto_Analise_de_Vendas.git)
    cd Projeto_Analise_de_Vendas
    ```
    (Lembre-se de substituir `SeuNomeDeUsuario` pelo seu username do GitHub)

2.  **Instalar as dependências**:
    Recomenda-se criar um ambiente virtual para gerenciar as dependências.

    ```bash
    python -m venv venv
    source venv/bin/activate  # No Windows, use `venv\Scripts\activate`
    pip install -r requirements.txt
    ```

3.  **Rodar o Código**:
    O código principal da análise está no arquivo `Projeto_Analise_de_Vendas.ipynb` (localizado na pasta `notebooks/`). Você pode executá-lo em um ambiente Jupyter Notebook ou Jupyter Lab:

    ```bash
    jupyter notebook notebooks/Projeto_Analise_de_Vendas.ipynb
    ```

    Após a execução do notebook, os gráficos serão gerados. **Para que um gráfico apareça no `README.md`, você precisará salvá-lo na pasta `img/` com o nome `visao_geral_vendas.png`.** Por exemplo, no seu notebook, após criar um gráfico e antes de `plt.show()` ou `plt.close()`:

    ```python
    import os
    # ... (seu código para criar o gráfico, ex: fig, ax = plt.subplots()...)

    # Caminho para salvar a imagem (assumindo notebook em 'notebooks/' e 'img/' na raiz)
    img_folder = os.path.join('..', 'img') # '..' para subir um nível para a raiz do projeto

    if not os.path.exists(img_folder):
        os.makedirs(img_folder)
        print(f"Pasta '{img_folder}' criada com sucesso.")

    # Salva o gráfico principal para o README
    fig.savefig(os.path.join(img_folder, 'visao_geral_vendas.png'), bbox_inches='tight', dpi=300)
    plt.close(fig) # Fecha a figura para não exibí-la se não for necessário
    ```

## 🤝 Contribuições

Contribuições são bem-vindas! Se você tiver ideias para melhorias, novas funcionalidades ou encontrar algum problema, sinta-se à vontade para abrir uma *issue* ou enviar um *pull request*.

## 📄 Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 📧 Contato

Se você tiver alguma dúvida ou sugestão, entre em contato:

* **Nome**: Flávio Henrique Barbosa
* **LinkedIn**: [Flávio Henrique Barbosa | LinkedIn](https://www.linkedin.com/in/fl%C3%A1vio-henrique-barbosa-38465938)
* **Email**: flaviohenriquehb777@outlook.com

---
