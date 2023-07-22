# Propriedades CSS

## Propriedades de Codificação e Importação:
- `@charset`: Define a codificação de caracteres em uma folha de estilo CSS.
- `@import`: Importa folhas de estilo CSS externas.
- `@font-face`: Importa fontes externas.
- `@keyframes`: Define as propriedades CSS para animação.
- `@media`: Permite a utilização de diferentes propriedades CSS para diferentes tipos de telas.

## Propriedades de Formatação de Texto:
- `widows`: Especifica o número mínimo de linhas que devem ser deixadas no topo de uma coluna ou página.
- `orphans`: Especifica o número mínimo de linhas que devem ser deixadas no final de uma coluna ou página.

## Propriedades de Redefinição:
- `all`: Redefine todas as propriedades do elemento, exceto `unicode-bidi` e `direction`.

## Propriedades de Layout e Posicionamento:
- `display`: Especifica o tipo de display.
- `float`: Especifica uma flutuação.
- `clear`: Especifica a posição de um elemento próximo a um elemento flutuante.
- `columns`: Especifica as propriedades: `column-width` e `column-count`.
- `column-width`: Especifica a largura das colunas.
- `column-count`: Especifica o número de colunas de um elemento.
- `column-fill`: Especifica como as colunas são preenchidas.
- `column-span`: Especifica quantas colunas um elemento de bloco deve preencher.
- `column-rule`: Especifica as propriedades: `column-rule-width`, `column-rule-style` e `column-rule-color`.
- `column-rule-width`: Especifica a largura da regra vertical.
- `column-rule-style`: Especifica o estilo da regra vertical.
- `column-rule-color`: Especifica a cor da regra vertical.
- `flex`: Especifica as propriedades: `flex-grow`, `flex-shrink` e `flex-basis`.
- `flex-grow`: Especifica como o item cresce em relação aos demais no container flexível.
- `flex-shrink`: Especifica como o item diminui em relação aos demais no container flexível.
- `flex-basis`: Especifica o tamanho inicial dos itens no container flexível.
- `flex-flow`: Especifica as propriedades: `flex-direction` e `flex-wrap`.
- `flex-direction`: Especifica a direção do container flexível.
- `flex-wrap`: Especifica se os itens no container flexível devem quebrar a linha.
- `justify-content`: Especifica o alinhamento dos itens no container flexível seguindo a direção definida no `flex-direction`.
- `align-content`: Especifica o alinhamento das linhas dos itens no container flexível.
- `align-items`: Especifica o alinhamento dos itens no container flexível seguindo a direção contrária definida no `flex-direction`.
- `align-self`: Especifica o alinhamento individual de um item no container flexível.
- `order`: Especifica a ordem do item em relação aos demais no container flexível.
- `grid`: Especifica as propriedades: `grid-template-rows`, `grid-template-columns`, `grid-template-areas`, `grid-auto-rows`, `grid-auto-columns` e `grid-auto-flow`.
- `grid-template`: Especifica as propriedades: `grid-template-rows`, `grid-template-columns` e `grid-template-areas`.
- `grid-template-rows`: Especifica o tamanho para cada linha no container gradeado.
- `grid-template-columns`: Especifica o número de colunas e o tamanho para cada coluna no container gradeado.
- `grid-template-areas`: Especifica áreas com identificadores no container gradeado.
- `grid-auto-rows`: Especifica um tamanho padrão para as linhas no container gradeado.
- `grid-auto-columns`: Especifica um tamanho padrão para as colunas no container gradeado.
- `grid-auto-flow`: Especifica como os itens são inseridos no container gradeado.
- `grid-row`: Especifica as propriedades: `grid-row-start` e `grid-row-end`.
- `grid-column`: Especifica as propriedades: `grid-column-start` e `grid-column-end`.
- `grid-area`: Especifica as propriedades: `grid-row-start`, `grid-column-start`, `grid-row-end` e `grid-column-end`.
- `grid-row-start`: Especifica em qual linha um item começa no container gradeado.
- `grid-column-start`: Especifica em qual coluna um item começa no container gradeado.
- `grid-row-end`: Especifica em qual linha um item termina no container gradeado.
- `grid-column-end`: Especifica em qual coluna um item termina no container gradeado.
- `gap`: Especifica as propriedades: `row-gap` e `column-gap` no container gradeado.
- `row-gap`: Especifica o tamanho do espaço entre as linhas no container gradeado.
- `column-gap`: Especifica o espaço entre as colunas no container gradeado.
- `vertical-align`: Especifica o alinhamento vertical de um elemento inline.
- `position`: Especifica o tipo de posicionamento.
- `left`: Especifica a distância até a esquerda.
- `right`: Especifica a distância até a direita.
- `top`: Especifica a distância até o topo.
- `bottom`: Especifica a distância até o fundo.
- `z-index`: Especifica a ordem na pilha de renderização no eixo-z.
- `isolation`: Especifica uma ordem de pilha isolada para o elemento.
- `object-fit`: Especifica como os elementos `img` e `video` devem ser redimensionados dentro dos próprios containers.
- `object-position`: Especifica a posição dos elementos `img` e `video` dentro dos próprios containers.
- `visibility`: Especifica a visibilidade.
- `opacity`: Especifica a opacidade.
- `filter`: Adiciona um efeito visual no elemento.
- `box-shadow`: Adiciona uma sombra ao elemento.
- `box-decoration-break`: Especifica como as propried

