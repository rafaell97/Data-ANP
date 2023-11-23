# Projeto ETL - [ANP]

## Descrição

O projeto ETL (Data-ANP) é um sistema de Extração, Transformação e Carga projetado 
para consumir as informações semestrais de preços de combustíveis coletadas por todo o país disponibilizado pela ANP. Ele automatiza a coleta, transformação e carregamento de dados, 
proporcionando uma solução eficiente para garantir dados consistentes e atualizados em um ambiente de armazenamento.

## Regra de negócio
- Extrair o arquivo disponibilizado no site da ANP.
- Gerar arquivos segregados por: Região, estado, bandeira, produto e mês.
- Todos os arquivos devem ter uma versão: agregada e aberta.
- Novo campo com a data da carga.

## Funcionalidades Principais

- **Extração de Dados:**
  - Conecta-se ao site da anp e realiza o download do arquivo no formato .zip, descompacta e disponibiliza para extração das informações.

- **Transformação:**
  - Aplica transformações para limpar, organizar e enriquecer os dados conforme necessário, em conformidade com a regra de negócio. 

- **Carga de Dados:**
  - Carrega os dados transformados em arquivos .csv, criando uma estrutura de pasta conforme a regra de separação definida.

## Tecnologias Utilizadas

- Python
- Spark
