# Estilização com o CSS:

CSS, ou Cascading Style Sheets (Folhas de Estilo em Cascata), é uma linguagem de marcação utilizada no desenvolvimento de páginas web para definir a apresentação e o layout dos elementos HTML. Com o CSS, é possível controlar a aparência dos elementos, como cores, fontes, espaçamento e posicionamento, permitindo a separação entre o conteúdo estrutural (HTML) e sua formatação visual. Isso possibilita a criação de designs consistentes e agradáveis, além de facilitar a manutenção e a adaptação de páginas web para diferentes dispositivos e tamanhos de tela.

## Iniciando outro arquivo HTML:

Como estamos acostumando, vamos criar outro arquivo html. Vamos chamá-lo de personalizacoes.html ou outro título de sua preferência. Comece iniciando o html clicando no atalho html:5, depois reinicie o _liveserver_ ou acesse o url `http://127.0.0.1:5500/personalizacoes.html`.
Vamos também colocar algumas tags no corpo html. Dentro do body coloque:

```
    <h1>Meu titulo personalizado</h1>
    <h2>meu subtítulo colorido</h2>
    <p>paragrafo1</p>
    <button>Botão</button>
```
 
## Iniciando o CSS:

Na IDE crie um novo arquivo com extensão .css, por exemplo `style.css`. Agora vamos no arquivo html para vincular a folha de estilo ao nosso site. No head comece digitando link e escolha a opção link:css conforme a imagem abaixo. A seguinte tag vai ser inserida `<link rel="stylesheet" href="style.css">`. Mude o texto em href para o nome do seu arquivo.

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/6f75cafb-98f7-4275-a5d5-465ef069bd40)

## Primeiros comandos:

O CSS é bastante simples. Sua sintaxe é a seguinte:

```
nomeDaTag{
  comando1: valor;
  comando2: valor1, valor2;
  comando3: valor;
}
```
Assim, definimos uma tag e colocamos os comandos de personalização dentro das chaves e essas mudanças vão ser aplicados a todos os elementos da página com a tag que definimos. Diferente do HTML, essa linguagem de marcação precisa ; para separar seus comandos. Vamos a um exemplo bastante simples. Escreva no seu arquivo CSS e em seguida teste no navegador:

```
body{
    background-color: #afe2ff;
}
```
A cor do background deve ter mudado. Agora faça:
```
h1{
    color: yellow;
}
p{
    color: #fff;
}
button{
    color: rgb(255, 255, 0);
}
```

## Um pouco mais de cor:

No código acima, definimos cores para os elementos h1, p e button presentes no html. Repare que em um dos casos escrevemos o nome da cor e no outro definimos em hexadecimal e rbg. Em geral, a segunda e terceira opção é são as preferidas, pois possibilitam cores mais personalizadas. Também pudemos usar o rgba para lidar com a transparencia da cor!
```
nav{
    background-color:  #090058;
    color: white;
}
```

## Criando um formulário bonito:

Na aula passada criamos diversos formulários, mas eles pareciam bem "crus". Que tal adicionarmos um pouco mais de estilo aos nossos formulários? Apague todas as tags dentro do body de personalização e coloque no lugar:

```
    <form>
        <label for="id">usuário:</label>
        <input type="text" name="id" id="">
        <br>
        <label for="password">senha:</label>
        <input type="password" name="" id="">
        <br>
        <button>Login</button>
    </form>
```
### Personalizando a div:

Primeiro vamos mexer no corpo do formulário. Escolha uma cor que ache interessante e coloque no css para a tag form, seguindo a sintaxe:

```
form{
  comando: valor;
}
```
Agora vamos adicionar mais comandos no forms:
+ **width:** é o tamanho horizontal do form. Geralmente elementos tentam ter o tamanho horizontal maior possível, mas queremos uma caixa de formulário um pouco melhor. Então coloque o comando `width: valor`, o valor pode variar em diversos tipos, por exemplo 30%, 250px, 5rem, 5em, etc. Escolha um valor que lhe agrade.
+ **padding:** uma vez com o tamanho e a cor selecionada, podemos perceber que nossos campos de formulário estão muito colados no elemento pai. Assim, devemos usar o padding. Padding é uma instrução sobre a distancia dos elementos filhos da borda. Experimente colocar um padding: 40px;
+ **mais sobre o padding:** repare com elemento pai tem quatro bordas: cima, esquerda, baixo e direita. Podemos escolher a distancia de maneira personalizada, para cada um desses lados com a sintaxe: `padding: 20px 30px 20px 30px;`. Outra maneira de selecionar padding é a seguinte: `padding: alturaDeCima alturaDosLados`, no caso da altura de cima e de baixo serem as mesmas, bem como as laterais, por exemplo: `padding: 2em .5em;` (no CSS, .5 é a mesma coisa que 0.5).
+ **border:** vamos colocar uma borda em nosso formulário. Você pode usar o comando: `border: tipo tamanho cor`, por exemplo: `border: solid 1px gold;`
