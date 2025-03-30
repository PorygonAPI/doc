<h1 align="center">Regras para Contribuição - Equipe Porygon</h1>

<h1 align="center">Sumário</h1>

<p align="center">
  <a href ="#geral"> GERAL </a>  •
  <a href ="#strike"> STRIKE </a>  •
  <a href ="#daily"> DAILY </a>  •
  <a href="#padrões"> PADRÕES </a> •
  <a href="#commit"> COMMIT </a> •
  <a href ="#pull-request"> PULL REQUEST </a>  •
  <a href ="#branch"> BRANCH </a>
</p>

## GERAL
Este projeto é acadêmico e realizado em equipe, exigindo colaboração, comprometimento e responsabilidade de todos os integrantes, sem distinção de funções. *Embora os papéis de Product Owner (PO) e Scrum Master (SM) atuem como facilitadores e mediadores, cabe a todos os membros contribuir para a melhoria contínua do código, desenvolver um front-end com boa experiência de usuário, ajustar as tasks e garantir a qualidade dos resultados entregues.*

É fundamental que os cards das tasks sejam revisados tanto por quem os desenvolve quanto por quem realiza a revisão ou os testes. Se houver dúvidas ou necessidade de validação de alguma modificação ou melhoria, além da quebra da task e criação de um card complementar, a comunicação deve ser feita através do grupo no WhatsApp. Alternativamente, os membros podem entrar em contato diretamente com a PO ou o SM para validação.

Os wireframes e o backlog servem como ferramentas de validação para o cliente, proporcionando uma visão clara do que será entregue. No entanto, **essas definições não são fixas ou imutáveis**, podendo ser ajustadas conforme o andamento do projeto e conforme novas necessidades surgirem durante o desenvolvimento.

## STRIKE
Ao assumir uma task, o membro deve revisar o card e os detalhamentos fornecidos, solicitando esclarecimentos adicionais, se necessário. A verificação de dependências e a adesão aos padrões estabelecidos no código também são de responsabilidade do responsável pela task. Caso existam dúvidas relacionadas ao código, elas devem ser resolvidas rapidamente, uma vez que qualquer atraso pode comprometer as entregas. Se o responsável pela task não conseguir finalizá-la, **é essencial comunicar o grupo com antecedência para que outra pessoa possa assumir**.

### CRITÉRIOS:
 * Não entregar uma task sem aviso prévio. Deve-se informar ao grupo pelo menos 3-2 dias antes do prazo final se a entrega não poderá ser realizada;

 * Entregar uma task de forma insatisfatória ou incompleta sem justificativa válida;

* Não entregar uma task completa durante todo o prazo da Sprint.

> **1ª Ocorrência: Aviso verbal**

> **2ª Ocorrência: Aplicação de um strike**

### PENALIDADES:
>1° Strike: Alerta oficial e conversa para o ajuste de postura.

>2° Strike: Reunião entre o PO e o SM com uma conversa para aviso da redução na nota da participação.

>3° Strike: Será feita uma reunião com os membros do grupo para discussão da exclusão do membro e redistribuição das tarefas.

## DAILY
Para garantir que todos estejam informados e que o fluxo de trabalho seja contínuo, as dailies serão realizadas de forma assíncrona a cada 2 dias. Cada integrante deverá atualizar o grupo do WhatsApp nas terças, quintas e sábado/domingo informando sobre o progresso das tasks, se já foi aberta uma Pull Request (PR), e se precisa de ajuda em algum ponto específico.

### FORMATO:

Ex1: Server, Task #0 – Resumo do progresso.

Ex2: Client, Task #0 – Resumo do progresso.

Ex3: Doc, Task #0 – Resumo do progresso.

---

## COMMIT

Os commits devem ser descritivos e seguir um padrão definido para manter a rastreabilidade e a clareza no histórico do repositório.

### ESTRUTURA:

`<tipo> (#<id_demanda1>, #<id_demanda2>, ..., #<id_demandaN>): <descrição da entrega feita no commit>`

Tipos de commit:

* feat  : Adiciona uma nova funcionalidade. 
* fix  : Corrige um bug. 
* docs  : Alterações na documentação. 
* style  : Mudanças de formatação, espaçamento, etc.,  que não afetam a funcionalidade. 
* refactor  : Refatoramento de código sem mudança de funcionalidade. 
* test  : Adição ou modificação de testes. 
* chore  : Tarefas de build, configurações, dependências,  etc. 

### EXEMPLO: 

`feat (#7): adicionar endpoint de listagem de usuários`

_Issue: Implementado o endpoint GET/usuarios para listar todos os usuários cadastrados._

## PULL REQUEST

Os Pull Requests devem seguir a mesma mensagem que os commits. 

### EXEMPLO: 

`feat (#7): adicionar endpoint de listagem de usuários` 

_Descrição: #7 Foi criado um endpoint para listar todos os usuários, utilize a rota localhost:8080/usuario_

Inclua uma breve descrição do que foi feito, bem como indicações para teste e prints. Para linkar um card, é necessário colocar o número da Issue acompanhada do #, devendo aparecer um pop-up para selecionar. 

Descrição:

* O que foi feito?  (Descreva a funcionalidade ou correção  realizada) 
* Como testar?  (Passos para validar as mudanças) 
* Dependências  (Se houver dependências de outras tarefas ou PRs) 
* Screenshots  (Se aplicável, incluir prints ou gifs para facilitar a revisão) 

## BRANCH

As branches devem seguir um padrão para facilitar a organização do repositório e a 
rastreabilidade das alterações.

Estrutura da branch: 

`<id_demanda1>, <id_demanda2>, ..., <id_demandaN>-<descricao>`

Em branch não usamos caracteres especiais e nem pontuações.
  
### EXEMPLOS:

`7-adicionar-endpoint-de-listagem-de-usuarios`