ades: `box-shadow`, `margin`, `border`, `border-image`, `padding`, `background` e `clip-path` são adicionadas quando o container é fragmentado.
- `mix-blend-mode`: Especifica como um elemento deve se mesclar com o fundo do elemento pai.
- `box-sizing`: Especifica como o container é dimensionado.
- `height`: Especifica a altura.
- `width`: Especifica a largura.
- `max-height`: Especifica a maior altura permitida.
- `max-width`: Especifica a maior largura permitida.
- `min-height`: Especifica a menor altura permitida.
- `min-width`: Especifica a menor largura permitida.

## Propriedades de Borda:
- `outline`: Especifica as propriedades: `outline-width`, `outline-style` e `outline-color`.
- `outline-width`: Especifica a largura do contorno.
- `outline-style`: Especifica o estilo do contorno.
- `outline-color`: Especifica a cor do contorno.
- `outline-offset`: Especifica a distância do contorno.
- `margin`: Especifica todas as propriedades de margem.
- `margin-top`: Especifica a margem superior.
- `margin-bottom`: Especifica a margem inferior.
- `margin-left`: Especifica a margem da esquerda.
- `margin-right`: Especifica a margem da direita.
- `border`: Especifica todas as propriedades de borda.
- `border-color`: Especifica a cor da borda.
- `border-radius`: Especifica o arredondamento da borda.
- `border-width`: Especifica a largura da borda.
- `border-style`: Especifica o estilo da borda.
- `border-collapse`: Especifica se as bordas das células em uma tabela devem se colapsar em uma.
- `border-spacing`: Especifica o espaçamento entre os itens a partir da borda.
- `border-image`: Especifica todas as propriedades de imagem a ser usada como borda.
- `border-image-outset`: Especifica o início da borda.
- `border-image-repeat`: Especifica a repetição da imagem a ser usada como borda.
- `border-image-slice`: Especifica como cortar a imagem a ser usada como borda.
- `border-image-source`: Especifica a fonte da imagem a ser usada como borda.
- `border-image-width`: Especifica a largura da imagem a ser usada como borda.
- `border-top`: Especifica a borda superior.
- `border-top-color`: Especifica a cor da borda superior.
- `border-top-style`: Especifica o estilo da borda superior.
- `border-top-width`: Especifica a largura da borda superior.
- `border-top-left-radius`: Especifica o arredondamento da borda superior da esquerda.
- `border-top-right-radius`: Especifica o arredondamento da borda superior da direita.
- `border-bottom`: Especifica a borda inferior.
- `border-bottom-color`: Especifica a cor da borda inferior.
- `border-bottom-style`: Especifica o estilo da borda inferior.
- `border-bottom-width`: Especifica a largura da borda inferior.
- `border-bottom-left-radius`: Especifica o arredondamento da borda inferior da esquerda.
- `border-bottom-right-radius`: Especifica o arredondamento da borda inferior da direita.
- `border-left`: Especifica a borda da esquerda.
- `border-left-color`: Especifica a cor da borda da esquerda.
- `border-left-style`: Especifica o estilo da borda da esquerda.
- `border-left-width`: Especifica a largura da borda da esquerda.
- `border-right`: Especifica a borda da direita.
- `border-right-color`: Especifica a cor da borda da direita.
- `border-right-style`: Especifica o estilo da borda da direita.
- `border-right-width`: Especifica a largura da borda da direita.

