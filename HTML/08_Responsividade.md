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

Para aplicar CSS customisado com base no tamanho da tela,
