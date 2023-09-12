# Display: flex e Display: grid.

## Esclarecimento sobre posicionamento:

Nessa aula veremos um pouco sobre posicionamento de elementos usando o CSS. Normalmente quem esta estudando HTML e CSS começa vendo posicionamento por meio do comando Position, left, bottom no CSS. Em nossa capacitação, optamos por começar pelo display: flex e grid, pois é o que normalmente utilizamos em nossos projetos e também porque é uma solução mais elegante. Porém, aprender o position também é importante e me salvou em várias tasks, então sinta-se a vontade para estudar esse comando por fora. Agora, vamos ao display: flex;

## Display flex:

Como dito acima, o display: flex é uma ferramenta interessante do CSS para manipular a posição de elementos HTML. DIferente do position, left, top e etc. o display: flex não pode manipular os elementos por pixels, distancias ou porcentagem. Ele é mais um organizador, que facilita nosso trabalho, pois nos polpa de ter que calcular, por exemplo, o número de pixels para centralizar um elemento. O display: flex é aplicado aos elementos child daqueles que selecionamos. Por exemplo, temos:
```
<div class = 'profilePicContainer'>
  <img src = 'www.enderecoDaImagem.com' class = 'profilePic'>
  <h2>Olá, Fulano!</h2>
  <a href = 'www.linkDaAplicacao.com'> Alterar foto de perfil </a>
</div>
```
No código a cima, temos as tags `img, h2` e `a` como child de uma `div` de classe "profilePicContainer". Para aplicamormos uma formatação nos elementos child dessa div, fazemos no CSS:
```
.profilePicContainer{
  display: flex;
}
```
### Exemplos de display: flex:
Seção sem display: flex:

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/8d0cff18-e8bd-4c44-9360-f46321e59379)

Seção com display flex:

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/9934e0a8-1e9e-4266-bb56-da8c2e4a3e82)

### Fragmentando para usar o display: flex:

Por vezes para usarmos o display: flex temos que fragmentar bem as nossas tags, colocando elas dentro de divs pais. Repare na imagem abaixo. Nela temos uma seção típica de contato com formulário e localização. Repare no sentido dos elementos, seguindo as setas. Inicialmente temos dois elementos alinhados horizontalmente, um do lado do outro. Internamente, temos elementos empilhados (um acima do outro). Assim, temos que ter elementos pais diferentes para traçar direções diferentes para os filhos. Na imagem abaixo os elementos pais são simbolizados pelas bordas azul e vermelhas.

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/c4d8dbcd-5203-4e88-875b-05bf47ddb6bf)

Fragmentando ainda mais: na imagem abaixo fragmentamos ainda mais a seção, adicionando outro elemento pai para os inputs de endereço e jogando display: flex nele.

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/b72dcf78-8715-4be3-99ef-c7109d211df2)

## Comandos relacionados:
Uma vez que temos um elemento pai com o estado flex, podemos adiconar mais comandos.

### Flex-direction: row x column:

O flex-direction orienta o CSS acerca do direcionamento dos itens filhos. Podemos fazer uma analogia as setas dos exemplos acima. Abaixo temos uma comparação de uma mesma seção com flex-direcion column vs. row.

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/bb1dccd5-b97d-466e-953f-04206271d3dc)
![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/d929ccbf-cbd2-4731-aed4-bf74e2bc948c)

### Align-itens:

O comando align-itens orienta acerca da orientação dos itens filho. align-itens: (left, center)

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/590e8ecb-ce4c-4ffb-8d5d-5c6c3e25c4b0)
![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/f624cfef-0612-41f2-b8d1-ebfa9e340453)

### Justify-content:

O comando justify-content tem uma função muito parecida com align-itens, porém no sentido inverso. **importante:** align-itens e justify-content se invertem dependendo do row ou column.

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/7b87bb40-3a53-4b23-aab5-e53e6a5a7a9e)

## Usando o devtools:

O devtools do seu navegador vai ser uma ferramenta interessante para quando estiver trabalhando com flexbox. No chrome você pode apertar `F12` no seu teclado para chamar o devtools, no Opera é: `Ctrl + Shift + C`. Quando você acessar o devtools, uma janela como da imagem abaixo vai abrir. Em sua jornada de desenvolvimento web, essa janela de devtools vai ser sua companheira constante! Podemos selecionar elementos do HTML para espioná-los um pouco melhor pelo devtools a partir da seta circulada em vermelho. Primeiro clicamos nela, depois no elemento que queremos examinar. Ou podemos clicar na janela logo abaixo, repare que ele discrimina elementos que estão selecionados com display: flex ou grid. Uma vez que você selecionou um elemento com flexbox o botão circulado em azul vai aparecer. Nele você pode colocar opções de flexbox e ver a mudança em tempo real, assim pode voltar para o CSS e colocar o mesmo comando.

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/ef264213-52a6-4723-8543-a2ed303f7a58)

