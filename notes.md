## O que é HTML:

HTML (Linguagem de Marcação de HiperTexto) é o bloco de construção mais básico da web. Define o significado e a estrutura do conteúdo da web.

"Hipertexto" refere-se aos links que conectam páginas da Web entre si, seja dentro de um único site ou entre sites. Links são um aspecto fundamental da web. Ao carregar conteúdo na Internet e vinculá-lo a páginas criadas por outras pessoas, você se torna um participante ativo na world wide web.

## Tags:

As tags são as marcações do HTML. Tais tags constituem os elementos da linguagem de marcação, que podem ser com fechamento ou vazios.

Um elemento HTML é separado de outro texto em um documento por "tags", que consistem no nome do elemento entre "<" e ">".

Exemplo:

```html
<h1>Título</h1>
<strong>Negrito</strong>
<!-- elemento com fechamento -->

<img src="" alt="" />
<input type="text" />
<!-- elementos vazios -->
```

## Atributos:

Elementos HTML possuem atributos, que servem como informações extras para colocarmos nos elementos ou configurações puras.

```html
<img src="conteúdo do atributo" alt="texto alternativo" />
```

Os atributos booleanos não precisam de conteúdo. Por exemplo, o _disabled_.

```html
<input type="text" disabled />
```

Atributos globais servem para todo o HTML, onde mais de um elemento pode receber essa tag, como "class", utilizada para aplicar estilos CSS.

Atributos globais mais utilizados: class, contenteditable, data-\*, hidden, id, style, tabindex, title.

Já os atributos específicos são aqueles onde cada elemento possui seu próprio atributo.

## Aninhamento de tags:

Podemos escrever tags dentro de outras, por exemplo:

```html
<div>
  <p>Vou <em>escrever</em> em itálico.</p>
</div>
```

Nesse caso, a tag "em" é filha das tags "p" e "div", que é a tag pai.

Existe o posicionamento dos elementos. Algumas tags ficarão em linha, não quebrarão para a próxima, mas a outras sim, como a tag "p", que faz um bloco no texto:

```html
<p>
  Aqui é um texto em uma linha.
  <p>Outro texto em outra linha.</p>
</p>
```

## Caracteres reservados:

Se eu quisesse fazer uma quebra de linha, poderia usar a tag "br" (break). Mas se quisesse, de fato, colocar espaços, teria que usar caracteres bem diferentes, como "&npsp;".

Alguns caracteres reservados são: "&", ">", "<" e " ' ". Mas posso utilizados 'puros' como: "&amp ;" "&gt ;" "&lt ;" "&apos ;".

## Anatomia Documento:

<! DOCTYPE html >
Serve para que os navegadores, principalmente antigos, entendam que o documento a ser lido é um HTML.

< html >
Essa tag vai conter dois importantes elementos, o < head > e o < body >.

Head vai conter configurações importantes da página, mas que o usuário não verá ainda, como "meta", que vai informar vários tipos de metadados de nossa página, como a aceitação de caracteres especiais.

Já no body é onde estará o conteúdo que o usuário verá na página.
