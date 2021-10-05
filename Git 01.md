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

<p align="center">
![alt text](https://github.com/rosthansilva/HowToGit/blob/main/img/commit.png)
</p>