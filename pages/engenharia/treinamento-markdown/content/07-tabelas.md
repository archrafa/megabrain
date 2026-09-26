# Tabelas

## Sintaxe básica

Tabelas são um recurso do GFM (não fazem parte do CommonMark original). A estrutura usa `|` para separar colunas e uma linha de hifens para separar o cabeçalho do corpo:

```
| Coluna 1 | Coluna 2 | Coluna 3 |
|---|---|---|
| valor A | valor B | valor C |
| valor D | valor E | valor F |
```

| Coluna 1 | Coluna 2 | Coluna 3 |
|---|---|---|
| valor A | valor B | valor C |
| valor D | valor E | valor F |

## Alinhamento de colunas

Use `:` na linha separadora para controlar o alinhamento:

```
| Esquerda | Centro | Direita |
|:---|:---:|---:|
| a | b | c |
```

- `:---` alinha à esquerda (padrão)
- `:---:` centraliza
- `---:` alinha à direita

| Esquerda | Centro | Direita |
|:---|:---:|---:|
| a | b | c |

## Dicas práticas

- Você **não precisa** alinhar visualmente as barras `|` no arquivo fonte — só precisa ser consistente com o número de colunas.
- Para incluir um `|` literal dentro de uma célula, escape com `\|`.
- Tabelas muito largas podem ficar difíceis de editar manualmente; ferramentas como extensões de editor (ex.: "Markdown Table Formatter") ajudam a formatar automaticamente.
- Células vazias são permitidas — basta deixar o espaço entre as barras em branco.

## Exemplo real: comparação de ferramentas

| Ferramenta | Tipo | Suporta GFM? |
|---|---|---|
| GitHub | Hospedagem de código | Sim |
| Notion | Anotações | Parcial |
| Obsidian | Anotações locais | Sim (com plugins) |
| Slack | Chat | Parcial |

## Resumo do módulo

- `|` separa colunas, linha de `---` separa cabeçalho do corpo
- `:` na linha separadora controla alinhamento (esquerda, centro, direita)
- Tabelas são um recurso do GFM, não do Markdown "puro"
