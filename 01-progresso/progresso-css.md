Metodologia das Aulas

Projeto novo a cada aula, com repositório no GitHub
Professor ensina, pergunta, aluno tenta, professor corrige
Respostas não são dadas diretamente — o aluno é guiado a pensar
Se algo não ficou claro, o professor explica de novo de forma mais simples
Sugestões de melhoria são dadas quando faz sentido
Resumo no final de cada aula para atualizar o progresso.md

#progresso das Aulas

## Aula 1 - Diagnóstico HTML e CSS
- Nível atual: intermediário alto em HTML e CSS
- Semântica HTML: header, nav, main, section, footer
- Hierarquia de títulos: h1 → h2 → h3
- Box model e box-sizing: border-box
- Variáveis CSS com :root
- Flexbox aplicado em cards e navegação
- 100vh: quando usar e quando não usar
- Mobile First: conceito e filosofia
- Media queries: sintaxe e breakpoints

## Aula 2 - Git pelo terminal
- git init, git add, git commit, git log
- git remote add origin, git push
- Repositório criado: https://github.com/s-a-m-i-o/projeto-git
- Responsividade com Mobile First
- Media queries na prática
- Espaçamento com padding em vez de altura fixa
- Seletores perigosos com vígula
- Fluxo git completo num projeto real
- Criar e conectar repositório do zero

## Aula 3 - projeto : Quadro de Anúncios
- Repositório: https://github.com/s-a-m-i-o/quadro-de-anuncios
- Objetivo: viewer de imagens semanais com navegação anterior/próxima
- Mobile First desde o início
- Criado site HTML CSS e JS
- HTML semantico, importado links externos no head (googleFots, font awesome)
- CSS: separado por, reset, root e estilo, tres arquivos diferentes
- JS: função addEventListener: botão direiro proxima imagem, botão esquerdo imagem anterior

## Continuação da aula 3
- JS: Adicionado um Stop na primeira e ultima imagem
- Criando novo Index e paginas - REUNIÃO DA SEMANA, REUNIÃO PUBLICA, LIMPEZA e PREGAÇÃO
- Adicionado botão de voltar nas paginas
- JS: Adiciondo menu hamburger
- Criado README.md
- Finalizar projeto e adicionar README
- Projeto finalizado e publicado - https://s-a-m-i-o.github.io/quadro-de-anuncios/

## Aula 4 - CSS Avançado: Animações e Transitions

- Repositório: https://github.com/s-a-m-i-o/transitions_animacoes
- Projeto: Portfólio fictício de Bruce Wayne
- Comandos novos do terminal: mkdir, touch, mv
- transition: suaviza mudança entre estados, precisa de um gatilho (:hover, :focus, etc)
- Sintaxe do transition: propriedade duração timing
- transform: propriedade ideal pra animar, não afeta o layout ao redor
- Funções do transform: translateX, translateY, scale, rotate, skew
- @keyframes: define os quadros da animação com porcentagens (0%, 50%, 100%)
- animation: chama o @keyframes pelo nome e define duração, timing e repetição
- Diferença entre transition e animation: transition precisa de gatilho, animation roda sozinha
- Timing functions na prática: linear ideal pra rotação contínua, ease-in-out pra movimentos naturais
- Variáveis CSS funcionam pra qualquer valor, não só cores
- Página de exemplos criada com vários modelos de animações combinando transform, cores e box-shadow

## Aula 5 - CSS Avançado: Pseudo-elementos e Seletores Avançados

- Repositório: https://github.com/s-a-m-i-o/pseudo-elementos
- Projeto: Card de produto com selo de oferta e animação
- ::before e ::after: criam elementos "fantasma" antes e depois do conteúdo, sem tocar no HTML
- content é obrigatório nos pseudo-elementos, mesmo vazio content: ""
- Pseudo-elementos precisam de display: block ou display: flex pra aceitar width e height
- position: relative no pai + position: absolute no filho = filho se posiciona em relação ao pai
- Diferença entre pseudo-classes (:): representam um estado — e pseudo-elementos (::): criam uma parte do elemento

- - Seletores avançados:

- :first-child — seleciona o primeiro filho
- :last-child — seleciona o último filho
- :nth-child(n) — seleciona o filho pela posição
- :not() — seleciona todos exceto o especificado
- > — seleciona apenas filhos diretos
- + — seleciona o elemento imediatamente após outro
- ~ — seleciona todos os irmãos após um elemento

## Aula 6 - CSS Avançado: CSS Grid

- Repositório: https://github.com/s-a-m-i-o/css-grid
- Projeto: Dashboard com layout completo usando Grid
- CSS Grid trabalha em duas dimensões (linhas e colunas) diferente do Flexbox que trabalha em uma
- display: grid transforma o elemento em container Grid
- grid-template-columns define o tamanho e quantidade de colunas
- grid-template-rows define o tamanho e quantidade de linhas
- Unidade fr (fraction) ocupa o espaço disponível restante
- grid-column: 1/3 faz o elemento ocupar da linha de grade 1 até a 3 (duas colunas)
- Os números do grid-column representam as linhas de grade, não as colunas
- Grid aninhado: um grid dentro de outro, contextos independentes que não conflitam
- Flex e Grid podem ser usados juntos no mesmo projeto
- ::after pode ser usado como elemento fantasma para equilibrar layout flex

## Aula 7 - Reforço: Flexbox Completo e Position

- Repositório: https://github.com/s-a-m-i-o/reforco-flexbox
- Projeto: Página de experimentos com Flexbox e Position

