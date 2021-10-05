# O que é o git ?

Git e um git server ( Ou service ) é uma ferramenta de versionamento que permite que contrele a mudança de seu codigo e projetos de forma distribuida e colaborativa.


### O que é um commit

Commit é a ação que marca a conclusão de uma fase do projeto.
Dentro do desenvolvimento e das melhores praticas do versionamento de codigo, fazer um commit somente com códigos que tenham assuntos correlatos
é considerado uma das melhores praticas.

### O que é staging area 

Staging area é a area que mantém os arquivos salvos para o proximo commit.

> Imagine que estou desenvolvento um software e após a primeira fase eu tenho desenvovlido parte do front e do backend.
Eu executo dois commits separados, um para os arquivos e partes de arquivos relativos ao front e outro relativo ao backend par aque assim eu tenha maior facilidade de voltar minha mudança. Tenha em mente que o commit não é um backup do seu código ma sim um **estado** onde podemos voltar.  

#### Exemplo

Criei 3 arquivos :

- Frented.nada; 
- Backend.nada e
- Meioarquivo.nada

Após a criação dos mesmos eu rodo **git add Frented.nada** em seguida **git add -p Meioarquivo.nada**. Em meio arquivo eu tenho parte do codigo de backend e de front end misturado em um arquivo só ( Por mais que soe absurdo em cenários reais ), usando **git add -p Meioarquivo.nada**, eu posso escolher somente a parte que comete ao fronted e após enviar para staging levar ele ao repósitório remoto com **git push**. Em seguida, todo o restante é parte do backend, logo posso rodar um **git add .** para adicionar todas as mudanças em staging e enviar ao repositório remoto com **git push** em seguida seguro que de todos os commits fazem parte dos mesmos assuntos.
</br>
</br>
<p align="center">


<img src="https://github.com/rosthansilva/HowToGit/blob/main/img/commit.png" alt="Sublime's custom image"/>

</p>


## Commit like Pro

Qual o Nivel de importancia de um commit ?
O nivel de importancia de um commit pode ser medido simplesmente pelo nivel de criticidade da sua aplicação para sua empresa ou seus clientes.
Se não há a necessidade de uma reversão de seu codigo devido a um erro de um Junior ou um pleno que acidentalmente subiu em sua rede um codigo que não deveria ou não testou o bastante o codigo antes de subir para o reporitório ( O que é muito comum em pequenos times).

O Commit leva com ele uma mensagem e é uma boa pratica que além de um commit ter um assunto/tarefa especifica a ser subido no repositório, ele também tenha uma mensagem com informações relevantes para o trabalho e não seja uma especie de backup do trabalho do membro da squad que cada vez qaue altera algo comita sem saber o que dizer e acaba rodando um git commit -m "a" para aprovação.

como já foi visto acima, a sintax para comitar seu codigo é simples :

```
## comitando um codigo qualquer ##
git commit -m "E lá vamos nós"
```

Dessa forma o git irá enviar seu codigo junto a uma mensagem aos usuários do repositório.
caso prefira escrever essa mensagem diretamente com o seu editor de texto favorito pode rodar diretamente *git commit*
e o git irá abrir o seu editor de texto padrão para adição da mensagem que srá enviada com o commit.


## Como devo enviar um comit ?

Um commit é quase como um email, é uma marca sua naquele projeto e quanto mais clara for a sua comunicação mais fácil será o entendimento de quem junto com você trabalha.
Para seguir uma melhor pratica pense que o commit precisa de um Assunto, e um corpo assim como o email. O Assunto sendo o que foir feito e podendo até ficar em caixa alta e o interior do corpo com as mudanças feitas
Um exemplo bobo de commit :

```
git commit 

-- 

# Please enter the commit message for your changes. Lines starting
# with '#' will be ignored, and an empty message aborts the commit.
#
# On branch main
# Your branch is up to date with 'origin/main'.
#
# Changes to be committed:

DEU MERDA NO CARTÃO DA FABRICA
***

- Alteração no checkout
- alterado branch do git flow para master e não main
- agora quando o usuário loga parece um prompt que diz " Linux é melhor que windows"
- O som de login agora é a trilha do carro do ovo passando na sua rua
- o sapo não lava o pé
```

> muito provavelmente se não tem conhecimentos de linux o git abriu o vim e você ficou preso na tela de edição perdido.
No vim para iniciar a edição aperte a tecla I do seu teclado e conseguirá escrever. Com a tecla ask você encerra a edição voltando ao estado de comando e para sair do arquivo digite :wq! ou :x!. Viu só ? Simples como voar sem asas.


<p align="center">


<img src="https://c.tenor.com/F3c-Uuu99jkAAAAC/here-we-go-woody-woodpecker.gif" alt="Sublime's custom image"/>

</p>




## REcptulando 

- Staging é uma area de transferencia que prepara para o repositório remoto.
- Commit é um estado marcado do processo de produção que nos ajuda a entender o processo e se possível/necessário voltar a esse estado anterior
- Vim é melhor que nano
- Git é um comando para versionamento e o servidor é onde o codigo acaba ficando no fim das contas