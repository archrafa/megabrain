# Links e Imagens

## Links básicos

A sintaxe é `[texto exibido](URL)`:

```
[Documentação do GitHub](https://docs.github.com)
```

Resultado: [Documentação do GitHub](https://docs.github.com)

## Links com título (tooltip)

Adicione um título entre aspas depois da URL — aparece como tooltip ao passar o mouse:

```
[Documentação do GitHub](https://docs.github.com "Clique para abrir a documentação")
```

## Links automáticos

Para transformar uma URL ou e-mail em link clicável sem texto personalizado, use `< >`:

```
<https://www.exemplo.com>
<contato@exemplo.com>
```

## Links de referência

Úteis quando o mesmo link é usado várias vezes no documento, ou para manter o texto mais limpo:

```
Veja mais em [nossa documentação][docs] ou no [repositório][repo].

[docs]: https://docs.exemplo.com
[repo]: https://github.com/exemplo/repo
```

## Links internos (âncoras)

Para linkar para um cabeçalho dentro do mesmo documento, use `#` seguido do título em minúsculas e com hifens no lugar de espaços:

```
[Ir para a seção de listas](#listas)
```

## Imagens

A sintaxe é quase igual à de links, mas com `!` na frente:

```
![Texto alternativo da imagem](https://exemplo.com/imagem.png)
```

- O **texto alternativo** (`alt text`) é exibido se a imagem não carregar e é importante para acessibilidade e SEO.
- Assim como links, imagens também aceitam título entre aspas e formato de referência.

## Imagem como link

Para tornar uma imagem clicável, envolva a sintaxe de imagem dentro da sintaxe de link:

```
[![Logo](logo.png)](https://exemplo.com)
```

## Boas práticas

- Sempre preencha o texto alternativo das imagens — não deixe `![]()`.
- Prefira links de referência em documentos longos com muitos links repetidos.
- Verifique se os links relativos (para arquivos dentro do mesmo repositório) usam o caminho correto a partir da raiz do projeto.
