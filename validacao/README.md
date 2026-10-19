# Validação do código

Os resultados abaixo foram obtidos em **18/10/2026** a partir dos arquivos deste diretório, antes de publicação no GitHub Pages.

## HTML — Nu Html Checker, W3C

A opção **text input** foi usada no [Nu Html Checker](https://validator.w3.org/nu/) para validar o conteúdo de cada arquivo HTML. Em todos os casos, o resultado foi: **“Document checking completed. No errors or warnings to show.”**

| Arquivo | Resultado em JSON da API oficial | Print da interface |
| --- | --- | --- |
| `index.html` | [index.json](index.json) | [index-w3c.jpg](index-w3c.jpg) |
| `cadastro.html` | [cadastro.json](cadastro.json) | [cadastro-w3c.jpg](cadastro-w3c.jpg) |
| `login.html` | [login.json](login.json) | [login-w3c.jpg](login-w3c.jpg) |

Os arquivos JSON foram recebidos da API do W3C e têm a lista `messages` vazia.

## CSS — W3C CSS Validation Service

O conteúdo de `css/style.css` foi enviado pela opção **Por entrada direta** no [validador CSS da W3C](https://jigsaw.w3.org/css-validator/), com perfil **CSS nível 3 + SVG**. O serviço respondeu: **“Parabéns! Não foram encontrados erros na sua folha de estilo.”** O resultado apresentou **2 alertas de nível 1**, referentes às declarações de cores de `.botao.claro` e `.botao.claro:hover`. Esses alertas não são erros de sintaxe e não impedem a validação.

O [relatório HTML salvo](css-resultado-w3c.html) é uma cópia da resposta original do serviço. Foi adicionada apenas uma tag `<base>` para que as folhas de estilo e links relativos continuem apontando para a W3C ao abrir a cópia local. Nenhum texto do resultado foi editado.

Após a publicação, o CSS foi [validado pela URL pública](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fveterano00.github.io%2Frecicla-bairro%2Fcss%2Fstyle.css), também sem erros. O [print CSS](css-w3c.jpg) é uma captura da [resposta textual oficial](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fveterano00.github.io%2Frecicla-bairro%2Fcss%2Fstyle.css&output=text) da W3C, que inclui a URL analisada e a mensagem de sucesso. A captura da versão visual do serviço saía em branco; a opção `output=text` preservou o resultado oficial e permitiu registrar um print legível.
