# desafio-regras

Esse projeto consiste em um sistema de processamento e exibição de resultados para serem implementadas por candidatos interessados em participar do processo de seleção da empresa.

## O desafio

O sistema a ser implementado consiste em um motor de análise de produtos, onde caracteristicas de produtos são analisadas segundo regras cadastradas.

Pode-se dividir o projeto em duas partes:
1. Motor de análise:
    * Script (batch) que periódicamente checa se existem produtos não análisados e em caso positivo irá processar a classificação daquele produto.
        * Os produtos devem ser processados segundo regras. Por exemplo: análisar se o produto tem a caracteristica cor igual a vermelho, e então criar um objeto para registrar este resultado.
    * Exemplo de funcionamento do motor:
        1. Um produto é cadastrado no banco de dados com as seguintes caracteristicas:
            * cor: vermelho;
            * tipo: brinquedo;
            * codigo_gtin: 12345678
        2. O motor captura o produto recém cadastrado e analisa segundo um conjunto de regras.
            * Uma regra pode verificar se a cor do produto é vermelha, nesse caso o resultado é positivo.
        3. Para cada regra uma classificação é cadastrada de forma a informar o resultado.
    
2. Interface de usuário:
    * Telas para exibição de resultados e edição de objetos.

Devem ser implementados:
* Motor de processamento de regras.
* Pelo menos uma das seguintes funcionalidades:
    * Tela para exibição de produtos, suas caracteristicas e classificações. 
    * Tela para cadastro e edição de regras.
    * API para consulta de classificação de produtos.
 
Principais quesistos analisados:
* Implementação de testes:
    * São recomendadas metodologias de implementação como TDD e BDD.
* Qualidade do código:
    * Clareza;
    * Organização;
    * Performance.

Deve-se utilizar a linguagem Python 3.5 ou superior e Django 1.11 ou superior.

São dados exemplos de modelos de dados na seguinte fixture: [exemplos](https://github.com/felipehogrefe/desafio-regras/blob/main/fixtures.json). \
Estes modelos podem ser alterados, adicionando campos aos modelos ou criando novos modelos. \
Note que as regras são cruciais ao sistema, aconselha-se criar novas regras e/ou editar as existentes. 



