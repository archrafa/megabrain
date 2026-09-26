# Boas Práticas e Ferramentas

## Organização de arquivos

- Nomeie arquivos em minúsculas, com hifens no lugar de espaços: `guia-de-instalacao.md`, não `Guia De Instalação.md`.
- Um `README.md` na raiz de um repositório é o primeiro arquivo que qualquer pessoa vê — capriche nele.
- Para documentação extensa, separe em múltiplos arquivos `.md` organizados em pastas (ex.: `docs/instalacao.md`, `docs/configuracao.md`) em vez de um único arquivo gigante.

## Consistência de estilo

- Escolha um marcador de lista (`-` ou `*`) e um marcador de ênfase (`**` ou `__`) e mantenha o mesmo padrão em todo o documento/projeto.
- Use apenas um `#` (nível 1) por documento, reservado para o título principal.
- Deixe uma linha em branco antes e depois de blocos de código, tabelas e listas — melhora a legibilidade tanto no arquivo fonte quanto na renderização.

## Linters e formatadores

- **markdownlint**: extensão popular (VS Code, linha de comando) que aponta inconsistências de estilo.
- **Prettier**: também formata arquivos Markdown automaticamente.
- Configurar um linter no projeto evita discussões de estilo em revisões de código.

## Ferramentas úteis

| Ferramenta | Uso |
|---|---|
| VS Code + extensão Markdown Preview | Editar com visualização lado a lado |
| Obsidian / Notion / Joplin | Anotações pessoais em Markdown |
| Pandoc | Converter Markdown para PDF, Word, HTML e outros formatos |
| MkDocs / Docusaurus / GitBook | Gerar sites de documentação a partir de arquivos `.md` |
| markdownlint | Checar consistência de estilo |

## Acessibilidade

- Sempre preencha o texto alternativo de imagens.
- Use hierarquia de cabeçalhos correta (não pule de `#` para `###` sem justificativa) — leitores de tela dependem dessa estrutura.
- Evite usar apenas cor ou formatação visual para transmitir significado (ex.: "veja o item **em vermelho**" não funciona em texto puro).

## Erros comuns

1. Esquecer o espaço depois do `#` nos cabeçalhos.
2. Misturar `-`, `*` e `+` na mesma lista.
3. Não indicar a linguagem nos blocos de código, perdendo o destaque de sintaxe.
4. Esquecer a linha em branco antes de uma lista ou bloco de código, o que pode quebrar a renderização em alguns processadores.
5. Deixar links quebrados ou texto alternativo vazio em imagens.

## Resumo do módulo

- Nomes de arquivo em minúsculas com hifens
- Consistência de sintaxe em todo o projeto
- Use linters (markdownlint) para manter padrão
- Pandoc converte Markdown para outros formatos; MkDocs/Docusaurus geram sites de documentação
- Preste atenção à acessibilidade: alt text e hierarquia de cabeçalhos
