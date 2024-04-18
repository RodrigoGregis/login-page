# login-page

Este projeto foi desenvolvido com o objetivo de praticar e aprimorar os conhecimento em HTML e CSS. 

![](https://raw.githubusercontent.com/RodrigoGregis/login-page/main/image/preview.png)
___
## HTML

- Container: classe utilizada para representar o Conteúdo (geralmente possui uma largura máxima definida)

- No button, foi utilizado um id para que fosse possível pegar o elemento no JavaScript.

- Para estilização dos elementos, sempre utilizar class.

- h1:  https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/Heading_Elements

- div: https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/div

- span: https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/span

- form: https://developer.mozilla.org/pt-BR/docs/Learn/Forms/How_to_structure_a_web_form

- input: https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/input

- label: https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/label

- button: https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/button

- footer: https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/footer 

___
___
___

## CSS

- Flexbox: https://css-tricks.com/snippets/css/a-guide-to-flexbox/

- O @import é utilizado para importar fontes dentro de um arquivo CSS e deve estar sempre no **início** do documento.

- O @media é utilizado para alterar estilos em determinadas resoluções e deve sempre estar no **final** do documento.


### Ref #01
O **box-sizing** é responsável por definir como a largura e a altura de um elemento serão tratadas. 

Por padrão, o **box-sizing** é definido como **content-box**.

> **box-sizing: content-box;**

Ao utilizar o **box-sizing: content-box**, a largura e altura definida é aplicada somente à caixa de conteúdo do elemento.

No caso de utilizar, por exemplo, um padding, o valor será somado à largura e altura da caixa de conteúdo do elemento.

Por exemplo:

> &lt;div style="width: 250px; height: 250px; padding: 25px;"&gt;Olá, mundo!&lt;/div&gt;

Ela terá uma largura e altura total de 275px, que consite nos 250px de largura e altura + 25px de padding.


Já na utilização do **box-sizing: border-box**, os valores adicionais são subtráidos da largura e altura definidas no elemento.

Por exemplo:

> &lt;div style="width: 250px; height: 250px; padding: 25px;"&gt;Olá, mundo!&lt;/div&gt;


O elemento terá uma largura e altura total de 250px (valores definidos) e a largura e altura da caixa de conteúdo será de 225px.


___
### Ref #02

Quando utilizamos **display: flex** em um elemento, os elementos filhos passam a poder ser manipulados (alinhameno, posição, etc) com propriedades flex. 

Como, por exemplo:

> align-items: center;

> justify-content: space-between;

As vezes, os elementos filhos ficam em colunas (um abaixo do outro) ou em linha (um ao lado do outro).

Para alterar este comportamente podemos usar **flex-direction** com os valores **column** ou **row**.

Exemplos:

> flex-direction: column;

ou

> flex-direction: row;

---
### Atualizações

Foi alterada a forma de como é feita a prevenção de envio do formulário. 

Anteriormente foi utilizado o JavaScript. Agora é utilizado o **type="button"** no botão que está dentro do furmulário.

#### Motivo

Cada botão dentro de um **form** (formulário) possui, implicitamente, o **type="submit"**. Isso faz com que, ao clicar no botão, seja disparado as ações padrão do formulário.

Para evitar que seja disparado essas ações do furmulário podemos adicionar o **type="button"** no botão (**button**) que está dentro do furmulário.