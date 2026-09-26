# Listas

## Listas não ordenadas

Use `-`, `*` ou `+` no início da linha (escolha um e seja consistente no documento):

```
- Item um
- Item dois
- Item três
```

- Item um
- Item dois
- Item três

## Listas ordenadas

Use números seguidos de ponto. O Markdown renumera automaticamente na saída final, então na prática até repetir `1.` em todas as linhas funciona:

```
1. Primeiro passo
2. Segundo passo
3. Terceiro passo
```

1. Primeiro passo
2. Segundo passo
3. Terceiro passo

## Listas aninhadas (sub-itens)

Indente com 2 ou 4 espaços (dependendo do processador) para criar sub-listas:

```
- Item principal
  - Sub-item 1
  - Sub-item 2
    - Sub-sub-item
- Outro item principal
```

- Item principal
  - Sub-item 1
  - Sub-item 2
    - Sub-sub-item
- Outro item principal

## Listas de tarefas (task lists) — recurso do GFM

Muito usadas em issues e pull requests do GitHub para marcar progresso:

```
- [x] Escrever a introdução
- [x] Revisar sintaxe básica
- [ ] Gravar vídeo de exemplo
- [ ] Publicar o treinamento
```

- [x] Escrever a introdução
- [x] Revisar sintaxe básica
- [ ] Gravar vídeo de exemplo
- [ ] Publicar o treinamento

## Misturando listas com outros elementos

Você pode colocar parágrafos, citações e blocos de código dentro de um item de lista, desde que a indentação esteja alinhada com o início do texto do item:

```
1. Primeiro passo

   Uma explicação mais detalhada do primeiro passo, em um parágrafo próprio.

2. Segundo passo
```

## Resumo do módulo

- `-`, `*` ou `+` para listas não ordenadas (escolha um estilo e mantenha)
- Números com ponto para listas ordenadas
- Indentação de 2–4 espaços cria sub-listas
- `- [ ]` e `- [x]` criam listas de tarefas (checkboxes) no GFM
