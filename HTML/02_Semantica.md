# Segmentando o página usando a sintaxe:

Nessa lição iremos conhecer e experimentar um pouco mais as principais tags presentes no html para a segmentação da página web. Essa segmentação é muito importante para nossa página web por diversos motivos: ela deixa o código mais compreensivo e de melhor manutenção, habilita uma melhor sintaxe entre os devs, componentiza um pouco as coisas, ajuda em questões de acessibilidade e responsividade e também torna o site mais ou menos relevante para os principais motores de busca.

## Navbar:
Abreviação de "navigation bar" (barra de navegação), é um componente comum em páginas web e aplicações. Geralmente tem uma estrutura horizontal, focada na navegabilidade do usuário. No html, usa a tag `<nav></nav>`. Um exemplo de navbar:

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/a6b9e021-50a5-49ae-a310-d78f2f15bdd3)

## Main:
A tag `<main>` é um elemento HTML introduzido na especificação HTML5 para denotar o conteúdo principal de uma página da web. Ela é usada para agrupar o conteúdo central e principal de uma página, excluindo cabeçalhos, rodapés, barras laterais e outros elementos secundários.

O elemento `<main>` é uma parte importante do esforço para melhorar a acessibilidade e a estrutura semântica dos documentos HTML. Ao envolver o conteúdo principal em uma tag `<main>`, você está indicando claramente para os navegadores e tecnologias assistivas qual é a parte mais relevante do conteúdo.


## Section:
Em uma divisão da Main, que engloba um único tipo de conteudo. Uma analogia pode ser feita a um supermercado, onde existem seções de laticínos, onde só vende laticínios. No site, pode existir uma seção "sobre nós", "contatos" ou "nossos clientes". No html usamos a tag `<section>`. Segue um exemplo de section:

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/ab36240b-51d1-4c59-b83c-21fab1e42f4d)

## Divs:
Divs são divisões presentes dentro das seções dos sites. No Html usamos a tag `<div>`. Repare nas divs em verde na imagem abaixo:

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/fb436b24-ce96-48f5-8cb4-5a40f716b88e)

Repare que as divs são _chields_ do elemento pai, a section. Em geral divs estão dentro de outras tags, como seções ou mesmo dentro de outras divs. Divs podem ser usadas com css para organizar conteúdo (como colocá-los lado a lado ou em lista).

## Footer: 
É a seção inferior de um layout de site ou aplicativo que geralmente contém informações secundárias, links importantes e detalhes de contato. No html usa a tag `<footer>`. Um exemplo de footer:

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/975a51f1-5ff6-462c-87d9-674226e16556)

## Atividade:
Vamos retomar o código da lição anterior e utilizar a sintaxe correta para segmentá-lo, colocando os elementos da página como chields dos segmentadores seguindo a sintaxe do html. Começaremos com o cabeçalho, veja o exemplo abaixo. primeiro crie um elemento nav. Em seguida crie duas divs chields. Dentro da primeira div coloque as tags de link e dentro da segunda o título h1 e o subtítulo.

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/1a3457e1-4983-4b0c-91a9-d25e7005f9a1)

Em seguida crie uma main para o conteúdo principal da página. O esquema abaixo deve estar presente dentro da main, com o demarcado azul sendo uma section e os demarcados em verde sendo divs.

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/7964e890-e9e7-411f-a34f-b5bdc37047fb)

Por fim, crie o esquema abaixo. A parte contornada em azul deve estar dentro de uma tag footer e as partes demarcadas em verde devem estar dentro de duas divs.

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/217439af-9e7c-45d6-9c5c-226c6d2d1f45)

O código atual de nossa página é o próximo arquivo. Você pode comparar com o seu e usar tirar dúvidas com o seu guardião. Na próxima lição aprenderemos os primeiros passos de CSS.
