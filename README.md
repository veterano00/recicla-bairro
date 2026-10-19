# Recicla Bairro

Projeto 1 da disciplina **Programação Web Front-End — 2026/02**, da UTFPR, professora Rosangela Marquesone.

**Integrante:** Vinicius Ortiz Sian (trabalho individual).  
**Currículo:** [veterano00.github.io/curriculo_web_front](https://veterano00.github.io/curriculo_web_front/).

## Proposta

O Recicla Bairro é uma proposta de serviço educativo para ajudar moradores a separar resíduos domésticos e procurar orientação sobre a coleta seletiva de sua cidade. O público-alvo são pessoas da comunidade que querem começar a reciclar, mas têm dúvidas sobre os materiais e seus destinos.

O projeto está relacionado ao **ODS 12 — Consumo e produção responsáveis**, especialmente à meta 12.5, sobre prevenção, redução, reciclagem e reúso de resíduos. A página diferencia os recicláveis secos dos resíduos orgânicos e orienta a consultar o serviço municipal; não apresenta pontos de coleta fictícios.

## Páginas e funcionamento

- `index.html`: página principal, guia de cinco grupos de resíduos, orientações, apresentação do ODS e fontes de informação.
- `cadastro.html`: formulário com cinco campos obrigatórios: nome, e-mail, cidade, bairro e senha. Após preenchimento válido, o botão abre `login.html`.
- `login.html`: campos obrigatórios de e-mail e senha. O botão abre `index.html`.

Esta é a etapa de **HTML e CSS**. O cadastro e o login são demonstrativos: não criam contas, não verificam credenciais e não armazenam informações. Utilize dados fictícios. Os campos não possuem `name`, evitando que seus valores sejam incluídos na URL ao navegar. A validação de campo obrigatório e formato de e-mail é feita pelo próprio HTML.

## Tecnologias

- HTML5 com tags semânticas.
- CSS externo, modelo de caixa, Flexbox e Grid.
- Google Fonts: **DM Sans**, para títulos e botões, e **Arial**, para os demais textos.
- Material Icons do Google, conforme o recurso apresentado nas aulas.
- Cinco imagens locais do OpenMoji, usadas por meio de `<img>`.

Não utiliza JavaScript, frameworks, gerenciador de pacotes ou processo de compilação. Os arquivos SVG são imagens prontas de terceiros, não componentes nem código de aplicação.

A organização se adapta a larguras diferentes com `flex-wrap` e dimensões flexíveis, sem media queries. O arquivo [mapa das aulas](docs/MAPA-DAS-AULAS.md) relaciona os recursos com os PDFs. O atributo `action` foi a única adição explicitamente discutida e aceita pelo autor para cumprir o fluxo de navegação exigido no enunciado.

## Como abrir

1. Baixe ou clone o repositório.
2. Abra `index.html` em um navegador, mantendo as pastas `css` e `imagens` ao lado dele.
3. Opcionalmente, abra a pasta no VS Code e use **Open with Live Server**.
4. Teste `Participar`, preencha os cinco campos com dados fictícios, envie e faça o mesmo no login.

As imagens e o CSS estão no projeto. É necessária conexão com a internet para carregar a fonte DM Sans e os Material Icons. Se a fonte externa não carregar, os textos usam Arial como alternativa.

## Estrutura

```text
.
├── index.html
├── cadastro.html
├── login.html
├── css/
│   └── style.css
├── imagens/
│   ├── papel.svg
│   ├── plastico.svg
│   ├── vidro.svg
│   ├── metal.svg
│   ├── organico.svg
│   └── CREDITOS.md
├── docs/
│   ├── MAPA-DAS-AULAS.md
│   ├── ROTEIRO-VIDEO.md
│   ├── ENTREGA.md
│   └── previa-desktop.jpg
├── validacao/
│   └── README.md
├── entrega-modelo.txt
└── README.md
```

## Requisitos atendidos na implementação

| Requisito | Implementação |
| --- | --- |
| Página principal | `index.html` |
| Cadastro com 5 ou mais campos | 5 campos obrigatórios em `cadastro.html` |
| Login com e-mail e senha | `login.html` |
| Navegação cadastro → login → principal | `action` dos formulários |
| Cabeçalho, rodapé e menu | `header`, `footer` e `nav` |
| 2 ou mais ícones | `recycling`, `eco`, `home`, `groups` e outros |
| 4 ou mais caixas de texto | Parágrafos de apresentação, materiais, passos e projeto |
| 5 ou mais imagens | 5 imagens diferentes, com 8 ocorrências de `<img>` |
| 3 ou mais links | Menu, páginas, fontes oficiais e currículo |
| 4 ou mais cores | Verde, azul, vermelho, amarelo, marrom e tons neutros |
| 2 fontes, uma externa | DM Sans (Google Fonts) e Arial |
| Currículo no rodapé | Link de Vinicius Ortiz Sian |

Consulte [os registros de validação](validacao/README.md) e [o checklist de entrega](docs/ENTREGA.md) para distinguir a implementação concluída das etapas de publicação e apresentação.

## Publicação no GitHub Pages

Os arquivos estão preparados para publicação estática pela raiz do repositório. O site ainda não foi publicado a partir desta pasta. O passo a passo está em [docs/ENTREGA.md](docs/ENTREGA.md).

## Fontes e créditos

- [ODS 12 — Nações Unidas no Brasil](https://brasil.un.org/pt-br/sdgs/12).
- [O que é reciclagem — Ministério do Meio Ambiente](https://www.gov.br/mma/pt-br/assuntos/educacao-ambiental/glossario-ea/o-que-e-reciclagem).
- [Coleta seletiva — Prefeitura de Belo Horizonte](https://prefeitura.pbh.gov.br/slu/informacoes/reciclavel/levs), apresentado como exemplo municipal, não como serviço de outra cidade.
- [OpenMoji](https://openmoji.org/): ilustrações sob [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/), com os créditos detalhados em [imagens/CREDITOS.md](imagens/CREDITOS.md).
- [Google Fonts](https://fonts.google.com/) e [Material Icons](https://fonts.google.com/icons).

## Apresentação

Há um [roteiro de até 3 minutos](docs/ROTEIRO-VIDEO.md), que deve ser estudado e adaptado à sua maneira de falar. O vídeo precisa mostrar o autor, as três páginas e a estrutura do código. A gravação e a entrega no Moodle ainda precisam ser feitas.
