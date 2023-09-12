# Seletores Avançados do CSS:

Seletores são comandos CSS que ajudam a referenciar elementos HTML em uma página da web para aplicar estilos e formatação. Eles são usados para definir quais partes do código HTML devem ser afetadas pelas regras de estilo CSS, permitindo que os desenvolvedores controlem a aparência e o layout de uma página da web de forma eficaz. Basicamente já usamos seletores em nossos comandos CSS, por exemplo:
```
*{
  border: none;
  padding: 0px;
}
h2{
  color: white;
  font-size: 25px;
}

```
No código acima temos dois seletores o seletor h2 que se refere a tag secundária de título e a tag * que se refere a todos os elementos da página. Existem outros tipos de seletores que conhecemos como de id e classe, por exemplo: `#cardBox{background-color: purple;}` e `.card{color: white;}`. Porém, existem ainda mais seletores e iremos explorar os principais nessa lição!

## Seletores de descendencia direta e indireta:

Esses seletores funcionam para elementos child de outro, aplicando formatações somente neles. Sua sintaxe é `elementoPai > elementoFilho` e `elementoPai elementoFilho` respectivamente. Por exemplo: `div > p {color: red;}` no comando acima, atribuimos a cor vermelha a cada elemento de tag p que é child de uma div. Assim, essa instrução NÃO será atribuida a elementos p que não são child de div.

### diferença entre descendencia direta e indireta:

A diferença entre os comandos `div > p {color: red;}` e `div p {color: red;}`, seletores de descendencia direta e indireta, é bastante simples. O primeiro só é aplicado a filhos diretos de p, assim se tivermos:

```
<div>
  <form>
    <p>Olá eu sou neto da div!</p>
  </form>
</div>
```
O comando `div > p {color: red;}` não irá colorir p, porém o comando: `div p {color: red;}` irá! Pois p é um descendente indireto de div!

## Seletores de atributos:
Podemos selecionar elementos também por atributos! Lembra quando estávamos na lição de formulários e tínhamos, por exemplo: `<input type="text">` ou `<label for="email">Email</label>`? Esses campos tem os atributos "for" e "type", mas ainda existem outros como: "href", "src", "name", "method", "placeholder", "id" e "class". A sintaxe para selecionar por atributo é a seguinte: `seletor[type="atributo"]`, exemplos: `input[name="username"]`, `form[method="GET"]`, `a[href]`, `label[for="Password"]`.

## Seletores de pseudoclasses:



## Tarefa de casa:
1. Pesquisar sobre o seletos irmãos ou + e ~.
2. 
