<p align="center">


<img src="https://about.gitlab.com/images/blogimages/moving-to-gitlab-cover.png" alt="Sublime's custom image"/>

</p>


# Git precisa fazer sentido

Um dos maiores problemas de tecnologia é " Um time desordenado "
Lazy sysadmin, Programers e PO's. Imagine um time que não consegue entrar em concordancia em suas mudanças e que constantemente estão revendo suas formas de agir de maneira desordenada e sem interação.

Hoje, tanto o produto quanto a infraestrutura são parte do repositório da empresa. Então podemos dizer que 100% do patrimoónio de uma empresa estará em seu repositório git.

um empresa que tem um gitlab onpremisse, sem backup de disco, com anos de desenvolvimento dependendo de um hardware velho e ultrapassado se preocupa com a segurança de seu código ? 
Sim foi uma retórica.

É de suma importancia garantir **INTEGRIDADE**, parte do dever de nossos amigos de SI ( Segurança da informação ).

Então para que possamos ir em partes, como decidimos a melhor estratégia para nossos repositórios ?

Quais as melhores opções ?

Vamos iniciar com os Open Sources ... Teriamos então gitlab que por sua vez é o mais famoso, Gogs que é legal mas não tanto e o Gittea, que é super leve e compacto e faz somente seu papel ... **GUARDAR CODIGO**

Apesar de ser um repositório, com a evolução do devops e da tecnologia, os servidores de versionamento de código começaram a acumular algumas funções e dentre os opensource podemos dizer que o gitlab se sai bem nesse acumulo sendo ele também um repositório de container ( Muito fácil de se configurar por sinal ), SCM ( Servidor de Versionamento de código), Pipeline para CI/DC alem de integrar-se com outras ferramentas de forma nativa indo um tanto além de um simples servidor que guarda códigos.