## Propriedades de Preenchimento:
- `padding`: Especifica todas as propriedades de preenchimento.
- `padding-top`: Especifica o preenchimento superior.
- `padding-bottom`: Especifica o preenchimento inferior.
- `padding-left`: Especifica o preenchimento da esquerda.
- `padding-right`: Especifica o preenchimento da direita.

## Propriedades de Fundo:
- `background`: Especifica todas as propriedades de fundo.
- `background-color`: Especifica a cor do fundo.
- `background-image`: Especifica uma imagem de fundo.
- `background-position`: Especifica a posição da imagem de fundo.
- `background-size`: Especifica o tamanho da imagem de fundo.
- `background-repeat`: Especifica se a imagem de fundo deve repetir.
- `background-origin`: Especifica a origem da posição da imagem de fundo.
- `background-clip`: Es

pecifica até onde o fundo deve se estender no container.
- `background-attachment`: Especifica se a imagem de fundo deve rolar com a página.
- `background-blend-mode`: Especifica como as camadas de fundo irão se mesclar.

## Propriedades de Transbordamento e Quebra de Texto:
- `overflow`: Especifica o tratamento para o conteúdo transbordado.
- `overflow-wrap`: Especifica a quebra do conteúdo transbordado.
- `overflow-x`: Especifica o tratamento para o conteúdo transbordado no eixo x.
- `overflow-y`: Especifica o tratamento para o conteúdo transbordado no eixo y.
- `color`: Define a cor do texto.
- `text-align`: Especifica o alinhamento do texto.
- `text-align-last`: Especifica o alinhamento da última linha quando o `text-justify` é definido.
- `text-decoration`: Especifica as propriedades: `text-decoration-line`, `text-decoration-color`, `text-decoration-style` e `text-decoration-thickness`.
- `text-decoration-line`: Especifica a posição da linha decorativa sobre o texto.
- `text-decoration-color`: Especifica a cor da linha decorativa.
- `text-decoration-style`: Especifica o estilo de linha decorativa.
- `text-decoration-thickness`: Especifica a espessura da linha decorativa.
- `text-indent`: Especifica uma indentação ao texto.
- `text-justify`: Especifica a justificação quando o `text-align` é definido com "justify".
- `text-overflow`: Especifica o tratamento para o texto transbordado.
- `text-shadow`: Adiciona uma sombra ao texto.
- `text-transform`: Especifica a capitalização do texto.
- `text-underline-position`: Especifica a posição da linha decorativa.

## Propriedades de Fonte:
- `font`: Especifica todas as propriedades de fonte.
- `font-family`: Especifica a família da fonte.
- `font-style`: Especifica o estilo da fonte.
- `font-size`: Especifica o tamanho da fonte.
- `font-weight`: Especifica o peso da fonte.
- `font-feature-settings`: Permite um maior controle sobre fontes OpenType.
- `font-kerning`: Especifica o uso das informações de kerning.
- `font-size-adjust`: Especifica o controle do tamanho da fonte caso a primeira esteja indisponível.
- `font-variant`: Especifica se o texto deve ser exibido em um small-caps.
- `font-variant-caps`: Especifica glifos alternativos para letras maiúsculas.

