# Padrões do repositório

## Dados e segurança

- Não salvar bases grandes no Git.
- Não salvar tokens, secrets, credenciais ou arquivos `.env` no Git.
- Usar Google Drive para bases grandes, arquivos intermediários pesados e outputs.

## CNPJ

- CNPJ sempre deve ser tratado como texto.
- Preservar zeros à esquerda em qualquer leitura, limpeza, transformação ou exportação.
- Separar claramente **CNPJ básico** e **CNPJ completo** quando ambos existirem no processamento.

## Arquivos e formatos

- Usar Parquet apenas em `data/interim`, `data/processed` ou `outputs`.
- Não commitar arquivos Parquet, CSV, ZIP, DuckDB, SQLite, 7z, RAR ou outros arquivos grandes de dados.
- Gerar saídas auditáveis, com nomes claros e documentação suficiente para rastrear origem e transformação.

## Código e notebooks

- Criar scripts modulares em `src`.
- Criar notebooks apenas em `notebooks` ou `orquestrador`.
- Evitar scripts analíticos monolíticos; separar leitura, limpeza, matching, análise e relatórios nos módulos apropriados.
