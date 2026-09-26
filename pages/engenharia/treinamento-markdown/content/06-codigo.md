# Código

## Código inline

Como visto no módulo de ênfase, use crase simples para trechos curtos: `` `git commit` ``.

Se o próprio trecho de código contiver uma crase, use crases duplas ao redor: `` ``código com ` crase`` ``.

## Blocos de código

Para blocos maiores, use três crases antes e depois do bloco:

<pre>
```
função exemplo() {
  retornar "olá mundo";
}
```
</pre>

## Syntax highlighting (destaque de sintaxe)

A maioria dos processadores modernos (GitHub, VS Code, GitBook, MkDocs) suporta destaque de sintaxe automático se você indicar a linguagem logo após as três crases de abertura:

<pre>
```python
def saudacao(nome):
    return f"Olá, {nome}!"
```
</pre>

<pre>
```javascript
function saudacao(nome) {
  return `Olá, ${nome}!`;
}
```
</pre>

Linguagens comuns: `python`, `javascript`, `typescript`, `java`, `csharp`, `sql`, `bash`, `json`, `yaml`, `html`, `css`.

## Blocos de código indentados (sintaxe antiga)

O CommonMark original também aceita blocos de código indentados com 4 espaços ou 1 tab, mas essa forma **não permite** indicar a linguagem — por isso, prefira sempre a sintaxe com três crases.

```
    este é um bloco de código
    indentado com 4 espaços
```

## Quando usar cada um

| Situação | Sintaxe recomendada |
|---|---|
| Nome de comando, variável ou arquivo em uma frase | Código inline com crase simples |
| Trecho de código de várias linhas | Bloco com três crases + linguagem |
| Exemplo de saída de terminal | Bloco com três crases + `bash` ou `text` |

## Resumo do módulo

- Crase simples para código inline
- Três crases para blocos de código
- Sempre indique a linguagem depois das crases de abertura para ativar o destaque de sintaxe
- Evite blocos indentados com espaços — prefira sempre a sintaxe de três crases
