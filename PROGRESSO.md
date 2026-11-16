# Progresso | Pet&Style

## Sobre o projeto
Página inicial da loja fictícia Pet&Style, com as seções Header, Hero, Produtos, Depoimentos e Contato.

## Stack e convenções
- HTML com Tailwind CSS via CDN (layout, espaçamento e responsividade mobile-first)
- SCSS com metodologia BEM (visual dos componentes)
- Sass compilado para `css/style.css`
- Commits no padrão: `feat:`, `style:`, `docs:`, `chore:`, `fix:`

## Regra Tailwind x SCSS
Nunca definir a mesma propriedade nos dois. O Tailwind cuida de layout, grid, flex, gap, padding e breakpoints. O SCSS com BEM cuida de cores da marca, sombras, bordas, hover, estados e variações (modificadores).

---

## Diário

### 27/10/2026

**O que foi feito**
- Criado o repositório público `petstyle-loja-virtual` no GitHub.
- Criada a pasta do projeto e inicializado o Git na branch `main`.
- Criada a estrutura de pastas: `css/`, `imagens/` e `scss/` (com `abstracts/`, `base/` e `components/`).
- Criados os arquivos `index.html`, `.gitignore` e `PROGRESSO.md`.
- Configurado o `.gitignore` para ignorar `node_modules/`, `.DS_Store` e `*.log`.
- Primeiro commit e push para o GitHub realizados com sucesso.
- Instalado o Sass via npm e criado o `package.json` com os scripts `sass` (watch) e `build` (minificado).
- Criadas as variáveis da marca em `scss/abstracts/_variables.scss`.
- Criados o `scss/base/_base.scss` e o `scss/main.scss`.
- Primeira compilação com `npm run build` gerou o `css/style.css` sem erros.
- Segundo commit e push (`feat: configura Sass com variáveis da marca e base`).

**Próximos passos**
- Montar o `index.html` base com Tailwind via CDN e o link para `css/style.css`.
- Criar o Header com Flexbox (Tailwind) e o componente `header` em BEM.

### 04/11/2026

**O que foi feito**
- Criado o `index.html` base com Tailwind via CDN e o link para `css/style.css`, com comentários marcando onde entram as seções.
- Testado no Live Server: o fundo creme do `_base.scss` aparece e, na aba Network, `style.css` e o Tailwind carregaram sem erro 404.
- Terceiro commit e push (`feat: cria index.html base com Tailwind via CDN`).
- Criado o componente `scss/components/_header.scss` em BEM e registrado no `scss/main.scss`.
- Montado o Header no `index.html`: logo, menu de navegação, botão "Fale conosco" e botão hambúrguer, com Flexbox do Tailwind e `sticky` no topo.
- Adicionado script simples para abrir o menu no celular, com atualização do `aria-expanded`.
- Testado em desktop (links em linha, sem hambúrguer) e em 375 px (logo e hambúrguer, menu abrindo ao clicar).
- Quarto commit (`feat: cria Header responsivo com Flexbox e BEM`). O push falhou algumas vezes com erro 500 do GitHub (`Internal Server Error`) e passou depois, enviando junto o commit do diário (`docs: atualiza PROGRESSO.md com o Header`).

**Próximos passos**
- Criar a seção Hero com Tailwind e o componente `hero` em BEM (`scss/components/_hero.scss`).
- Ajustar o contraste do botão "Fale conosco" usando `$color-primary-dark` como cor padrão.

### 12/11/2026

**O que foi feito**
- Confirmado que o GitHub voltou ao normal (`git status` limpo e `git pull` sem demora).
- Criado o componente `scss/components/_hero.scss` em BEM, com selo, título, texto, botões, modificador `hero__cta--outline` e card visual, e registrado no `scss/main.scss`.
- Montada a seção Hero no `index.html`: selo, título com destaque em laranja, texto, dois botões e card em gradiente com a frase "Frete grátis". Layout com Grid e Flexbox do Tailwind, em uma coluna no celular e duas colunas a partir de 768 px.
- Testado em desktop: texto e botões à esquerda, card em gradiente à direita.
- Quinto commit e push (`feat: cria seção Hero responsiva com Flexbox, Grid e BEM`), enviados com sucesso.

**Próximos passos**
- Conferir o Hero em 375 px e o hover dos dois botões.
- Criar a seção de Produtos com pelo menos 4 cards (Grid do Tailwind e componente `product-card` em BEM).
- Ajustar o contraste do botão "Fale conosco" usando `$color-primary-dark` como cor padrão.

### 15/11/2026

**O que foi feito**
- Testado o Hero em 375 px no DevTools (375 x 840): tudo empilhado, com selo, título, texto, botões um sobre o outro e card em gradiente embaixo.
- Criado o componente `scss/components/_products.scss` em BEM, com os blocos `products` (título e subtítulo) e `product-card` (imagem, categoria, nome, descrição, preço e botão), e registrado no `scss/main.scss`.
- Montada a seção de Produtos no `index.html` com 4 cards (Roupinhas, Camas, Brinquedos e Acessórios), usando Grid do Tailwind: 1 coluna no celular, 2 a partir de 640 px e 4 a partir de 1024 px. Preços e nomes são fictícios, e a faixa colorida com o nome da categoria ocupa o lugar das fotos por enquanto.
- Testados os Produtos em desktop (4 cards lado a lado) e em 700 px (2 cards por linha). Preços e botões "Comprar" ficam alinhados na base dos cards, e o título aparece inteiro, sem ficar escondido atrás do Header.
- Criado o componente `scss/components/_testimonials.scss` em BEM, com os blocos `testimonials` (título e subtítulo) e `testimonial-card` (estrelas, texto, avatar, nome e pet), e registrado no `scss/main.scss`.
- Montada a seção de Depoimentos no `index.html` com 3 cards fictícios, em fundo branco para contrastar com o creme da página: 1 coluna no celular e 3 colunas a partir de 768 px.
- Testados os Depoimentos em desktop (3 cards lado a lado), em 375 px e em 700 px (cards empilhados, como previsto, porque o breakpoint é 768 px).
- Console do navegador sem erros, apenas o aviso esperado do Tailwind via CDN ("should not be used in production").
- Diário dos Produtos enviado ao GitHub (`docs: atualiza PROGRESSO.md com os Produtos`).

## 16/11/2026 - Imagem de destaque no Hero

- O card em degradê do Hero foi substituído por uma foto de destaque (`imagens/produto-roupinhas.png`), atendendo ao requisito de chamada principal com imagem de destaque.
- O aviso "Frete grátis em compras acima de R$ 150" virou uma etiqueta sobre a foto, feita com classes do Tailwind direto no HTML.
- Nenhuma imagem foi alterada, convertida ou apagada: a foto já existia no repositório e apenas foi reutilizada.
- Testado em 375 px (mobile): foto abaixo do texto, com a etiqueta sobre ela.
- Commit: `0a6dd2b` - `feat: adiciona imagem de destaque no Hero`.

### Divisão entre Tailwind e SCSS

A divisão foi proposital: o Tailwind (via CDN) cuida de layout, espaçamento e responsividade, com os breakpoints `sm:`, `md:` e `lg:`, e o SCSS com BEM cuida de cores, sombras e efeitos de hover.