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
### Personalizando o form:

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
+ **border-radius:** nosso formulário esta ficando legal, mas ainda esta um pouco quadradão, então vamos arredondá-lo usando o comando `border-radius: tamanhoDoArredondamento;`, escolha um valor em px, rem, em.


### Personalizando ainda mais:
Qual personalizamos nosso form ainda mais? Agora vamos para os campos. Edite primeiro as labels, usando os comandos: `color:` para mudar a cor da fonte, `font-size:` para mudar o tamanho da fonte (px, rem, em). Mude também os inputs, usando os comandos `width` e `background-color`, bem como o botão. No botão não esqueça de usar um `padding` para aumentar seu tamanho e border-radius para arredondá-lo!

## Personalização de chield:
Uma possibilidade que o CSS oferece é a personalização diferente para um elemento que é chield. Por exemplo, insira dois h3 em seu arquivo html, um dentro do body e outro dentro de uma div, seguindo o exemplo abaixo:
```
    <h3>Um h3</h3>
    <div>
        <h3>Outro h3</h3>
    </div>
```
Podemos personalizar os dois de maneira diferente, colocando no css:
```
h3{
    color: blue;
}
div h3{
    color: red;
}
```
Dessa maneira, um dos h3 vai ser azul e o outro vermelho. Repare na segunda sintaxe, ela diz: "color:red vai ser aplicado a tags h3 chield de uma tag div, ou simplesmente div h3".

## Ordem de leitura do CSS:
Vamos incluir mais tags iguais no HTML, coloque um h4, por exemplo: <h4>Olá, sou um h4!</h4>. Em seguida coloque no seu CSS dois comandos diferentes para o h4:
```
h4{
    color: blue;
}
h4{
    color: yellow;
}
```
Existe um conflito, pois no mesmo código estamos dizendo que tags h4 devem ser azuis e amarelas. Observe no navegador a cor do h4. Provavelmente seu h4 esta amarelo. Isso porque o CSS é lido e aplicado no html de cima para baixo, então comando escritos mais abaixo estão chegam na frente de comando mais em cima na hierarquia do CSS. Na próxima aula veremos opções mais sofisticadas de personalização e um pouco mais sobre hierarquia.

## Tarefa de casa:

Usando os códigos disponibilizados para o HTML, personalize conforme as imagens usando CSS.

**1.Navbar:** Tente usar os comandos text-align, padding, margin, font-weight e outros.
código:
```
    <nav>
        <a href="">Home</a>
        <a href="">Nossos Serviços</a>
        <a href="">Sobre</a>
        <a href="">Contato</a>
    </nav>
```
exemplo:
![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/136acbf1-4ede-441f-a76d-f06b38964bf2)

**2.Footer:**
código:
```
    <footer>
        <h2>Onde nos encontrar</h2>
        <p>Rua abc123</p>
        <h2>Fone</h2>
        <p>(99)1234-5678</p>
        <button>Fale conosco!</button>
    </footer>
```
exemplo:
![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/fc671c75-0d5e-4e39-b844-7fb0570cfb16)