- flex-wrap: wrap - elementos quebram pra próxima linha quando não couberem (usado em grids de cards)
- gap: espaço entre elementos, melhor que margin pq não afeta as bordas externas (ex: gap: 20px 40px - primeiro linhas, segundo colunas)
- align-content: alinha as linhas inteiras no eixo vertical, só funciona com flex-wrap: wrap (ex: space-between entre linhas de cards)
- flex-grow: define quanto o elemento cresce em proporção (ex: grow: 1 todos iguais, grow: 2 dobro dos outros)
- flex-shrink: define quanto o elemento encolhe em proporção (ex: shrink: 0 não encolhe nunca)
- flex-basis: tamanho base do elemento antes de crescer ou encolher (ex: basis: 200px começa com 200px)
- flex: atalho que combina os três - flex: grow shrink basis (ex: flex: 0 1 200px para cards)
- Para cards usar flex: 0 1 200px - não cresce, encolhe se precisar, começa com 200px
- align-self: alinha um filho específico diferente dos outros (ex: item2 no fundo enquanto outros ficam no topo)
- order: muda a ordem visual sem mexer no HTML (ex: order: 1 aparece antes de order: 2)

- display: block - ocupa a linha inteira, empurra próximo elemento pra baixo (ex: div, p, h1)
- display: inline - fica no fluxo do texto, não aceita width/height (ex: span, a, strong)
- display: inline-block - fica no fluxo do texto mas aceita width/height (ex: destacar palavra com tamanho definido)
- display: flex - controle total dos filhos do container (ex: alinhar cards lado a lado)

- position: static - padrão de todo elemento, segue o fluxo normal da página
- position: relative - serve de referência pro absolute do filho, e move o elemento em relação à sua própria posição original
- position: absolute - sai do fluxo da página, se posiciona em relação ao pai com position relative (ex: selo de oferta no card)
- position: fixed - fica fixo na janela do navegador independente do scroll (ex: menu hamburger no mobile)
- position: sticky - rola com a página mas gruda quando chega no ponto definido (ex: header que gruda no topo ao rolar)
- Centralizar com position: top: 50%, left: 50%, transform: translate(-50%, -50%)
- top, right, bottom, left: definem a posição do elemento a partir de cada lado

## Aula 8 - CSS Moderno: clamp(), :has() e Container Queries

- Repositório: https://github.com/s-a-m-i-o/css-moderno
- Projeto: Página de experimentos com CSS moderno

- clamp(): define um valor com mínimo, ideal e máximo - clamp(16px, 4vw, 48px)
- clamp() escala suavemente diferente das media queries que mudam de forma abrupta
- vw = porcentagem da largura da tela, vh = porcentagem da altura da tela
- clamp() funciona pra qualquer valor numérico: font-size, width, padding, gap
- clamp() e media queries se complementam: clamp() pra valores que escalam, media queries pra mudanças de layout

- :has() seleciona um elemento baseado no que ele contém
- .card:has(img) = seleciona todo card que tem uma imagem dentro
- :has() permite estilizar o pai baseado no filho, sem classes extras no HTML
- :has() pode trabalhar sozinho (estrutura do HTML) ou com JS (classes dinâmicas)

- container-type: inline-size - define o elemento como ponto de referência pro container query
- @container (min-width: 400px) - aplica estilo quando o container tiver aquela largura
- container queries olham o tamanho do elemento pai, media queries olham o tamanho da tela
- min-width: ativa quando a tela for maior ou igual ao valor (Mobile First)
- max-width: ativa quando a tela for menor ou igual ao valor (Desktop First)
- Mobile First usa min-width, Desktop First usa max-width

## Aula 9 - Responsividade com Mobile First

- Repositório: https://github.com/s-a-m-i-o/mobile-first
- Projeto: Landing page de portfólio fictício completa

- Mobile First: começar o CSS pelo mobile, adicionar media queries pra telas maiores
- No mobile elementos em coluna (flex-direction: column), no desktop em linha (flex-direction: row)
- min-width nas media queries pro Mobile First, max-width pro Desktop First
- Wireframe e README.md pra planejar o projeto antes de codar (cores, fontes, layout)
- Separar CSS em arquivos por função: reset, root, global, landinpage, responsivo, animacoes
- Reset profissional: img com max-width 100% e display block, font inherit nos inputs, list-style none
- h2 com display block e width 100% dentro do flex-wrap pra ocupar linha inteira
- min-height em vez de height fixo nos cards pra não cortar conteúdo
- Abordagem de CSS separado por função é ideal pra projetos médios
- Dois @media iguais podem ser unidos em um só bloco
- Hover nos ícones de redes sociais com filter drop-shadow colorido
- position sticky pra headers que grudam no topo, fixed pra elementos sempre visíveis

## Provas Finais de CSS

- Prova 1 - HTML: 7,4/10 - Aprovado
- Pontos fracos: sintaxe do meta charset/viewport, conceito de atributos HTML

- Prova 2 - CSS: 6,6/10 - Aprovado com ressalvas
- Pontos fracos: scale sem deg no @keyframes, min-width vs max-width no Mobile First, sintaxe do CSS Grid

- Prova 3 - HTML + CSS: 9,4/10 - Aprovado com excelência
- Pontos de atenção: type email nos inputs, min-height em vez de height fixo, @keyframes pulsar começar em scale(1)

-(link da prova final) https://github.com/s-a-m-i-o/prova-final-html-css/tree/main