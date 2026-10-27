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

**Próximos passos**
- Instalar o Sass e criar o `package.json` com os scripts de compilação.
- Criar os partials SCSS e definir as variáveis da marca (cores, tipografia).
- Montar o `index.html` base com o Tailwind via CDN e o link para `css/style.css`.
- Começar o Header com Flexbox, usando BEM nas classes.