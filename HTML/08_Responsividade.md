# Responsividade:

Responsividade em web é a capacidade da página ou aplicação se adaptar a diferentes leyouts de tela ou tamanhos. Imagine que um site projetado para computador pode não ficar tão legal na interface de um smartphone, ou um site feito para um monitor normal pode precisar de algumas adaptações para um monitor 4k. Vamos aprender alguns comandos para aplicar um pouco de responsividade na nossa página.

Crie uma nova página HTML e link com um CSS e insira os seguintes comandos:
```
<img src="https://fastly.picsum.photos/id/841/800/300.jpg?hmac=vBGUd7wIprHEZu2CeYYwJz3AxBq2p8EmSp7Gi6BQ4Oc" alt="">
<h1>Olá, sou um titulo!</h1>
```

No CSS insira: 
```
img{
  width: 900px;
}
h1{
  font-size: 150px;
}
```
Agora temos uma imagem com um tamanho fixo de pixels. Uma boa prática pode ser escolher o tamanho da imagems com medidas relativas como rem e em, por exemplo width: 20rem; 

## Testando a reponsividade com devtools:

Você pode testar a responsividade usando o devtools. Primeiro abra o devtools (`F12` no chrome e `ctrl + shift + c` no opera). Existem duas maneiras, você pode simular telas menores arrastando a lateral do devtools e fazendo ele ocupar um espaço maior na tela ou pode acessar o ícone circulado em azul da imagem abaixo. Também pode optar por aparelhos de diferentes tamanhos de tela clicando na cascata sublinhada em amarelo:

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/7f5dc3f3-0193-4a1b-a440-52f7fc227898)

## Aplicando efeitos diferentes no CSS para diferentes tamanhos de tela:

Para aplicar CSS customisado com base no tamanho da tela, podemos usar a sintaxe `@media screen and (condições){comandosCSS}`. Vamos ver alguns exemplos:

**ex1: Body vermelho para aparelhos com largura de tela maior que 1024px:**
```
@media screen and (min-width: 1024px){
  body{
      background-color: red;
  }
}
```

**ex2: mudando o tamanho de imagens para aparelhos com a largura entre 720px e 1024px:**
```
@media screen and (min-width: 720px) and (max-width: 1023px){
  img{
    width: 50vw;
  }
}
```

**ex3: empregando vários comandos para aparelhos cuja altura da tela seja menor que 600px:**
```
@media screen and (max-height: 600px){
  img{
    height: 10vh;
  }
  p{
    color: dark-gray;
    font-size: 12px;
  }
  body{
    background-color: yellow;
  }
}
```
teste os códigos CSS acima usando o devtools para diminuir o tamanho da tela.

## Unidades de tamanho responsivas:

Nos exemplos acima, pudemos ver duas novas unidades de tamanho, são elas: vh e vw. A viewport height é uma unidade de medida relativa em porcentagem ao tamanho da altura da janela do navegador, então se quisermos que uma imagem tenha uma altura oculpe 10% do tamanho da janela do usuário, podemos fazer `img{height: 10vh;}`. Vh, claro, pode ser usado em outros contextos como: `p{font-size: 2vh}` ou `div{widht: 15vh}`. O Vw (viewport width) é muito semelhante ao height, porém e relativa ao cumprimento em porcentagem da janela. Assim, se quisermos que a largura das divs sejam 30% da largura da janela exibida no navegador, podemos fazer `div{widht: 30vw;}`. Repare que essas medidas, tanto vw quanto vh, dependem do tamanho da tela e irão se ajustar. Contudo, essas medidas podem não ser indicadas em alguns casos, sendo mais interessantes para fazer itens de tamanhos harmoniosos (por exemplo se formos posicionar 4 divs lado a lado, pode ser interessante que cada tenha 25% ou 20% do tamanho da largura da tela).


