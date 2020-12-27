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

## Semântica:

Um dos principais objetivos do HTML é dar estruturação ao texto, fazendo as marcações para que o texto tenha mais significado. Para isso, são utilizados elementos semânticos para alcançarmos esses objetivos.

Há benefícios de escrever sites mais semânticos, como por exemplo, a influência em que seu site é indexado nas páginas de pesquisa. Poder utilizar leitores de tela, códigos em JavaScript e CSS para procurar elementos HTML, são outros benefícios de se ter um HTML bem estruturado semanticamente.

Uma dica é sempre se fazer perguntas, como, "será que preciso fazer uma lista? essa lista vai ter ordem? Preciso de um título? Preciso de um artigo? Esse artigo terá seções?".

## Listas:

Podem ser ordenadas e não ordenadas.

Para criar uma lista sem ordenação, crio os itens dentro da tag "li" e os envolvo com a tag "ul".

```
<h1>Suco Detox</h1>
<h2>Ingredientes:</h2>

<ul>
  <li>1 folha de couve;</li>
  <li>300ml de água de côco;</li>
  <li>1 maçã com casca;</li>
  <li>50ml de suco de limão</li>
</ul>
```

Esses elementos podem ser envolvidos em uma lista ordenada, utilizando-os dentro da tag "ol".

```
<h1>Suco Detox</h1>
<h2>Ingredientes:</h2>

<ol>
  <li>1 folha de couve;</li>
  <li>300ml de água de côco;</li>
  <li>1 maçã com casca;</li>
  <li>50ml de suco de limão</li>
</ol>
```

## Citações:

Recurso HMTL que temos para avisar que estamos pegando essa citação/esse texto de fora.

Utilizando < blockquote >, posso deixar bem grande o texto.

Utilizando o atributo < cite >, ajuda a falar de qual URL eu busquei essa citação.

```
<blockquote cite="https://google.com">
  O Elemento HTML <code>&lt;blockquote&lt;</code> indica que um texto texterno foi citado.
```

```
<p>
  De acordo com <a href="https://google.com"><cite>página MDN blockquote</cite></a>
</p>
```

O elemento quote, < q >, é utilizado para citações curtas que não precisam de parágrafos ou quebra de linhas.

## Abreviações:

Utilizando a tag < abbr >, podemos explicar abreviações de siglas, por exemplo, ao "descansar" o mouse sobre a palavra e, assim, ajudar o usuário da página a entender o que significa aquela abreviação.

```
<p>
  Usamos <abbr title="Hypertext Markup Language">HTML</abbr> para estruturar páginas Web.
</p>
```

## Detalhes de contato:

Com a tag < address >, conseguimos passar detalhes de contato da pessoa que escreveu o HTML, especificando o contato do autor que criou a página HTML.

```
<address>
  <p>
    Angélica Albuquerque<br>
    Rio de Janeiro, RJ
  </p>
</address>
```

## Lista de descrição:

O objetivo é marcar um conjunto de itens e suas descrições.

```
<h2>Glossário</h2>
<dl>
  <dt>Hypertext</dt>
  <dd>Hipertexto é o termo que remete a um texto ao qual se agregam outros conjuntos de informação na forma de blocos de textos, palavras, imagens ou sons, cujo acesso se dá através de referências específicas, no meio digital denominadas hiperligações.</dd>
</dl>
```

dl = description list
dt = description term
dd = fornece detalhes ou uma definição mais completa do termo precedente (definido por < dt >) numa lista de descrições (< dl >).

## Representação de código dentro do HTML:

Podemos utilizar a tag < code > para partes genéricas ou pequenas do código.
Já com a tag < pre >, podemos criar blocos de código, pois essa tag mantém os espaços em branco e recuos que eu colocar em meu código.

## Elementos genéricos:

< div >: serve para agruparmos conteúdo. Trabalha com ideia de bloco.
< span >: serve para agruparmos texto. Trabalha com ideia de linha.

## Âncora:

É o elemento que liga conteúdo com outro conteúdo, a tag < a >, responsável por fazer a ligação de diversas páginas.

#### Anatomia:

**Atributos:**

- globais (title, ids, class...)
- href (referência para onde iremos ao clicar no link)
  - url completa
  - fragmento
  - email
  - telefone
  - outros
- download
- target
  - self (padrão, abre na mesma janela)
  - \_blank (abre em nova janela)

### Absoluto x relativo:

Absoluto incluirá todo o protocolo e nome de domínimo e sempre apontará para o mesmo local, pois é absoluto.

Caminho relativo é relativo à página aberta no momento e apontará para lugares diferentes.
