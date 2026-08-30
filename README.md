# Situação de Aprendizagem 1 - Desenvolvimento Web

## Aluno: Renan Croffi

### Professor: Rodrigo Attique

#### GitHub Pages
[Link github pages](https://recroffi.github.io/situacao-aprendizagem-1/)

## O Projeto

Elaboração de um blog pessoal, contendo 3 paginas em html interligadas. Utilizando também css e todos outros conceitos que foram passados durante o período de aulas.

## Páginas

O site tem três páginas HTML interligadas pelo menu de navegação do cabeçalho, presente em todas elas.

| Página | Conteúdo |
| --- | --- |
| `index.html` | Página inicial do blog. Lista o post com título, miniatura, resumo, data e o link "Leia mais". |
| `post.html` | O post completo: imagem de destaque, título, três parágrafos de texto, data e link de retorno à página inicial. |
| `sobre.html` | Apresentação pessoal em duas colunas — foto de perfil com moldura à esquerda, biografia à direita — e link de retorno à página inicial. |

Cabeçalho e rodapé são comuns às três páginas.

## Wireframes

_Wireframes_ são guias visuais simples, ou _blueprints_ de um website ou de um app. Nesse projeto foram elaborados usando **Figma**.

### Início (`index.html`)

![Wireframe da página inicial: cabeçalho com o título "Meu Blog", menu de navegação (Início, Blog, Sobre) e lista de posts com título, data, resumo e link "Ler mais".](wireframes/home-top-section.png)

### Post (`post.html`)

![Wireframe da página de post: título, data de publicação, espaço reservado para a imagem do post, o texto em três parágrafos, link "Voltar para a página inicial" e o rodapé "© 2024 Meu Blog".](wireframes/post.png)

### Sobre (`sobre.html`)

![Wireframe da página Sobre: seção "Sobre o Blog" com texto de apresentação e formulário "Entre em Contato" com os campos Nome, E-mail, Mensagem e o botão Enviar.](wireframes/sobre-top-section.png)

### Rodapé (comum às três páginas)

![Wireframe do rodapé: faixa estreita com o texto "© 2024 Meu Blog" alinhado à esquerda do conteúdo.](wireframes/footer-outer.png)

## Tecnologias Utilizadas

- **HTML** — linguagem de marcação usada na estrutura das três páginas web.
- **CSS** — folha de estilo única (`assets/css/style.css`) responsável por todo o visual do site: tipografia, cores, layout do cabeçalho e do rodapé em _flexbox_, a moldura da foto de perfil e os efeitos de _hover_ dos links.
- **Markdown** — usado na elaboração deste documento (README.md).
- **Figma** — usado na elaboração dos wireframes.

## Estrutura desse repositório

```text
.
├── assets
│   ├── css
│   │   └── style.css
│   └── img
│       ├── cores.png
│       ├── perfil.jpg
│       └── webdev.jpg
├── wireframes
│   ├── footer-outer.png
│   ├── home-top-section.png
│   ├── post.png
│   └── sobre-top-section.png
├── index.html
├── post.html
├── README.md
└── sobre.html
```

## Cores Utilizadas

| Cor | Código | Onde é usada |
| --- | --- | --- |
| ⬜ Branco | `#ffffff` | Fundo da página e fundo da moldura da foto de perfil. |
| ⬛ Quase preto | `#111111` | Texto principal, links de navegação em destaque e os links "Leia mais" e "Voltar". |
| 🔘 Cinza médio | `#666666` | Links da navegação, texto do rodapé e o _hover_ dos links "Leia mais" e "Voltar". |
| ▫️ Cinza claro | `#cccccc` | Borda inferior do cabeçalho e borda superior do rodapé. |
| ▫️ Cinza claro | `#dddddd` | Borda da moldura da foto de perfil. |
| ▫️ Cinza claro | `#e5e5e5` | Divisória acima do link "Voltar" na página Sobre. |
| Sombra | `rgba(0, 0, 0, 0.1)` | Sombra da moldura da foto de perfil. |
| Sombra | `rgba(0, 0, 0, 0.3)` | Sombra da moldura da foto de perfil ao passar o mouse. |
