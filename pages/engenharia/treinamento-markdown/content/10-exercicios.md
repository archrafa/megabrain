# Exercícios Práticos

Chegou a hora de praticar. Tente resolver cada exercício escrevendo o Markdown mentalmente (ou em um editor à parte) antes de conferir o gabarito.

## Exercício 1 — Cabeçalhos e ênfase

Escreva o Markdown que produziria o seguinte resultado:

> **Guia Rápido**
>
> Este é um texto com uma palavra em *destaque* e outra em **muito destaque**.

<details>
<summary>Ver gabarito</summary>

```
# Guia Rápido

Este é um texto com uma palavra em *destaque* e outra em **muito destaque**.
```

</details>

## Exercício 2 — Lista de tarefas

Escreva uma lista de tarefas (GFM) com três itens, sendo os dois primeiros concluídos e o último pendente.

<details>
<summary>Ver gabarito</summary>

```
- [x] Configurar o ambiente
- [x] Escrever o primeiro commit
- [ ] Abrir o pull request
```

</details>

## Exercício 3 — Link e imagem

Escreva um link para `https://exemplo.com` com o texto "Acesse aqui" e, na linha seguinte, uma imagem de `logo.png` com texto alternativo "Logo da empresa".

<details>
<summary>Ver gabarito</summary>

```
[Acesse aqui](https://exemplo.com)

![Logo da empresa](logo.png)
```

</details>

## Exercício 4 — Tabela

Monte uma tabela com as colunas "Linguagem" e "Paradigma", com duas linhas de dados à sua escolha, alinhando a segunda coluna ao centro.

<details>
<summary>Ver gabarito</summary>

```
| Linguagem | Paradigma |
|---|:---:|
| Python | Multiparadigma |
| Haskell | Funcional |
```

</details>

## Exercício 5 — Bloco de código

Escreva um bloco de código em Python que defina uma função `soma(a, b)` que retorna `a + b`, com destaque de sintaxe ativado.

<details>
<summary>Ver gabarito</summary>

<pre>
```python
def soma(a, b):
    return a + b
```
</pre>

</details>

## Exercício 6 — Identifique o erro

O trecho abaixo tem um problema de sintaxe. Qual é?

```
##Título sem espaço
* item 1
- item 2
```

<details>
<summary>Ver gabarito</summary>

Dois problemas: falta espaço depois do `#` (deveria ser `## Título sem espaço`), e a lista mistura marcadores diferentes (`*` e `-`) — o ideal é escolher um só e manter consistência.

</details>

## Checklist final

- [ ] Sei criar cabeçalhos de todos os níveis
- [ ] Sei aplicar negrito, itálico e tachado
- [ ] Sei criar listas ordenadas, não ordenadas e de tarefas
- [ ] Sei inserir links e imagens
- [ ] Sei criar blocos de código com destaque de sintaxe
- [ ] Sei montar e alinhar tabelas
- [ ] Sei usar citações e elementos avançados
- [ ] Conheço boas práticas e ferramentas do ecossistema Markdown

Parabéns por concluir o treinamento! Continue praticando escrevendo seus próprios documentos em Markdown — a fluência vem com o uso do dia a dia.
