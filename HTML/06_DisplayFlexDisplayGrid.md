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


