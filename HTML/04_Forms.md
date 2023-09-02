# Experimentando as tags de formulário:

Páginas na WEB em geral trabalham com o envio de formulários, seja um formulário de login ou inscrição, um formulário de atendimento, opinião, compra, exclusão, edição, etc. O HTML possibilita de forma nativa fazer esse envio usando a tag `<form>`. Existem outras tags auxiliares que nos ajudarão na hora de criar formulários funcionais. Nessa aula iremos explorar essas tags.

## Criando um novo arquivo para o formulário:

Vamos criar um novo arquivo html no nosso diretório, você pode chamá-lo de `formulario.html`. Lembre-se que para iniciar um código HTML no VSCode você pode começar escrevendo html e clicar no atalho `html:5`. Pode ser necessário você ter que reiniciar o _Liveserver_ conforme a imagem abaixo ou digitar no navegador: `http://127.0.0.1:5500/formulario.html`.

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/3ddcd078-19ba-4223-b6f3-1f3797a9bc7f)

## Criando um novo formulário:

Dentro da tag `<body>` iremos incluir a tag `<form>`. Essa é a tag de formulário e pode receber alguns argumentos que iremos explorar mais tarde. Inicialmente iremos colocar os argumentos:
+ method = "post"
+ action = "/envio"
Assim, nossa tag form vai ficar com essa cara: `<form method="get" action="/envio"></form>`;

## Inserindo campos de formulário:

Em geral, formulários tem campos para o usuário responder. Vamos experimentar alguns deles. Dentro da tag `<form>` insira:
+ **label:** Labels são textos de descrição. Eles descrevem o tipo de informação que o usuário deve colocar no input abaixo. Então coloque a seguinte label: `<label for="username">Seu nome</label>`
+ **input:** Inputs são os campos que receberão as respostas do usuário. Existem vários tipos de input: texto, número, senha, data, etc. O tipo do campo vai ser definido no argumento _type_, por exemplo: "text", "password", "number", entre outros. Então coloque: `<input name="username" type="text">`. Perceba o atributo _name_. Ele faz a união da tag com o input, relacionando-se com o _for_.
+ **label 2:** Iremos inserir mais labels, uma para cada campo, então coloque: `<label for="password">sua senha</label>`
+ **button:** Essa tag cria um botão para envio de formulário ou chamado de funções javascript. Ele deve ficar assim: `<button>Entrar</button>`. O texto "Entrar", localizado na tag é o texto exibido no botão.
+ **br:** Br é a tag de quebrar linha (deve vir do inglês, break). Coloque uma tag br depois de cada tag acima para o formulário ficar mais legível.

## Conhecendo um pouco mais dos argumentos do form:

Agora você pode visitar sua página na web e tentar fazer o login com uma senha e usuário qualquer. Inicialmente a página vai reportar um erro, pois estamos enviando informações para lugar nenhum. Coloque em "voltar" no seu navegador para voltarmos a página de formulário. Os campos da tag form são os seguintes:
+ **method:** esse é o método que vai no cabeçalho do pacote HTTP. Diversos tipos de métodos são usados em redes de computadores como: "GET", "POST", "PUT" e "DELETE". Mudar esse argumento vai mudar o campo do cabeçalho HTTP.
+ **action:** nesse caso, action recebe uma url para mandar esse pacote. Então se quisermos, por exemplo, mandar um pacote para facebook/login, podemos fazer: `<form action="facebook/login>"`. No caso da nossa aplicação, um erro ocorre pois não existe "/envio". Experimente colocar "/formulario.html" (ou o nome que escolheu para o arquivo) e enviar um formulário.

## Transmissão de conteúdo:

Perceba sua URL na parte de cima do navegador. Ela deve estar como na imagem abaixo (se não estiver tente clicar nela):

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/91272e0a-b406-4e65-aba3-036bf76ca02c)

Repare que existem dois campos na URL o **username** e o **password**, eles aparecem logo após o **?**. Esse é o modelo de envio de dados pela URL, ela segue o seguinte padrão: `www.urldosite?campo1=valor1&campo2=valor2&...campoN=valorN`. Existem outras maneiras de enviar dados pela web, essa é só uma delas. Você pode perceber que nossa senha esta sendo enviada sem qualquer tipo de segurança e nossa conta poderia ser facilmente hackeada, mas esse tipo de envio funciona para dados menos sensíveis.

## Placeholder:

Uma opção ao uso da tag <label> é a insersão do argumento placeholder dentro do input. Ele segue a seguinte sintaxe: `<input name="username" type="text" placeholder="Seu nome">` Esse argumento vai fazer que o texto que voc


## Tarefa de casa:
No formulario.html recrie os seguintes formulários (obs, use as sugestões do VSCode enquanto estiver digitando input para conseguir dicas do type do input):

**1. formulário com campo numérico:**

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/66cb5a22-a6b9-4223-9743-2985ed226bc4)

**2. formulário com checkbox:**

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/605a3002-f700-43ef-91fb-3c59d97f8420)

**3. formulário com range e data:**

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/7314b54f-0034-496e-8a69-a92be439d6de)

**4. formulário com placeholder:**

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/36f684a0-6898-427b-a1e5-f09390cbe35d)

**5. formulário com color, radio (três deles) e range:**

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/219ecfaf-be08-44e5-a8b9-5f7c592d8ead)

**6. formulário de envio de arquivos:**

![image](https://github.com/Johnvasc/GTi_Capacitacao/assets/39773960/415dea2e-190d-4060-addb-9afe081c1685)