## Propriedades de Espaçamento, Linha e Quebra de Palavras:
- `white-space`: Especifica como o espaço em branco é tratado.
- `word-break`: Especifica como as palavras são quebradas.
- `word-wrap`: Especifica como as palavras devem se quebrar.
- `word-spacing`: Especifica o tamanho do espaço entre as palavras.
- `letter-spacing`: Especifica o tamanho do espaço entre as letras.
- `line-height`: Especifica a altura da linha.

## Propriedades de Texto Bi-Direcional:
- `direction`: Especifica a direção do texto no elemento de nível de bloco.
- `unicode-bidi`: Especifica se o texto deve ser substituído para oferecer suporte a outros idiomas.
- `writing-mode`: Especifica se o texto é horizontal ou vertical.
- `tab-size`: Especifica a largura da tabulação.
- `quotes`: Especifica o tipo de aspas para citações.
- `hyphens`: Especifica se um hífen deve ser adicionado e a linha quebrada num texto transbordado.

## Propriedades de Estilo de Lista:
- `list-style`: Especifica todas as propriedades de estilo.
- `list-style-image`: Especifica uma imagem como estilo da lista.
- `list-style-position`: Especifica a posição do estilo da lista.
- `list-style-type`: Especifica o tipo do estilo da lista.

## Propriedades de Tabelas:
- `caption-side`: Especifica o posicionamento da legenda de uma tabela.
- `empty-cells`: Especifica se deve exibir bordas em células vazias em uma tabela.
- `table-layout`: Especifica o algoritmo utilizado na renderização da tabela.

## Propriedades de Máscara e Imagem:
- `mask-image`: Especifica uma camada que serve como máscara para um elemento.
- `mask-origin`: Especifica a origem da posição da máscara.
- `mask-position`: Especifica a posição da máscara.
- `mask-repeat`: Especifica se a máscara deve repetir.
- `mask-size`: Especifica o tamanho da máscara.

## Propriedades de Renderização de Imagem:
- `image-rendering`: Especifica o algoritmo utilizado para o dimensionamento da imagem.

## Propriedades de Comportamento do Mouse e Seleção de Texto:
- `scroll-behavior`: Especifica a animação do scroll ao clicar em um link para a própria página.
- `cursor`: Especifica o tipo de cursor do mouse sobre o elemento.
- `caret-color`: Especifica a cor do cursor em elementos editáveis, como `input` e `textarea`.
- `accent-color`: Especifica a cor de tipos de `input` e `progress`.
- `pointer-events`: Especifica se um elemento reage ao apontamento do mouse.
- `user-select`: Especifica se o texto no elemento é selecionável.

## Propriedades de Transformação e Animação:
- `backface-visibility`: Especifica a visibilidade da face traseira.
- `resize`: Especifica se um elemento é redimensionável.
- `clip-path`: Permite que você corte o elemento no formato desejado.
- `perspective`: Especifica um posicionamento 3D para o elemento.
- `perspective-origin`: Especifica a origem do posicionamento 3D.
- `transform`: Especifica todas as propriedades de transformação.
- `transform-origin`: Especifica a origem da transformação.
- `transform-style`: Especifica o estilo da transformação.
- `transition`: Especifica todas as propriedades de transição.
- `transition-property`: Especifica a propriedade de transição.
- `transition-delay`: Especifica o atraso da transição.
- `transition-duration`: Especifica a duração da transição.
- `transition-timing-function`: Especifica a mudança de velocidade da transição.
- `animation`: Especifica todas as propriedades de animação.
- `animation

-name`: Especifica o nome da animação.
- `animation-duration`: Especifica a duração da animação.
- `animation-timing-function`: Especifica a mudança de velocidade da animação.
- `animation-delay`: Especifica o atraso da animação.
- `animation-iteration-count`: Especifica o número de iterações da animação.
- `animation-direction`: Especifica se a animação será reproduzida para frente, para trás ou alternada.
- `animation-fill-mode`: Especifica o estado do estilo no início/fim da animação.
- `animation-play-state`: Especifica o estado de execução da animação.