Observe que os comandos estão indexados junto com seus códigos em CSS para que você possa fazer a alteração no arquivo caso goste das mudanças. É importante saber que a alteração no devtools NÃO será salva, é apenas uma mudança visual para observação.

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/91a56522-330a-42ee-970f-c5b323dfd0a7)


## Display grid:

Display: grid é outra ferramenta interessante para ordenação de elementos. Esse comando funciona, como o nome diz, como uma grade. Um exemplo pode ser visto abaixo:

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/36d8462b-f438-4841-97ac-47f946e8dde2)

Assim como o display: flex, o display: grid também é aplicado nos elemententos child. Na imagem acima temos o grid aplicado a uma div pai sobre elementos filhos button. Eles estão espaçados em colunas de quatro igualmente segundo o seguinte comando: `grid-template-columns: 25% 25% 25% 25%;`. Existem mais exemplos abaixo:

**grid-template-columns: 33% 33% 33%:**
![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/bd98e4b4-33b3-41b0-95d7-3d0b3a330dc8)


**grid-template-columns: 50% 50%:**
![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/374b0b3a-ad59-4622-9f44-55491c052bb8)

**grid-template-columns: 12rem 12rem 12rem:**

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/9d9e7b7a-572a-49d7-869b-b3a15a783f6d)

## Tarefa de Casa:

**1. Jogue esse joguinho para se familiarizar com os displays:**
https://flexboxfroggy.com

**2. Use display: flex e o código abaixo para reproduzir as imagens.**

```
    <section id="father">
        <div id="textDiv">
            <h2>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Fugiat, veniam?</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque sint dolor, amet, distinctio, eos incidunt recusandae ab quos repellendus nostrum necessitatibus reprehenderit vitae perferendis qui. Natus cumque, aut ullam cum quae fugit ad nulla aperiam odio accusantium, officia sed totam quis veritatis minus eius, debitis accusamus blanditiis. Qui, totam alias.</p>
        </div>
        <form action="">
            <input type="text" placeholder="nome">
            <input type="text" placeholder="endereço">
            <input type="email" placeholder="email">
            <textarea name="" id="" cols="50" rows="10"></textarea>
            <button>Enviar</button> 
        </form>
    </section>
```


imagem 1:

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/23e61ac6-1c1b-483b-8ec1-46d837af63a5)

imagem 2:
dica: utilize os comandos align-itens e justify-content.

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/37b842d7-64e1-4452-9f06-1a2d7b7eb2a0)

**3. Use o código abaixo e o display: grid para reproduzir as imagens abaixo:**

```
    <section id="father">
        <div class="card">
            <h2>Lorem ipsum dolor sit amet.</h2>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aspernatur, illum! Ut fugit quas repudiandae libero!</p>
        </div>
        <div class="card">
            <h2>Lorem ipsum dolor sit amet.</h2>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aspernatur, illum! Ut fugit quas repudiandae libero!</p>
        </div>
        <div class="card">
            <h2>Lorem ipsum dolor sit amet.</h2>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aspernatur, illum! Ut fugit quas repudiandae libero!</p>
        </div>
        <div class="card">
            <h2>Lorem ipsum dolor sit amet.</h2>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aspernatur, illum! Ut fugit quas repudiandae libero!</p>
        </div>
        <div class="card">
            <h2>Lorem ipsum dolor sit amet.</h2>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aspernatur, illum! Ut fugit quas repudiandae libero!</p>
        </div>
        <div class="card">
            <h2>Lorem ipsum dolor sit amet.</h2>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aspernatur, illum! Ut fugit quas repudiandae libero!</p>
        </div>
    </section>
```

inclua também no css:

```
body{
  background-color: black;
  padding: 0px;
  margin: 0px;
}
.card{
  background-color: white;
  border: none;
  border-radius: 12px;
  padding: 2rem 3rem;
  margin-bottom: 2rem;
}
.card h2{
  text-align: center;
}
button{
  padding: .8rem 1.4rem;
  border-radius: 12px;
  background-color: rgb(79, 248, 0);
  color: white;
  max-width: 10rem;
}
```

imagem1:

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/2fba3c62-a253-4922-a872-b949feac1d36)

imagem2:

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/19f6c5a7-7180-4156-b1cf-7002058a89ff)

