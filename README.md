# RAFAEL//HUB

Hub pessoal com as páginas HTML geradas com o Claude: arquitetura, autoavaliação, engenharia, IA, negócio bancário e crédito rural, e carreira. Publicado via GitHub Pages.

## Estrutura

```
.
├── index.html                                     # hub (catálogo por categoria)
├── .nojekyll
└── pages/
    ├── arquitetura/
    │   ├── memento-arquitetura.html               # checklist de avaliação de solução (80 itens)
    │   ├── matriz-persistencia.html               # decisão de banco: CAP, PACELC, Outbox
    │   ├── aws-well-architected.html              # 6 pilares, review e anti-patterns        (de .docx)
    │   ├── owasp-top10.html                       # OWASP Top 10 2021, vetores e mitigações   (de .docx)
    │   ├── gof-design-patterns.html               # 23 padrões GoF                           (de .docx)
    │   ├── padroes-arquiteturais-modernos.html    # 20 padrões distribuídos                  (de .docx)
    │   └── performance-computacional.html         # leis de escala, método, playbook
    ├── autoavaliacao/                             # série interativa Domino/Reviso/Estudo    (de .docx)
    │   ├── arquitetura-solucoes.html
    │   ├── arquitetura-software.html
    │   ├── arquitetura-corporativa.html
    │   └── arquitetura-ia.html
    ├── engenharia/
    │   ├── treinamento-git-github-actions.html    # Git, Git Flow, GitHub e Actions (TorqueOS)
    │   ├── prancha-python.html                    # trilha Python com olhar de arquiteto
    │   └── guia-devin.html                        # Devin (Cognition) para arquitetos        (de .docx)
    ├── ia/
    │   ├── matematica-por-tras-dos-llms.html      # álgebra linear, cálculo e probabilidade interativos
    │   ├── arquitetura-ia-do-zero.html            # curso de arquitetura de IA               (de .docx)
    │   ├── visceras-da-ia.html                    # pesos, carregamento e inferência         (de .docx)
    │   └── montador-de-prompt.html                # montador de prompt estático/volátil
    ├── negocio/
    │   └── mapa-areas-banco-bian.html             # áreas, processos e domínios de um banco × BIAN
    ├── agro/
    │   ├── esteira-credito-agricola.html          # 18 domínios da esteira PF (DDD × BIAN × MCR)
    │   └── guia-agronegocio-brasileiro.html       # referência do agronegócio                (de .docx)
    └── carreira/
        ├── guia-mestre-2026.html                  # vida, saúde, estudo e carreira até 2031
        ├── lista-leitura-plano-evolucao.html      # livros por frente + cronograma
        └── plano-estudos-arquiteto-ia.html        # 14 meses, 4 fases                        (de .pdf)
```

## Publicar no GitHub Pages

1. Faça o merge do PR na branch `main`.
2. Em **Settings → Pages**, selecione *Deploy from a branch* → `main` / `/ (root)`.
3. A URL fica `https://<seu-usuario>.github.io/<nome-do-repo>/`.

## Adicionar uma nova página

1. Coloque o HTML em `pages/<pasta>/<nome>.html`.
2. No `index.html`, adicione um objeto no array `PAGES`:

```js
{cat:"arq", t:"Título", href:"pages/arquitetura/nome.html", date:"2026-10-01",
 type:"Ferramenta", icon:"check", d:"Descrição curta.",
 m:[["12","itens"]], tags:["Tag1","Tag2"]}
```

3. Categorias (`cat`): `arq`, `auto`, `eng`, `ia`, `agro`, `car`. Para criar outra, adicione em `CATS`.
4. Ícones: `check`, `db`, `gauge`, `cloud`, `shield`, `grid`, `target`, `branch`, `code`, `terminal`, `sigma`, `layers`, `cpu`, `wand`, `map`, `leaf`, `compass`, `book`, `route`. `date` é opcional.
5. Para o botão "◂ HUB", copie o bloco `<a class="hub-back">` + `<style>` do fim de qualquer página.

## Páginas convertidas

As páginas marcadas "(de .docx)" e "(de .pdf)" foram convertidas para um layout de leitura comum: sumário lateral com filtro (atalho `/`), barra de progresso, tema claro/escuro e versão para impressão. Nos quatro guias de autoavaliação, a coluna "Autoavaliação" virou botões Domino/Reviso/Estudo com placar, salvos no `localStorage`.

## Observações

- **Privacidade:** o GitHub Pages é público mesmo com repositório privado (exceto no plano Enterprise). O *Guia Mestre* traz nome completo, rotina, saúde, nutrição, crenças e reflexões de carreira; a *Lista de Leitura* cita o engajamento da comunidade em que você atua. As duas têm `noindex`, que evita buscadores mas não impede o acesso de quem tiver o link. Na conversão do *Guia do Agronegócio* e de *As Vísceras da IA*, as linhas de capa com nome e empregador ("Elaborado para…", "Preparado para…") ficaram de fora.
- Memento, Matriz, Prancha Python, Lista de Leitura e os guias de autoavaliação guardam o progresso no navegador. Nada sai do seu browser.
