# CLAUDE.md — NEGOCIOSDOJAPAO

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** NEGOCIOSDOJAPAO
**Nicho:** Negócios e Empreendedorismo
**Keywords:** Fundado em 2014 no Estado do Rio de Janeiro o Blog Negocios
**Paleta de cores:** ocean | **Fonte:** playfair

Fundado em 2014 no Estado do Rio de Janeiro, o Blog “Negócios do Japão” já é um meio de comunicação expressivo no cenário nacional. Antes de prover mais conhecimento sobre o nosso Blog, eu preciso te explicar como surgiu o nome. “Negócios do Japão” nada mais é que um ditado, ou uma expressão, que nós criamos na nossa roda de amigos. Chamavam de “negócios da China” todos os melhores negócios que fechavam, e nós começamos chamar de “Negócios do Japão” os negócios melhores ainda. É claro que também temos uma admiração enorme pelo país, cultura e empreendedorismo que existe lá. Bom, agora que você já sabe sobre o nome do Blog, posso te explicar melhor as nossas intenções. De início e meio, nosso objetivo sempre foi informar o maior número de pessoas possível sobre a área de negócios, empreendedorismo e finanças. Ao acontecer uma evolução no nosso Blog, várias pessoas começaram escrever para nós sobre outros assuntos. E como nosso Blog se tornou muito grande no seu nicho, começamos também a fazer alguns posts patrocinados, já que um link do nosso site vale muito para qualquer empresa. Mas isso não é a melhor coisa que tenho pra comunicar a você. O melhor de tudo é que analisamos friamente todos os conteúdos para garantir a qualidade e confiabilidade dos conteúdos postados. Nesse Blog você verá diversos temas relacionados a negócios. Basta visitar nossa página principal e começar a ganhar conhecimento.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-G |
| Hero | Hero-G |
| Features | Features-B |
| About Section | About-I |
| Posts | Posts-A |
| Footer | Footer-D |
| Página Sobre | Sobre-F |
| Página Contato | Contato-G |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
