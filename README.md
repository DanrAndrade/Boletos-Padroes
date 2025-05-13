# Gerador de Documentos de Cobrança (Boleto Bancário)

## Descrição

Este projeto é uma aplicação Java desenvolvida para gerar "Documentos de Cobrança" (comumente conhecidos como Boletos Bancários) para diferentes instituições financeiras brasileiras. O sistema calcula todos os componentes necessários do boleto, como Nosso Número, Campo Livre, Código de Barras e Linha Digitável, seguindo as especificações de cada banco. Adicionalmente, oferece a opção de gerar uma representação visual do documento em formato PDF.

A aplicação utiliza o padrão de projeto Builder para permitir uma construção flexível e customizada dos documentos de cobrança para cada banco suportado.

## Funcionalidades Principais

* Geração de documentos de cobrança para:
    * Banco do Brasil
    * Itaú Unibanco
    * Bradesco
* Cálculo automático do Campo Livre específico para cada banco.
* Cálculo do Fator de Vencimento seguindo as regras da FEBRABAN (incluindo a transição para a data base de 2025).
* Geração do Código de Barras numérico de 44 posições.
* Geração da Linha Digitável formatada com seus respectivos dígitos verificadores (Módulo 10).
* Interface de linha de comando (CLI) para entrada interativa dos dados do documento.
* Geração opcional do documento de cobrança em formato PDF utilizando a biblioteca iText.

## Tecnologias Utilizadas

* *Linguagem:* Java 17
* *Build e Gerenciamento de Dependências:* Apache Maven
* *Geração de PDF:* iText 5.5.13.3

## Pré-requisitos

Para compilar e executar este projeto, você precisará ter instalado em seu ambiente:

* JDK (Java Development Kit) na versão 17 ou superior, com a variável de ambiente JAVA_HOME configurada.
* Apache Maven.

## Configuração e Instalação

1.  Clone este repositório ou faça o download do código-fonte.
    bash
    # Exemplo com git clone (se aplicável)
    # git clone <url_do_repositorio>
    
2.  Navegue até o diretório raiz do projeto (onde o arquivo pom.xml está localizado).

## Como Compilar o Projeto

No diretório raiz do projeto, execute o seguinte comando Maven para compilar o código e baixar as dependências:

```bash
mvn clean package
