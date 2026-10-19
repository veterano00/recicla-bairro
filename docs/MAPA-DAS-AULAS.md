# Relação do código com as aulas

Este arquivo ajuda a estudar e explicar o projeto. As páginas abaixo são as páginas dos PDFs fornecidos.

| Recurso do projeto | Material de referência |
| --- | --- |
| `DOCTYPE`, `html`, `head`, `body`, `title`, `meta`, `lang`, títulos, parágrafos e comentários | Aula 1 — HTML, páginas 4–5 |
| `header`, `nav`, `main`, `section`, `article`, `footer`, `div` e `span` | Aula 2 — HTML, páginas 5–8 |
| Links e caminhos relativos/absolutos | Aula 2 — HTML, páginas 9–11 |
| `img`, `src`, `alt`, `width`, `height` | Aula 3 — HTML, páginas 2–4 |
| Material Icons, incluídos por `<link>` e classe `material-icons` | Aula 3 — HTML, páginas 5–6 |
| `figure` e `figcaption` | Aula 3 — HTML, páginas 7–8 |
| `form`, `input`, tipos text/email/password/submit, `label`, `for`, `id` | Aula 3 — HTML, páginas 10–12 |
| `required`, `placeholder` e `method` | Aula 3 — HTML, páginas 13–15 |
| Seletores por elemento, classe, universal, descendentes, agrupamento e `:hover` | Aula 1 — CSS, páginas 6–9 |
| CSS externo | Aula 1 — CSS, página 10 |
| Cores, `color`, `background-color` | Aula 1 — CSS, páginas 13–16 |
| `font-family`, `font-size`, `font-weight`, Google Fonts, `text-decoration`, `text-align` | Aula 1 — CSS, páginas 17–21 |
| `width`, `height`, `margin`, `padding`, `border`, `border-radius`, `box-sizing`, `display`, `overflow` | Aula 2 — CSS, páginas 3–25 |
| `display: flex`, `flex-direction`, `flex-wrap`, `justify-content`, `align-items` | Aula 3 — CSS, páginas 5–14 |
| `flex-grow`, `flex-basis`, `flex-shrink`, abreviação `flex`, limites mínimos e máximos de largura/altura | Aula 3 — CSS, páginas 18–22 |
| `display: grid`, `grid-template-columns`, unidade `fr` e `gap` | Aula 4 — CSS, páginas 4–9 |

## Única adição discutida: action

O enunciado exige que o cadastro encaminhe para o login e que o login encaminhe para a página principal. O atributo `action` não foi localizado nas explicações dos PDFs. Seu uso pontual foi discutido com Vinicius e aceito, mantendo a preferência por seguir estritamente as aulas no restante do código.

```html
<form action="login.html" method="get">
```

`action` indica o arquivo que o navegador deve abrir após a validação dos campos e o envio do formulário. No login, o destino é `index.html`. Não há JavaScript nem autenticação.

O atributo `name` aparece nas aulas, mas foi omitido intencionalmente dos campos desta demonstração. Em um formulário GET, campos com `name` têm seus valores incluídos na URL. Como este projeto somente navega entre arquivos e não processa dados, não é necessário transmitir nome, e-mail ou senha.

## Como entender o CSS

- `.limite`: limita a largura do conteúdo e centraliza a página com `margin: 0 auto`.
- `.apresentacao`, `.materiais` e `.passos`: organizam as partes lado a lado com Flexbox.
- `flex-wrap: wrap`: permite que as partes desçam quando o espaço diminui.
- `flex: 1 1 190px`: combina crescimento, redução e tamanho inicial dos cartões.
- `.formulario`: usa uma coluna de Grid, separando os campos com `gap`.
- `.papel`, `.plastico`, `.vidro`, `.metal` e `.organico`: definem a cor de cada grupo.
- `.botao` e `.botao:hover`: definem a aparência normal e ao passar o mouse.

`gap` é apresentado no PDF de Grid e foi também aplicado aos contêineres Flexbox; tem a mesma função de espaçamento entre itens.

Os arquivos SVG em `imagens` são recursos visuais baixados do OpenMoji e usados como qualquer imagem em `<img>`. Não é necessário editar sua marcação. Os arquivos CSS fornecidos pelo Google são recursos externos de fonte/ícones, conforme a técnica demonstrada nas aulas.

Não foram utilizados media queries, variáveis CSS, animações, posicionamento absoluto, bibliotecas de componentes, JavaScript ou frameworks.
