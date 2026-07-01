# Fluxo operacional

Fluxo previsto para o ambiente operacional do projeto **BDE/RFB junho/2026**:

```text
GitHub → Codex → Pull Request → Merge → Colab → Google Drive → outputs
```

## Etapas

1. **GitHub** mantém o repositório com código, notebooks leves, documentação e estrutura versionada.
2. **Codex** cria branches, altera arquivos e prepara commits para revisão.
3. **Pull Request** concentra a revisão das mudanças antes de entrar na linha principal.
4. **Merge** incorpora ao branch principal apenas mudanças revisadas.
5. **Colab** executa notebooks e scripts com recursos de nuvem.
6. **Google Drive** armazena bases grandes da Receita Federal, arquivos intermediários pesados e artefatos de execução.
7. **outputs** recebe tabelas, relatórios e demais saídas geradas, sem commit de arquivos pesados.
