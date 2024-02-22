# API de Geração de Código de Barras

Esta é uma API desenvolvida durante a Next Level Week (NLW) da Rocketseat, ministrada por Rafael Ferreira, do canal Programador Lhama no YouTube. A API foi construída utilizando Python e Flask, e tem como objetivo gerar códigos de barras de forma simples e eficiente.

## Funcionalidades

- Geração de código de barras a partir de um texto fornecido.
- Suporte a diferentes formatos de código de barras, como EAN-13, Code 39, etc.

## Frameworks utilizados

- Cerberus 1.3.5
- Flask 3.0.1
- Python-barcode 0.15.1
- Pytest 8.0.0

## Como utilizar?

### Clone o repositório

Use o comando abaixo para clonar o repositório:

    $ git clone https://github.com/neanderdev/nlw-expert-python.git

### Criar e habilitar o virtualenv

Usar os comandos na raiz do projeto clonado.

Criar ambiente virtual:

    $ pip install virtualenv

    Windows:
    $ py -m venv .venv

    Unix/macOS:
    $ python3 -m venv .venv  

Habilitar/Ativar ambiente virtual:

    $ .\.venv\Scripts\activate.bat

Baixar libs (ficam baixadas apenas no ambiente virtual):

    $ pip install -r requirements.txt

Executar projeto:

    $ python run.py

Executar testes:

    $ pytest

### Usando a aplicação

Realizar requisição POST na url *http://localhost:3000/create_tag*

Body Json example:

    {
        "product_code": "123"
    }
