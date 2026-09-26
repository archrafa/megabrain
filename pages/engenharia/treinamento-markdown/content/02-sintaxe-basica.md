# Sintaxe Básica

## Cabeçalhos

Cabeçalhos usam o símbolo `#` no início da linha. Quanto mais `#`, menor o nível do título — de `#` (título principal) até `######` (nível 6).

```
# Título nível 1
## Título nível 2
### Título nível 3
#### Título nível 4
##### Título nível 5
###### Título nível 6
```

**Regra importante:** sempre deixe um espaço entre o(s) `#` e o texto do título.

## Parágrafos

Parágrafos são simplesmente linhas de texto separadas por uma **linha em branco**. Markdown ignora quebras de linha simples dentro de um mesmo bloco de texto.

```
Este é o primeiro parágrafo.
Esta linha ainda faz parte do primeiro parágrafo, mesmo estando em outra linha.

Esta linha, por estar separada por uma linha em branco, é um novo parágrafo.
```

## Quebra de linha forçada

Se você quiser forçar uma quebra de linha **dentro** do mesmo parágrafo (sem criar um novo parágrafo), existem duas formas:

1. Terminar a linha com **dois ou mais espaços** antes do Enter.
2. Usar a tag HTML `<br>` (funciona na maioria dos processadores).

## Linha horizontal

Para criar uma linha divisória, use três ou mais hifens, asteriscos ou underscores em uma linha isolada:

```
---
***
___
```

Todas produzem o mesmo resultado visual: uma linha horizontal separando seções.

## Comentários e escape de caracteres

Se você precisar exibir um caractere especial do Markdown sem que ele seja interpretado como formatação (por exemplo, um asterisco literal), use a barra invertida `\` antes dele:

```
\*isto não vira itálico\*
\# isto não vira um título
```

## Resumo do módulo

- `#` até `######` para cabeçalhos (com espaço depois do `#`)
- Linha em branco separa parágrafos
- Dois espaços no fim da linha força quebra dentro do parágrafo
- `---`, `***` ou `___` criam uma linha horizontal
- `\` escapa caracteres especiais
