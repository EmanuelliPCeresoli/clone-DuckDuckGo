RA: 1139729
ALUNA: Emanuelli Prigol Ceresoli
SITE USADO: Navegador DuckDuckGo!
PROFESSOR: Matheus Henrique Barquette

Este repositório contém um clone da página inicial do DuckDuckGo, desenvolvido como trabalho da disciplina [nome da disciplina]. O objetivo é reproduzir a estrutura, as proporções e o layout da página original usando HTML semântico e CSS, com uma paleta de cores própria (tema escuro, tons terrosos) no lugar da paleta original.

- A barra de pesquisa do cabeçalho foi substituída por um link "Saiba mais sobre o desenvolvedor dessa página", que leva a uma seção com apresentação e formulário de contato.
- A paleta de cores é diferente da original, para não ser uma réplica visual completa do site.

## Andamento

- **Dia 1:** README inicial criado, com identificação, link de referência e checklist.
- **Dia 2:** Estrutura inicial do HTML: head com metadados e início do header com o logo.

- Ajustes de conteúdo e revisão da estrutura do `index.html`.
  - Adicionada a imagem real do logo (`img/logo.png`), substituindo o placeholder.
  - Preenchido o texto de apresentação da seção "Sobre o desenvolvedor desta página"
    com informações reais (nome, curso e objetivo do clone), no lugar do texto provisório.
  - Conferido, por meio de teste no navegador sem CSS, que a ordem semântica do HTML
    está correta: logo → nav → título → cards → seção do desenvolvedor com formulário → rodapé.
    Isso confirma que a estrutura (critério 1.1) está pronta antes de iniciar o CSS.
  - Identificadas as imagens que ainda faltam adicionar: `lupa.png`, `navegador.png`,
    `duck-ai.svg` e `escudo.svg`. Definido o tamanho de referência de cada uma
    (ícones pequenos como SVG, ícones de card em ~128×128 px para telas retina).