## Propriedades de Filtros de Cores:
- `filter`: Aplica efeitos visuais (por exemplo, desfoque, saturação, brilho) em um elemento.

## Propriedades de Efeitos de Visibilidade e Opacidade:
- `visibility`: Especifica a visibilidade de um elemento.
- `opacity`: Especifica a opacidade de um elemento.
- `backdrop-filter`: Aplica um filtro de efeitos visuais no plano de fundo de um elemento.

## Propriedades de Opacidade e Transparência:
- `opacity`: Define a opacidade de um elemento.

## Propriedades de Cor:
- `color`: Define a cor do texto.
- `background-color`: Define a cor do fundo.

## Propriedades de Tamanho e Dimensão:
- `height`: Define a altura de um elemento.
- `width`: Define a largura de um elemento.
- `max-height`: Define a altura máxima de um elemento.
- `max-width`: Define a largura máxima de um elemento.
- `min-height`: Define a altura mínima de um elemento.
- `min-width`: Define a largura mínima de um elemento.

## Propriedades de Margem:
- `margin`: Define a margem ao redor de um elemento.
- `margin-top`: Define a margem superior de um elemento.
- `margin-bottom`: Define a margem inferior de um elemento.
- `margin-left`: Define a margem da esquerda de um elemento.
- `margin-right`: Define a margem da direita de um elemento.

## Propriedades de Espaçamento Interno:
- `padding`: Define o espaço interno dentro do contorno de um elemento.
- `padding-top`: Define o espaçamento interno superior de um elemento.
- `padding-bottom`: Define o espaçamento interno inferior de um elemento.
- `padding-left`: Define o espaçamento interno da esquerda de um elemento.
- `padding-right`: Define o espaçamento interno da direita de um elemento.

## Propriedades de Borda:
- `border`: Define todas as propriedades de borda.
- `border-color`: Define a cor da borda.
- `border-radius`: Define o arredondamento da borda.
- `border-width`: Define a largura da borda.
- `border-style`: Define o estilo da borda.
- `border-top`: Define a borda superior.
- `border-top-color`: Define a cor da borda superior.
- `border-top-style`: Define o estilo da borda superior.
- `border-top-width`: Define a largura da borda superior.
- `border-top-left-radius`: Define o arredondamento da borda superior da esquerda.
- `border-top-right-radius`: Define o arredondamento da borda superior da direita.
- `border-bottom`: Define a borda inferior.
- `border-bottom-color`: Define a cor da borda inferior.
- `border-bottom-style`: Define o estilo da borda inferior.
- `border-bottom-width`: Define a largura da borda inferior.
- `border-bottom-left-radius`: Define o arredondamento da borda inferior da esquerda.
- `border-bottom-right-radius`: Define o arredondamento da borda inferior da direita.
- `border-left`: Define a borda da esquerda.
- `border-left-color`: Define a cor da borda da esquerda.
- `border-left-style`: Define o estilo da borda da esquerda.
- `border-left-width`: Define a largura da borda da esquerda.
- `border-right`: Define a borda da direita.
- `border-right-color`: Define a cor da borda da direita.
- `border-right-style`: Define o estilo da borda da direita.
- `border-right-width`: Define a largura da borda da direita.

## Propriedades de Fundo:
- `background`: Define todas as propriedades de fundo.
- `background-color`: Define a cor do fundo.
- `background-image`: Define uma imagem de fundo.
- `background-position`: Define a posição da imagem de fundo.
- `background-size`: Define o tamanho da imagem de fundo.
- `background-repeat`: Define se a imagem de fundo deve repetir.
- `background-origin`: Define a origem da posição da imagem de fundo.
- `background-clip`: Define até onde o fundo deve se estender no elemento.
- `background-attachment`: Define se a imagem de fundo deve rolar com a página.
- `background-blend-mode`: Define como as camadas de fundo irão se mesclar.

