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
- Quarto commit (`feat: cria Header responsivo com Flexbox e BEM`). O push falhou duas vezes com erro 500 do GitHub (`Internal Server Error`), então o commit ficou apenas local por enquanto.

**Próximos passos**
- Repetir o `git push` quando o GitHub estabilizar e confirmar com `git status`.
- Criar a seção Hero com Tailwind e o componente `hero` em BEM (`scss/components/_hero.scss`).
- Ajustar o contraste do botão "Fale conosco" usando `$color-primary-dark` como cor padrão.