# Curso de Git do básico ao avançado
Nesse curso visto no link [Udemy] `(https://ibm-learning.udemy.com/course/git-e-github-do-basico-ao-avancado-c-gist-e-github-pages)`

## Recomendações
- Instalar o git no seu SO (sistema operacional):
    - Acessando o link [Git]`(https://git-scm.com/downloads)`
    - Instalar o VS Code [Visual Studio Code]`(https://code.visualstudio.com/download)`

## Criando o repositório ou repo

No seu GitHub você pode seguir as informações que ele já lhe dá ou você pode fazer pelo terminal.
Quando você cria pelo GitHub, ele lhe dá após algumas informações que são essas:
```
echo "mensagem" >> README.md
git init
git add README.md
git commit -m 'first commit'
git branch -M master
git remote add origin [seu repositório]
git push -u origin master
```

## Primeiros passos
Para dar se o início ao uso do Git, precisamos abrir um repositório (repo) em um servidor ou serviço de SCM (versionamento), podemos usar o GitHub que é uma comunidade de diversos desenvolvedores.
Você precisará abrir um repo em sua conta e depois pelo seu computador fazer a inicialização do mesmo.
O comando para inicializar um repositório é o ```git init``` que irá criar uma pasta ```.git``` na pasta que destinar o comando por via de terminal ou prompt de comando.
Se você utilizar o ```VSCode``` basta no terminal que já vem imbutido nele fazer esse comando ou pelo seu ```Git Bash``` que foi instalado quando você fez a instalação do [Git].
Após ter clonado ou ter feito o envio do seu repo localmente, você poderá fazer seus primeiros commits.

## Fazendo commits
Para realizar um commit você precisa ter um objeto ou item criado, para realizar essa função você pode fazer a quebra da maldição do mundo do TI, criando um arquivo qualquer com a frase ```Hello World```, para fazer a criação do objeto você pode fazer pelo seu terminal usando o comando ```echo "Hello World" >> helloWorld.txt```.
O que esse comando faz?
- echo: é um comando para escrever algo em um arquivo, por isso ele é seguido de aspa duplas ( " ), que simboloza que você está escrevenvo um texto;
- ">>": esse comando faz com que você escreva a frase ou texto anterior dentro de um objeto;
- nome do objeto: no final do comando você informa o nome do objeto e a sua extensão, no exemplo de cima foi feito a criação de um objeto chamado helloWorld com a extensão .txt;

Após a criação do objeto você precisa "trackear" o mesmo, ou seja, informar ao Git que esse objeto será enviado, essa função se dá ao comando ```git add [nome do objeto]``` ou seja, você precisa dar o comando git add seguido do nome do objeto, para seguirmos com o exemplo, você irá dar o comando ```git add helloWorld.txt``` fazendo ele ficar trackeado e dentro do stage. 
- ```Meu Deus muita palavra difícil e diferente... Fique calmo que você se acostuma e não tem tanta necessidade do desespero```

A palavra stage é o momento que você fala para o Git que esse objeto está na fila para o envio, fácil não é?

Muito bem agora, você precisará fazer o commit, ou seja, o devido envio com uma mensagem que explica ou de fácil entendimento com o que você está fazendo.
Para isso você precisa usar o comando ```git commit -m ''``` o que cada coisa faz?
- git commit: é o comando que você chama para fazer o commit do objeto;
- -m: é o comando que você irá informar uma mensagem, que deve ser seguido das aspas simples;
- '': é onde será colocado o texto explicativo ou comentário do que se trata o objeto ou a alteração;

Então vamos digitar ```git commit -m 'Quebrando a maldição Hello World'``` e damos o enter;
Agora precisamos finalizar e enviar o objeto para o servidor remoto do git.

## Enviando objetos

Para finalizar e realizar o envio do objeto fazemos o comando ```git push``` que se dá a necessidade a cada git commit dado para oficializar o envio.
Se for o seu primeiro envio para o repositório remoto, você será alertado pelo git que precisa dar um comando mais completo.
Comando esse que é: ```git push --set-upstream orgin master```;