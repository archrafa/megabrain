# RAFAEL//HUB

Hub pessoal com as páginas HTML geradas com o Claude: arquitetura de soluções, engenharia, IA, negócio bancário, crédito rural e carreira. Publicado via GitHub Pages.

## Estrutura

```
.
├── index.html                                   # hub (catálogo por categoria)
├── .nojekyll                                    # serve os arquivos como estão, sem Jekyll
└── pages/
    ├── arquitetura/
    │   ├── memento-arquitetura.html             # checklist de avaliação de solução (80 itens)
    │   ├── matriz-persistencia.html             # decisão de banco: CAP, PACELC, Outbox
    │   └── performance-computacional.html       # leis de escala, método, playbook, biblioteca
    ├── engenharia/
    │   ├── treinamento-git-github-actions.html  # Git, Git Flow, GitHub e Actions (TorqueOS)
    │   └── prancha-python.html                  # trilha Python com olhar de arquiteto
    ├── negocio/
    │   └── mapa-areas-banco-bian.html           # áreas, processos e domínios de um banco × BIAN
    ├── ia/
    │   └── matematica-por-tras-dos-llms.html    # álgebra linear, cálculo e probabilidade interativos
    └── carreira/
        ├── guia-mestre-2026.html                # vida, saúde, estudo e carreira até 2031
        └── lista-leitura-plano-evolucao.html    # livros por frente + cronograma trimestral
```

## Publicar no GitHub Pages

1. Faça o merge do PR na branch `main`.
2. Em **Settings → Pages**, selecione *Deploy from a branch* → `main` / `/ (root)`.
3. A URL fica `https://<seu-usuario>.github.io/<nome-do-repo>/`.

## Adicionar uma nova página

1. Coloque o HTML em `pages/<categoria>/<nome>.html`.
2. No `index.html`, adicione um objeto no array `PAGES`:

```js
{cat:"arq", t:"Título", href:"pages/arquitetura/nome.html", date:"2026-10-01",
 type:"Ferramenta", icon:"check", d:"Descrição curta.",
 m:[["12","itens"]], tags:["Tag1","Tag2"]}
```

3. Categorias existentes (`cat`): `arq`, `eng`, `ia`, `agro`, `car`. Para criar outra, adicione em `CATS`.
4. Ícones: `check`, `db`, `gauge`, `branch`, `code`, `sigma`, `map`, `compass`, `book`. `date` é opcional. Um card com `status:"lost"` aparece como pendência, sem link.
5. Para o botão "◂ HUB", copie o bloco `<a class="hub-back">` + `<style>` do fim de qualquer página.

## Observações

- **Privacidade:** o GitHub Pages é público mesmo com repositório privado (exceto no plano Enterprise). O *Guia Mestre* traz seu nome completo, rotina, saúde, nutrição, crenças espirituais e reflexões de carreira. A *Lista de Leitura* cita o engajamento da comunidade em que você atua. As duas têm `noindex`, que evita buscadores mas não impede o acesso de quem tiver o link.
- Memento, Matriz, Prancha Python e Lista de Leitura guardam o progresso no `localStorage` do navegador. Nada sai do seu browser. A Lista de Leitura usava a API de armazenamento do Claude; foi adaptada para `localStorage`.
- **Pendente:** o *Mapa de Domínios da Esteira de Crédito Agrícola PF* ainda não está no repositório. Salve o HTML em `pages/agro/` e troque o card `status:"lost"` por um link.
