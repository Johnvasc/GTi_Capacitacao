# Head e Body:

## Tag HTML:
Vamos começar explorando a tag HTML. É uma das primeiras tags presentes no código é onde vai quase todas as outras tags. Repare na tag `<html lang="en">` e em seu fechamento `</html>` no final do código. Como foi dito, por questões de organização, as principais tags vão ser filhas dessa tag. Um elemento html é filha (_chield_) de outro quando ele é criao no escopo de seu elemento pai. Então quase todos os elementos são filhas da tag html. Esse conceito de _Chield_ vai ser abordado novamente em ocasiões futuras, como no Javascript. Repare que na abertura da tag html, existe o atributo _lang_. Esse atributo se refere a linguagem da página. Ele está inicialmente setado como "en" (english), mas pode ser mudado de acordo com o idioma preferido, por exemplo pt-br.

## Head:
A head é a tag que abriga a parte conceitual do site. Aqui também, em um futuro próximo, é onde vão ficar links de scripts e folhas de estilização. Vamos começar exploraando suas principais tags _chield_.
* `<meta charset="UTF-8">`: essa tag especifica o tipo de caracteres presentes na página. Dificilmante você vai precisar mexer nela, pois o UTF-8 conta com os principais caracteres incluindo os latinos.
*  `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: tag de responsividade (esse conceito vamos explorar mais a frente), é destinada a lidar com a exibição do site em diferentes aparalho e resoluções. Carrega três atributos relativos a nome, tamanho das dimensões e escala.
* `<title>Document</title>`: como dito na aula de introdução, é a tag título do site que é exibido nas guias do navegador. Em geral, tags de texto recebem seu argumento entre a abertura e o fechamento, como também é o caso dessa tag. Alguns exemplos dela: `<title>youtube</title>`, `<title>GTi Engenharia Jr - Soluções Web</title>`.

## Body:
O body é a tag que abriga a parte visual e interativa do site, o famoso UI (User Interface). Ele deve estar vazio agora em seu projeto, então iremos introduzir algumas tags. Primeiro, abra o _Live Server_, ele deve estar no canto inferior direito da IDE, conforme a imagem abaixo:

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/7dc550c0-0e0a-4206-9222-b256fe64de1a)

O _Live Server_ vai abrir a sua página, que nesse momento esta vazia, no navegador. Vamos testar algumas tags no código:
* `<h1>Olá mundo!</h1>`: Essa é tag `<h1>` ou simplesmente tag título. Semanticamente, é onde vir títulos importantes de sessões ou até mesmo o título do site. Salve essa alteração no código (para salvar alterações rápidas no código use sempre `ctrl + s`) e visite a página da web no navegador. Existem outras tags de título de hierarquia inferior, começando sempre com h.
* `<h2>Olá, sou um subtitulo de hierarquia inferior ao h1</h2>`: esse é um outro título de hierarquia inferior. Escreva no seu código e observe as diferenças entre o peso dos títulos no navegador.
* `<h6>Sou o h6 e existem vários na minha frente segundo a hierarquia</h6>`: coloque h6 no seu código e observe ele no navegador. Utilizar os títulos segundo a hierarquia correta é muito importante! Os motores de busca da internet (chrome, bing, etc), utilizam essas tags na hora de incluir sites relevantes ao usuaário de acordo com as palavras-chave digitadas escolhidas por ele.
* `<p>Eu sou um paragrafo!</p>`: Essa é a tag de texto principal. É onde devem vir todos os textos sem hierarquia da página.
* `<p>apresentando: <b>Sou a tag do negrito</b></p>`: Essa tag vem dentro da tag de paragrafo para dar ênfase a alguma parte do texto. Outra tag que faz a exata mesma coisa é a tag `<strong>`. Teste ambas no seu código.
* `<p>apresentando: <i>Sou a tag do itálico</i></p>`: Essa tag vem dentro da tag de paragrafo para dar ênfase a alguma parte do texto ou destacar palavras estranjeiras.
* `<p>apresentando: <s>Soua a tag do taxado</i></p>`: Essa tag vem dentro da tag de paragrafo para cortar/taxar o texto.
* `<a href="google.com">sou um link</a>`: Essa tag é a tag de link, que pode redirecionar o usuário para outro site ou sessão. O atributo `href` referencia ao endereço a ser direcionado, então teste mudar para algum outro site. A tag link pode vir dentro ou não da tag p.
* `ol ou ul`: são listas ordenadas (ordereds) e não-ordenadas (unordereds) com itens `<li>eu sou um item</li>`. A sintaxe segue o exemplo:
```
<ul>
  <li>item 1</li>
  <li>item 2</li>
  ...
  <li>item n</li>
</ul>
```


![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/c1c13a60-e6e8-469c-8f20-ffef219c4ec3)


## Lição de casa:

Use as tags textuais que você aprendeu nessa lição para replicar a página abaixo:

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/dd767ae1-bff5-46f7-b39c-f7059b8f2394)

