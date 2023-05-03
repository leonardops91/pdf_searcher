# Busca de Funcionários em Arquivos PDF

Este script foi desenvolvido para facilitar a busca de vários nomes e matrículas ao mesmo tempo em um arquivo de PDF. O desafio era encontrar uma solução para buscar registros em um arquivo com um grande número de páginas e tornava-se oneroso utilizar o Ctrl+F para cada um deles, além de ocupar muito tempo do responsável. A solução foi feita utilizando a linguagem Python e as bibliotecas PyPDF2, CSV e Pandas.

## Pré-requisitos

Antes de utilizar o script, é necessário instalar a biblioteca PyPDF2.

Para instalar a biblioteca no Google Colab, basta executar o seguinte comando:
```
!pip install PyPDF2
```

## Utilização

O script requer o caminho completo para dois arquivos: um arquivo CSV com a lista de nomes e matrículas dos funcionários e outro arquivo PDF com o boletim diário em que se deseja procurar as ocorrências.

O usuário deve inserir o nome do arquivo CSV e do arquivo PDF, respeitando a sintaxe:
```python
arquivo_funcionarios = '/caminho/completo/funcionarios.csv'
arquivo_pdf = '/caminho/completo/arquivo.pdf'
```

O script irá varrer todo o arquivo em busca de cada nome e cada matrícula, retornando, caso haja ocorrências, os registros encontrados e as respectivas páginas no arquivo.

O resultado será exibido em um dataframe do Pandas com as informações dos funcionários encontrados.
