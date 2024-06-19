# Conversão de Unidades

Este projeto é um serviço web RESTful construído com Flask em Python, que fornece conversões de temperatura e câmbio. O serviço inclui endpoints para converter temperaturas de Celsius para Fahrenheit e Kelvin, e para converter moedas de Dólares (USD) para Reais (BRL) e de Euros (EUR) para Reais (BRL).

## Funcionalidades

- Conversão de Celsius para Fahrenheit
- Conversão de Celsius para Kelvin
- Conversão de Dólares (USD) para Reais (BRL)
- Conversão de Euros (EUR) para Reais (BRL)

## Requisitos

- Python 3.7 ou superior
- Flask 3.0.3 ou superior

## Instalação

1. Clone o repositório:
    ```sh
    git clone https://github.com/seu-usuario/conversao-unidades.git
    ```
2. Navegue até o diretório do projeto:
    ```sh
    cd conversao-unidades
    ```
3. Crie um ambiente virtual:
    ```sh
    python -m venv venv
    ```
4. Ative o ambiente virtual:
    - No Windows:
      ```sh
      venv\Scripts\activate
      ```
    - No Linux/Mac:
      ```sh
      source venv/bin/activate
      ```
5. Instale as dependências:
    ```sh
    pip install Flask
    ```

## Execução

1. Certifique-se de que o ambiente virtual está ativado.
2. Execute o aplicativo Flask:
    ```sh
    python app.py
    ```
3. Abra o navegador e vá para `http://127.0.0.1:5000` para acessar a página inicial e testar os endpoints.

## Uso

### Endpoints

- **Celsius para Fahrenheit**
  - URL: `/convert/celsius-to-fahrenheit`
  - Método: `GET`
  - Parâmetro: `celsius` (temperatura em Celsius)
  - Exemplo:
    ```sh
    curl "http://127.0.0.1:5000/convert/celsius-to-fahrenheit?celsius=100"
    ```

- **Celsius para Kelvin**
  - URL: `/convert/celsius-to-kelvin`
  - Método: `GET`
  - Parâmetro: `celsius` (temperatura em Celsius)
  - Exemplo:
    ```sh
    curl "http://127.0.0.1:5000/convert/celsius-to-kelvin?celsius=100"
    ```

- **USD para BRL**
  - URL: `/convert/usd-to-brl`
  - Método: `GET`
  - Parâmetro: `usd` (quantidade em Dólares)
  - Exemplo:
    ```sh
    curl "http://127.0.0.1:5000/convert/usd-to-brl?usd=100"
    ```

- **EUR para BRL**
  - URL: `/convert/eur-to-brl`
  - Método: `GET`
  - Parâmetro: `eur` (quantidade em Euros)
  - Exemplo:
    ```sh
    curl "http://127.0.0.1:5000/convert/eur-to-brl?eur=100"
    ```

## Estrutura do Projeto
conversao_unidades_project/
├── app.py
├── static/
│ └── style.css
└── templates/
└── index.html

