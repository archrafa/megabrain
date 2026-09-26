# Elementos Avançados

## Citações (blockquotes)

Use `>` no início da linha:

```
> Esta é uma citação simples.
```

> Esta é uma citação simples.

Citações podem ser aninhadas e conter outros elementos:

```
> Nível 1 da citação
>> Nível 2, aninhado
>
> Um **negrito** dentro da citação também funciona.
```

> Nível 1 da citação
>> Nível 2, aninhado
>
> Um **negrito** dentro da citação também funciona.

## HTML embutido

A maioria dos processadores de Markdown permite misturar tags HTML diretamente no texto, para casos que a sintaxe nativa não cobre:

```
Este texto tem uma quebra<br>forçada usando HTML.

<details>
<summary>Clique para expandir</summary>
Conteúdo escondido que aparece ao clicar.
</details>
```

## Notas de rodapé (footnotes)

Recurso disponível em várias extensões (não no CommonMark puro, mas comum em MkDocs, Pandoc e outros):

```
Aqui está uma afirmação que precisa de fonte[^1].

[^1]: Esta é a nota de rodapé com a explicação ou fonte.
```

## Definição de termos (glossário)

Algumas extensões suportam listas de definição:

```
Markdown
: Linguagem de marcação leve para formatação de texto.

GFM
: Variante do Markdown usada pelo GitHub, com tabelas e task lists.
```

## Emojis

Muitas plataformas (GitHub, Slack, Discord) suportam atalhos de emoji com `:nome:`:

```
Ótimo trabalho! :tada: :rocket:
```

## Escapando blocos inteiros

Se precisar mostrar um exemplo de Markdown sem que ele seja processado, use quatro crases externas quando o exemplo interno já usa três:

<pre>
````
```
código de exemplo
```
````
</pre>

## Resumo do módulo

- `>` cria citações, e pode ser aninhado com `>>`
- HTML puro pode ser misturado ao Markdown quando necessário
- Notas de rodapé, listas de definição e emojis dependem da extensão/plataforma usada
- Use crases extras para "escapar" um bloco de código que já contém crases
