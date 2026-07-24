<h1 align="center">Dicas para montar o Markdown</h1>

O Markdown aceita nativamente várias tags HTML para quando você precisa de um controle fino de layout (como alinhamento ou dimensão de imagens) que a sintaxe tradicional do Markdown não cobre.Abaixo está o resumo com as principais equivalências e recursos de estilização HTML que funcionam muito bem no README.md (especialmente no GitHub, GitLab e Bitbucket)

```diff
-CLIQUE NA ABA "CODE" PARA VER O CODIGO HTML
```

<h2 align="center">1. Títulos e HierarquiaEstilo DesejadoSintaxe MarkdownTag HTML EquivalenteTítulo</h2>
    1# Título       <h1>Título</h1>Título
    2## Título      <h2>Título</h2>Título 
    3### Título     <h3>Título</h3>Título 
    4#### Título    <h4>Título</h4>

<h2 align="center">2. Formatação de TextoEstilo DesejadoSintaxe MarkdownTag HTML Equivalente</h2>
Negrito - **texto**   <b>texto</b> ou <strong>texto</strong>
Itálico - *texto*<i>texto</i> ou <em>texto</em>
Riscado - ~~texto~~<s>texto</s> ou <strike>texto</strike>
Sublinhado - (Não tem nativo)<u>texto</u>Texto Menor(Não tem nativo)<small>texto</small>Sobrescrito(Não tem nativo)<sup>texto</sup>Subscrito(Não tem nativo)<sub>texto</sub>
Quebra de linhaEspaço duplo no fim - <br> ou <br />

<h2 align="center">3. Centralização e AlinhamentoPara alinhamento, o HTML usa o atributo</h2>
align:Centralizar Texto ou Título:HTML<h1 align="center">Meu Título Centralizado</h1>
<p align="center">Este parágrafo está centralizado no README.</p>

Alinhar à Direita:HTML
<p align="right">Texto alinhado à direita.</p>

Justificar Texto:HTML
<p align="justify">Texto distribuído uniformemente entre as margens.</p>

<h2 align="center">4. Imagens e Mídias (Controle de Tamanho e Posição)</h2>
O Markdown padrão (![alt](url)) não permite alterar o tamanho da imagem.
Com HTML você controla largura, altura e alinhamento:Centralizar Imagem:
HTML
<p align="center">
  <img src="https://github.com/s-a-m-i-o/wiki-pessoal/blob/main/markdown/logo1.png" alt="Logo do meu site" width="300">
</p>

Imagem ao lado do texto (Float):HTML<img src="link-da-imagem.png" align="left" width="100">
Seu texto aqui vai envolver a imagem do lado esquerdo.

<h2 align="center">5. Blocos Expansíveis (Collapsible / Dropdown)Excelente para esconder detalhes longos, logs de erro ou tutoriais sem poluir o visual principal:</h2>
HTML
<details>
  <summary>Clique para expandir / ver mais</summary>
  
  Aqui dentro você pode colocar qualquer texto, código ou até Markdown!
</details>

<h2 align="center">6. Divisores, Caixas e Detalhes VisuaisLinha Horizontal:</h2>
Markdown: 
---HTML: <hr>Destaque de Código / Teclas:<kbd>Ctrl</kbd> + <kbd>C</kbd> (Gera um visual de tecla do teclado: Ctrl + C).

Aviso de Compatibilidade: Evite usar CSS inline complexo (como <div style="color: red;">) ou tags de scripts <script>), pois o GitHub e a maioria das plataformas de Git removem estilos CSS arbitrários por questões de segurança.
