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
| `sobre.html` | Apresentação pessoal em duas colunas — foto de perfil com moldura à esquerda, biografia à direita — seguida do formulário "Entre em Contato" e do link de retorno à página inicial. |

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

## Linguagens de Marcação

Linguagens de marcação não executam instruções, como fazem as linguagens de programação. Elas usam marcadores, as _tags_, para descrever a estrutura e o significado de um documento. Três delas se destacam, cada uma com uma finalidade distinta:

| Linguagem | Finalidade | Aplicação |
| --- | --- | --- |
| **HTML** (_HyperText Markup Language_) | Descrever a estrutura e o conteúdo de páginas web, definindo o papel de cada elemento na página. Possui um conjunto fixo de _tags_, já definidas pela especificação. | Usado nesse projeto na construção das três páginas do blog. |
| **XML** (_eXtensible Markup Language_) | Armazenar e transportar dados de forma estruturada, sem determinar como eles serão exibidos. É extensível, ou seja, quem escreve o documento cria as próprias _tags_. | Não foi usado nesse projeto. É aplicado em arquivos de configuração, _feeds_ RSS e na troca de dados entre sistemas diferentes. |
| **Markdown** | Formatar textos de maneira simples e legível, usando uma sintaxe enxuta que depois é convertida em HTML. | Usado na elaboração desse documento (README.md). |

A diferença central está no propósito de cada uma: o HTML se preocupa com a **apresentação estruturada** do conteúdo para o navegador, o XML se preocupa com os **dados** em si e não com sua exibição, e o Markdown se preocupa com a **escrita**, sendo uma alternativa mais leve ao HTML para documentos de texto.

Outros exemplos de linguagens de marcação são o XHTML, uma versão do HTML que segue as regras mais rígidas do XML; o SVG, usado para descrever imagens vetoriais; e o LaTeX, voltado para a produção de documentos científicos.

## Tecnologias Utilizadas

- **HTML** — linguagem de marcação usada na estrutura das três páginas web.
- **CSS** — folha de estilo única (`assets/css/style.css`) responsável por todo o visual do site: tipografia, cores, layout do cabeçalho e do rodapé em _flexbox_, a moldura da foto de perfil e os efeitos de _hover_ dos links.
- **Markdown** — usado na elaboração desse documento (README.md), conforme detalhado na seção acima.
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

A paleta foi mantida propositalmente enxuta, em tons de cinza, para que o foco ficasse no conteúdo do blog.

| Cor | Código | Onde é usada |
| --- | --- | --- |
| ⬜ Branco | `#ffffff` | Fundo da página, fundo da moldura da foto de perfil, fundo dos campos do formulário e texto do botão "Enviar". |
| ⬛ Quase preto | `#111111` | Texto principal, links de navegação em destaque, os links "Leia mais" e "Voltar", fundo do botão "Enviar" e a borda dos campos do formulário quando estão em foco. |
| 🔘 Cinza médio | `#666666` | Links da navegação, texto do rodapé, o _hover_ dos links "Leia mais" e "Voltar" e o _hover_ do botão "Enviar". |
| ▫️ Cinza claro | `#cccccc` | Borda inferior do cabeçalho, borda superior do rodapé e borda dos campos do formulário. |
| ▫️ Cinza claro | `#dddddd` | Borda da moldura da foto de perfil. |
| ▫️ Cinza claro | `#e5e5e5` | Divisórias das seções "Entre em Contato" e do link "Voltar", e fundo dos trechos de código citados no post. |
| Sombra | `rgba(0, 0, 0, 0.1)` | Sombra da moldura da foto de perfil. |
| Sombra | `rgba(0, 0, 0, 0.3)` | Sombra da moldura da foto de perfil ao passar o mouse. |

## Decisões Técnicas

Abaixo estão registradas as escolhas feitas durante a construção do website e as razões por trás delas.

- **CSS externo em um único arquivo.** Todo o estilo foi centralizado em `assets/css/style.css`, em vez de usar estilos internos ou por atributo. Como o cabeçalho e o rodapé se repetem nas três páginas, um arquivo único evita a duplicação de código e faz com que qualquer ajuste no visual valha para o site inteiro de uma só vez.

- **Elementos semânticos no lugar de `div` genéricas.** Foram usados `header`, `nav`, `main`, `article`, `section` e `footer` para delimitar as regiões das páginas. Além de deixar o código mais legível, isso permite que leitores de tela e mecanismos de busca entendam o papel de cada parte do documento, o que uma `div` sozinha não comunica.

- **_Flexbox_ para o leiaute.** O cabeçalho, o rodapé e as duas colunas da página Sobre foram organizados com _flexbox_. A escolha se deu porque o leiaute é simples e unidimensional, alinhando elementos em uma única direção por vez, situação em que o _flexbox_ resolve o problema com menos código do que alternativas como o posicionamento absoluto.

- **Fonte do sistema.** Foi declarada uma pilha iniciada em `system-ui`, aproveitando a fonte padrão do sistema operacional do visitante. Isso evita o carregamento de fontes externas, deixando o site mais rápido, e garante um texto que já é familiar a quem está lendo.

- **Classe `.ativo` no menu.** O link da página em que o visitante se encontra recebe destaque em negrito e sublinhado. É um recurso simples de usabilidade, que responde à pergunta "em que parte do site eu estou" sem precisar de nenhum script.

- **Validação do formulário pelo navegador.** Os campos usam `required` e o campo de e-mail usa `type="email"`. Como a unidade curricular trata de HTML e CSS, a validação foi deixada a cargo dos próprios recursos nativos do HTML5, sem recorrer a JavaScript.

- **`label` associado a cada campo.** Cada rótulo do formulário usa o atributo `for` apontando para o `id` do campo correspondente. Isso amplia a área clicável do campo e, principalmente, faz com que leitores de tela anunciem corretamente o que deve ser preenchido.
