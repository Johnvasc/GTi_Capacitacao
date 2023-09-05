# Classes e IDs:

Viemos aula passada opções de personalização no CSS, porém nossos comandos de personalização eram amplos demais, se aplicando a todos os elementos de uma tag. As vezes queremos criar estilos diferentes para uma mesma tag e usar a técnica do chield não é nem um pouco eficiente. As vezes também queremos criar um estilo padrão que se repita em só alguns elementos, por exemplo um botão vermelho e redondo que simbolize negativo ou um botão verde e quadrado de inscrição. Nesse contexto, as classes e IDs irão nos ajudar!

## IDs no CSS:
O ID no CSS, ou Identificador, é uma ferramenta poderosa para aplicar estilos específicos a elementos HTML em uma página da web. Ele é definido usando o caractere "#" seguido por um nome exclusivo que você atribui a um elemento HTML. Quando um ID é aplicado a um elemento, como uma div ou um botão, você pode usar regras CSS para direcionar esse elemento de maneira única. Também podemos adicionar vários IDs a uma tag, separando-os por espaços: `<div class = 'id1 id2 id3'></div>`, assim criamos uma div com três IDs: id1, id2, id3.
**dica:** no VSCode você pode criar uma tag rapidamente com um id fazendo: nomeDaTag#NomeDoID, por exemplo: h2#formTitle.

### Aplicando um ID no HTML:
Vamos criar uma tag com um id. Por exemplo, temos um formulário que é único no minha página, podemos colocar o id na tag form da seguinte maneira `<form id = "nomeDoID"></form>`. Repare que o ID é apenas outro atributo da tag, como já havíamos visto exemplos antes. Novamente: IDs são únicos em uma página, ou seja se uma tag tem o id _"userIcon"_, nenhum outro ID deve ter o mesmo nome. Ele funciona para elementos que tem uma personalização única.

### Aplicando comandos a um ID no CSS:
No CSS a sintaxe é a seguinte:
```
#nomeDoId{
  comando1: valor1;
  comando2: valor2;
  ...
  comandoN: valorN;
}
```
Dessa maneira, os comandos dentro das chaves vão ser aplicados somente a tag que tiver o ID _nomeDoId_. Repare no # antes do nome do Id. Ele é o identificador do ID. Comandos CSS para IDs sempre devem ser precedidos de uma #.

## Classes no CSS:
As classes no CSS são uma maneira versátil de aplicar estilos a elementos HTML que compartilham características semelhantes, mas não necessariamente exclusivas. Elas são definidas usando o atributo "class" em elementos HTML e são identificadas por um nome que pode ser reutilizado em vários elementos na mesma página ou até mesmo em diferentes páginas do site. Um exemplo pode ser um botão que se repete em várias partes da página, ou um _card_ que é replicado em várias seções.

### Aplicando classes no HTML:
Vamos criar uma tag com uma tag. Por exemplo, uma div vai receber vai aparecer em várias partes da página como um card, podemos colocar uma classe na tag div da seguinte maneira: `<div class = 'aboutCard'><div>`. Classes, diferente de IDs, não são únicas. Então podemos ter várias tags com a mesma classes, assim podemos ter um padrão de personalização para um certo elemento. Também podemos adicionar várias classes a uma tag, separando-as por espaços: `<div class = 'classe1 classe2 classe3'></div>`, assim criamos uma div com três classes: classe1, classe2, classe3.
**dica:** no VSCode você pode criar uma tag rapidamente com uma classe fazendo: nomeDaTag.NomeDaClasse, por exemplo: div.aboutCard.
**dica2:** ainda no VSCode podemos criar várias de uma tag usando nomeDaTag*NºdeRepetições, por exemplo: `div*5`. Assim, criamos 5 divs de uma vez.
**dica3:** podemos também criar elementos dentro de outros fazendo: tagExterna>TagInterna, por exemplo: div>h3.

### Aplicando comandos a classes no CSS:
No CSS a sintaxe é a seguinte:
```
.nomeDaClasse{
  comando1: valor1;
  comando2: valor2;
  ...
  comandoN: valorN;
}
```
Dessa maneira, os comandos dentro das chaves vão ser aplicados somente as tags que tiverem a classe _nomeDaClasse_. Repare no . antes do nome da classe. Ele é o identificador da classe. Comandos CSS para classes sempre devem ser precedidos de um "." .
 
## Tarefa de casa:

1. Replique o estilo light e dark para as navbars do código baixo.

Dica1: atribua IDs diferentes para ambas as navs e personalize usando esses IDs no CSS.

Dica2: utilize a sintaxe: `#nomeID nomeTag{comando: valor}` do CSS para utilizar menos comandos.
código:
```
  <nav id="">
    <a href="">Home</a>
    <a href="">Sobre</a>
    <a href="">Nossos serviços</a>
    <a href="">Contatos</a>
  </nav>
  <nav id="">
    <a href="">Home</a>
    <a href="">Sobre</a>
    <a href="">Nossos serviços</a>
    <a href="">Contatos</a>
  </nav>
</body>
```
referência:

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/55d98a41-3d8c-46bb-a9d7-94d70eb0744d)


2. Crie três cards seguindo o código e personalize eles utilizando CSS. Cada card deve ter um tema claro e um tema escuro!
Dica: use a sintaxe: `<div class = "classe1 classe2></div>"`. A classe1 pode ser uma personalização geral para os cards, enquanto a dois pode ser o tema claro ou escuro, dependendo do card!
código:
```
  <div class="">
    <h2>Troca de antimatéria</h2>
    <p>Na KE você faz a troca de antimatéria sem problemas adicionais. Existe garantia e cobertura total.</p>
  </div>
  <div class="">
    <h2>Lataria de cometa</h2>
    <p>Pensando em ter a lataria mais resistente da via lactia? Aqui deixamos você mais blindado que um cometa!</p>
  </div>
  <div class="">
    <h2>Troca de núcleo espacial</h2>
    <p>Núcleos verídicos, encontrados no centro de estrelas de neutrons, para uma autonomia de 5000000 de anos luz!</p>
  </div>
```
referência:

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/61c60070-1b9d-4852-bdc2-ed1376720217)
