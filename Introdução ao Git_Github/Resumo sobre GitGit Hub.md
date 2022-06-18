## Resumo sobre Git/Git Hub :facepunch: ##



## O que é Git? ##

Git é um software de versionamento de código que vai nos ajudar a criar e monitorar diferentes versões do nosso código dentro de nossa máquina; Git é apenas uma criação do Linux que nasceu com o descontentamento de um sistema de versionamento de código que já existia; 

Git e  Github são duas tecnologias completamente diferentes, porém complementares; Github é o repositório online onde vamos armazenando nosso código:

#### Benefícios de ambas tecnologias: ###

- Controle de versão
- Armazenamento em nuvem
- Trabalho em equipe
- Melhorar seu código
- Reconhecimento

### Navegação via command line interface e instalação  ###

A forma de interagir com o Git da forma que a tecnologia foi concebida é por linha de comando

![image-20220617204953521](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617204953521.png)



### Realizando a instalação do git 

Git-scm.com https://git-scm.com/ 

Executa o instalador e next... verifica em select componentes se estão marcadas as janelas: **Git Bash Here**, e **Git Gui Here**, pode-se também adicionar ícones no desktop (área de trabalho) ...next... em **configuring extra options**, marque os <u>dois Enable</u>, **file system caching** e **symbolic links** e na ultima tela deixa as duas opções desmarcadas e prossegue instalação, depois desmarca as duas opção pra que não se veja nota de lançamento. Verifica pesquisando no windows se Git está lá.

### Entendendo como o git funciona por baixo dos panos:

#### Sha1 

![image-20220617204124129](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617204124129.png)



Embaralha suas informações de um jeito muito específico:



![image-20220617204150866](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617204150866.png)

Identifica os arquivos de uma forma rápida e segura, ex:

![image-20220617204239747](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617204239747.png)

### Trabalhando com o Git:

Na área onde está o arquivo a ser trabalhado, com o botão direito do mouse aperta **Git Basch Here**

![image-20220617204736423](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617204736423.png)

No botão direito superior da tela aperta e options e muda o tema do seu terminal para o de seua preferência e salva.

![image-20220617204605053](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617204605053.png)

Quando estamos lidando com terminal colocamos sempre o nome do programa na frente. Estamos chamando pelo terminal o Git e o comando específico dele, como por exemplo:

- git init
- git add
- git commit

### Criando um repositório:

Já abrimos o git bash no local onde estão nossos arquivos criados e começamos com o comando **ls** pra listar. Entramos na pasta que desejamos com o comando **cd** e o nome da pasta, que pode ser auto completada pelo table. Pra limpar o terminal usa as telas **ctrl l**

Para visualizar arquivos ocultos que são pasta com um ponto na frente, usamos uma flex específica no comando ls que é **-a**:

**ls -a**

Pra voltar um nível, utiliza o comando **cd ..** (cd espaço ..)

### Configurações iniciais: 

Se é a primeira que o utiliza ele vai pedir um name, um apelido e um email, porque quando o objeto commit é criado ele é criado com um autor, pra quando se gerar um commit ele tenha um autor atrelado á ele;  então vamos rodar o segundo comando: **git config --global user.email "meuemail@gmail.com"** (a gente pode citá-la de forma global ou somente pra esse repositório) enter e git config --global user.name Nome) De preferência, utilize o mesmo email e apelido da sua conta do Github.

Utilize se possível ao invés do bloco de notas o Typora.

Voltando ao terminal  vamos *commitar* o arquivo criado; **git status** informa a situação atual .

**git add *** e enter

depois, **git commit -m "commit inicial"**

***Nota:*** Os commits são objetos do git que dão significados as operações e esses objetos em si carregam uma mensagem de texto juntamente com outros metadados como autor.



## Trabalhando com o github 

 Vamos criar uma conta e um repositório remoto e vamos apontar o nosso código na nossa máquina no nosso repositório local para um repositório remoto:

Criando conta: Sign up  e seguir os passos. É importante usar o mesmo email que foi configurado o git, mas se preciso for:

### Mudando seu email, user e nikename

No terminal digite: **git config --list**

Vai trazer todas a lista de configurações que estão no seu git, inclusive o email criado e o nike name. Da um **q** pra sair.

Se preciso for posso alterar isso: Então digitar o comando específico:

**git config --global --unset user.email** pra trocar email 

**git config --global --unset user.nickname**

**git config --global --unset user.name**

Pelas flechinas, pode-se navegar no histórico do terminal, assim voltando em **git config --list** vê-se que nem meu email e apelido aparecem mais lá e para criá-los:

**git config --global user.email** "meuemail@gmail.com" e o mesmo com o nikename

**git config --global user.nickname** "Apelido"

**git config --global user.name**  "Nome"

Se eu trouxer a configuração novamente: **git config --list** as alterações apareceram. De um **q** pra sair.

### Enviando um repositório pro github:

![image-20220617195042464](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617195042464.png)

 

![image-20220617195216262](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617195216262.png)

clica no botão new:

![image-20220617195309218](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617195309218.png)

Opcionalmente pode-se add um README, ele vai criar como se fosse a página inicial do nosso repositório, onde podemos colocar considerações iniciais, anotações, links úteis, coisa relacionadas ao que representam aquele repositório pra gente, como se fosse a home page do seu repositório caso já não o tenhamos criado em nossa máquina.

![image-20220617200602612](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617200602612.png)

![image-20220617195325575](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617195325575.png)

![image-20220617195421374](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617195421374.png)

nesse caso, ele diz que é um repositório vazio, temos que ir nosso repositório local e apontar pro repositório do github e aqui está nosso endereço do repositório do github:

![image-20220617195518647](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617195518647.png)

Assim copio com **ctrl C**

No git, limpa a tela **crtl l** e **ls** pra se situar

Vamos empurrar nosso repositório local pra um repositório remoto, pra uma origem remota

Então primeiro devemos adicionar a origem na qual estamos enviando esses arquivos com:

**git remote add origin https://github.com/Drlq/livro_receitas.git** e passar o link copiado do github e dar enter:

**git remote –v**

Vai aparecer pra mim a lista de repositórios remotos que tenho cadastrada:

![image-20220617195825828](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617195825828.png)

*Nota:* O origin é um apelido pra que a gente não precise ficar digitando o end https ou link o tempo inteiro.

E vou dar um git status:

Apenas pra se certificar de que não tem nenhuma tendência no repositório.

Pra levar nosso repositório local para o repositório remoto ele traduz do inglês diretamente como empurrar:

git push origin ( o apelido que foi dado pro link do nosso repositório la do github:)

**git push origin master**

Vai aparecer ess janela:

![image-20220617200141941](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617200141941.png)

Faz sua autenticação:

![image-20220617200210894](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617200210894.png)

E ele de fato enviou esse código, nosso repositório local para o remoto, e mostra pra onde ele enviou. Se eu voltar pro meu repositório do github e carregar a pagina (F5) já vai aparecer o nosso código:

![image-20220617200249788](C:\Users\PC\AppData\Roaming\Typora\typora-user-images\image-20220617200249788.png)

Aqui a aparece o início do sha, e se clicarmos nele poderemos ver nosso histórico sobre esse commit.







