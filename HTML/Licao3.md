# Estilização com o CSS:

CSS, ou Cascading Style Sheets (Folhas de Estilo em Cascata), é uma linguagem de marcação utilizada no desenvolvimento de páginas web para definir a apresentação e o layout dos elementos HTML. Com o CSS, é possível controlar a aparência dos elementos, como cores, fontes, espaçamento e posicionamento, permitindo a separação entre o conteúdo estrutural (HTML) e sua formatação visual. Isso possibilita a criação de designs consistentes e agradáveis, além de facilitar a manutenção e a adaptação de páginas web para diferentes dispositivos e tamanhos de tela.

## Iniciando o CSS:

Na IDE crie um novo arquivo com extensão .css, por exemplo `style.css`. Agora vamos no arquivo html para vincular a folha de estilo ao nosso site. No head comece digitando link e escolha a opção link:css conforme a imagem abaixo. A seguinte tag vai ser inserida `<link rel="stylesheet" href="style.css">`. Mude o texto em href para o nome do seu arquivo.

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/2d4b9e5f-d494-4483-b8fb-dba52489917c)

## Primeiros comandos:

O CSS é bastante simples. Sua sintaxe é a seguinte:

```
nomeDaTag{
  comando1: valor;
  comando2: valor1, valor2;
  comando3: valor;
}
```
Diferente do HTML, essa linguagem de marcação precisa ; para separar seus comandos. Vamos a um exemplo bastante simples. Escreva no seu arquivo CSS e em seguida teste no navegador:

```
body{
    background-color: #afe2ff;
}
```
A cor do background deve ter mudado. Agora faça:
```
p{
    color: #fff;
}
```
A comparação entre as tags e o modelo pode ser vista abaixo. Elas seguem a sintaxe:

* Nome da tag: body ou a tag p (paragrafo)
* {comandos;}: o comando background-color: seleciona uma cor para o plano de fundo (essa cor foi setada em hexadecimal). O comando color seleciona uma cor para fonte (também setada em hexadecimal).

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/151d0d60-4b34-4962-91ab-dcd506dc2c2c)

## Um pouco mais de cor:

Vamos colocar cores em mais tags, por exemplo na nav e sections:

```
nav{
    background-color:  #090058;
    color: white;
}
```