## Propriedades de Espaçamento, Linha e Quebra de Palavras:
- `white-space`: Define como o espaço em branco é tratado.
- `word-break`: Define como as palavras são quebradas.
- `word-wrap`: Define como as palavras devem se quebrar.
- `word-spacing`: Define o tamanho do espaço entre as palavras.
- `letter-spacing`: Define o tamanho do espaço entre as letras.
- `line-height`: Define a altura da linha.

## Propriedades de Texto Bi-Direcional:
- `direction`: Define a direção do texto no elemento de nível de bloco.
- `unicode-bidi`: Define se o texto deve ser substituído para oferecer suporte a outros idiomas.
- `writing-mode`: Define se o texto é horizontal ou vertical.
- `tab-size`: Define a largura da tabulação.
- `quotes`: Define o tipo de aspas para citações.
- `hyphens`: Define se um hífen deve ser adicionado e a linha quebrada num texto transbordado.

## Propriedades de Estilo de Lista:
- `list-style`: Define todas as propriedades de estilo.
- `list-style-image`: Define uma imagem como estilo da lista.
- `list-style-position`: Define a posição do estilo da lista.
- `list-style-type`: Define o tipo do estilo da lista.

## Propriedades de Tabelas:
- `caption-side`: Define o posicionamento da legenda de uma tabela.
- `empty-cells`: Define se deve exibir bordas em células vazias em uma tabela.
- `table-layout`: Define o algoritmo utilizado na renderização da tabela.

## Propriedades de Máscara e Imagem:
- `mask-image`: Define uma camada que serve como máscara para um elemento.
- `mask-origin`: Define a origem da posição da máscara.
- `mask-position`: Define a posição da máscara.
- `mask-repeat`: Define se a máscara deve repetir.
- `mask-size`: Define o tamanho da máscara.

## Propriedades de Renderização de Imagem:
- `image-rendering`: Define o algoritmo utilizado para o dimensionamento da imagem.

## Propriedades de Comportamento do Mouse e Seleção de Texto:
- `scroll-behavior`: Define a animação do scroll ao clicar em um link para a própria página.
- `cursor`: Define o tipo de cursor do mouse sobre o elemento.
- `caret-color`: Define a cor do cursor em elementos editáveis, como `input` e `textarea`.
- `accent-color`: Define a cor de tipos de `input` e `progress`.
- `pointer-events`: Define se um elemento reage ao apontamento do mouse.
- `user-select`: Define se o texto no elemento é selecionável.

## Propriedades de Transformação e Animação:
- `backface-visibility`: Define a visibilidade da face traseira.
- `resize`: Define se um elemento é redimensionável.
- `clip-path`: Permite que você corte o elemento no formato desejado.
- `perspective`: Define um posicionamento 3D para o elemento.
- `perspective-origin`: Define a origem do posicionamento 3D.
- `transform`: Define todas as propriedades de transformação.
- `transform-origin`: Define a origem da transformação.
- `transform-style`: Define o estilo da transformação.
- `transition`: Define todas as propriedades de transição.
- `transition-property`: Define a propriedade de transição.
- `transition-delay`: Define o atraso da transição.
- `transition-duration`: Define a duração da transição.
- `transition-timing-function`: Define a mudança de velocidade da transição.
- `animation`: Define todas as propriedades de animação.
- `animation-name`: Define o nome da animação.
- `animation-duration`: Define a duração da animação.
- `animation-timing-function`: Define a mudança de velocidade da animação.
- `animation-delay`: Define o atraso da animação.
- `animation-iteration-count`: Define o número de iterações da animação.
- `animation-direction`: Define se a animação será reproduzida para frente, para trás ou alternada.
- `animation-fill-mode`: Define o estado do estilo no início/fim da animação.
- `animation-play-state`: Define o estado de execução da animação.

## Propriedades de Filtros de Cores:
- `filter`: Aplica efeitos visuais (por exemplo, desfoque, saturação, brilho) em um elemento.

## Propriedades de Efeitos de Visibilidade e Opacidade:
- `visibility`: Define a visibilidade de um elemento.
- `opacity`: Define a opacidade de um elemento.
- `backdrop-filter`: Aplica um filtro de efeitos visuais no plano de fundo de um elemento.