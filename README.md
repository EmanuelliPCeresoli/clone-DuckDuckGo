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

  - **Dia 3:** definição de todas as variáveis do projeto no bloco :root.
Paleta de cores: 8 cores base extraídas de uma paleta terrosa (Coffee 
#371e13, Maroon 
#5e2a25, Clay Dust 
#c0aa8a, Creme 
#e1d3a9, Leather Couch 
#734f31, Deep Peach 
#a85530, Guave 
#8f7c3a, River Pine 
#534831), escolhida para um tema escuro que substitui a paleta original do DuckDuckGo (item de personalização visual, já que o professor pediu que a aparência não fosse uma réplica do site de referência).
Papéis atribuídos a cada cor: cada variável de cor base foi associada a uma função na página (fundo, texto principal, texto secundário, fundo dos cards, bordas, botões primário e secundário, selo, campos de formulário, foco de teclado), para que trocar a paleta inteira no futuro exija mexer só nesse bloco.
Antes de decidir os papéis, foi feito um cálculo de contraste (WCAG) entre as cores da paleta, para garantir texto legível sobre os fundos escolhidos e evitar problemas de acessibilidade.
Variáveis de tipografia e espaçamento: fonte base (pilha de fontes do sistema, system-ui), raio de borda padrão para cards e botões (12px) e espaçamento padrão entre seções (3rem), centralizando esses valores para reutilização em todo o CSS.
Corrigido também um problema de nome de arquivo: Style.css (maiúsculo) estava commitado com nome diferente do usado no index.html, o que poderia impedir o CSS de carregar em sistemas que diferenciam maiúsculas de minúsculas. Renomeado para style.css com git mv.

 **Reset:** `box-sizing: border-box` em todos os elementos (facilita o cálculo de
    padding/borda sem estourar larguras), remoção da margem padrão do `body`, e
    imagens limitadas a `max-width: 100%` para não estourar o layout em telas menores.
  - **Tipografia:** fonte, cor de fundo e cor de texto aplicadas ao `body` a partir
    das variáveis já definidas; tamanhos de `h1` e `h2` definidos para mobile
    (ajustados depois na media query de desktop); parágrafos com largura máxima de
    `65ch` para manter linhas de texto confortáveis de ler; links herdando a cor do
    texto ao redor, em vez do azul padrão do navegador.
  - **Acessibilidade:** contorno (`outline`) visível ao navegar por teclado (Tab) em
    links, botões e campos de formulário, usando a cor Guave como destaque de foco.
  