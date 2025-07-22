# Teste Analista de BI/Dados

Relatório feito no Google Colab: [relatorio.ipynb](https://colab.research.google.com/drive/1_j8MBhhYwuL3vuyVpbJYmmmwUbMCgJzw?usp=sharing)  
(O arquivo `relatorio.ipynb` está disponível na raiz deste repositório)


Este projeto consiste em um teste dividido em quatro partes, que juntas demonstram um fluxo completo de análise de dados. As três primeiras etapas concentram-se na avaliação da performance de campanhas digitais, abrangendo a extração, o tratamento, a análise e a visualização dos dados. A última etapa inclui integrações externas que enriquecem o teste.


---

## Estrutura do Projeto

### 1. Preparação de Dados

- Extração dos dados de uma planilha Google Sheets via API.
- Tratamento dos dados brutos que estavam em formato "CSV em célula".
- Conversão de colunas de datas e numéricas para formatos adequados.
- Exportação dos dados tratados para arquivo CSV.
- Atualização da planilha original com aba "Dados Tratados".

Arquivos relacionados:
- https://docs.google.com/spreadsheets/d/1YytDjZsIXBTg0ceoXoKq9C8-BMPNOKopZbywCuZSzRY/edit?usp=sharing
- `planilha_processada_da_google_sheets.csv`

---

### 2. SQL para Análises

- Criação de banco local SQLite (`campanhas.db`) para armazenar os dados tratados.
- Estruturação da tabela campanhas.
- Consultas SQL para identificar campanhas com mais leads e melhor CPL.
- Consultas extras para análise por campanha e por canal.

Arquivos relacionados:
- `campanhas.db`

---

### 3. Capacidade Analítica

Principais insights identificados a partir dos dados.

---

### 4. Integrações

- Consulta à API pública do Banco Central para obter cotações do dólar comercial dos últimos 7 dias úteis.
- Processamento dos dados em formato JSON para DataFrame Pandas.
- Exportação dos dados para CSV para uso em análises financeiras.

Arquivos relacionados:
- `cotacao_dolar_ultimos_7_dias.csv`
