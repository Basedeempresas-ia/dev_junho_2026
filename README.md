# BDE/RFB — dev_junho_2026

Este é o repositório operacional atual do projeto **BDE/RFB junho/2026**.

## Papel de cada ambiente

- **GitHub** guarda o código, a documentação versionada, os notebooks leves e a estrutura mínima do projeto.
- **Codex** cria e altera o código por meio de branches, commits e Pull Requests.
- **Google Colab** executa notebooks e scripts Python, usando este repositório como fonte de código.
- **Google Drive** guarda bases grandes da Receita Federal, arquivos intermediários pesados e outputs gerados.

## Regras importantes

- Bases grandes não devem ser commitadas neste repositório.
- Tokens, secrets, credenciais e arquivos `.env` não devem ser commitados.
- Arquivos de dados como CSV, ZIP, Parquet, DuckDB, SQLite, 7z e RAR devem permanecer fora do Git.
- Use as pastas `data/` e `outputs/` como pontos de montagem/organização local, preservando no Git apenas a estrutura com `.gitkeep`.

## Estrutura operacional

```text
orquestrador/
notebooks/
src/
  io/
  cleaning/
  matching/
  analysis/
  reports/
data/
  raw/
  interim/
  processed/
outputs/
  tables/
  reports/
docs/
```
