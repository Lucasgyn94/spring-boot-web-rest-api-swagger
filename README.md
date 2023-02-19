# spring-boot-web-rest-api-swagger
Criando uma API RESTful com spring boot web e swagger e Maven no gerenciamento de nossas dependências.

==> API
* Uma API (Programm Application Interface) é um código programável que faz a "ponte" de comunicação entre duas aplicações distintas.

==> REST e RESTful
* A API REST (representaional state transfer) é como um guia de boas práticas e RESTful é a capacidade de determinado sistema aplicar os príncipios de REST.

==> PRINCÍPIOS
Características para que seja uma API RESTful:
* cliente - servidor: aprimorar a portabilidade entre várias plataformas de interface do lado usuário e do servidor, permitindo uma evolução independente do sistema.

* interface uniforme - representa uma interação uniforme entre cliente e servidor.

* stateless: indica que a cada interação via API tem acesso a dados completos e compreensíveis

* cache: necessário para reduzior o tempo médio de resposta, melhorar a eficiência, desempenho e escalabilidade da comunicação.

* camadas: permite que a arquitetura seja menos complexa e altamente flexível

==> Nível de maturidade
Para padronizar e facilitar o desenvolvimento de APIs REST, Leonard Richardson propôs um modelo de maturidade para esse tipo de API, definido em 4 níveis:
Level 3: Hypermedia Controls
Level 2: HTTP Verbs
Level 1: Resources
Level 0: The Swamp of POX

* GET : retorna/pesquisa dados
* POST: Grava dados
* PUT: altera/atualiza dados
* DELETE: deleta dados

==> CONTROLLER
É um recurso que disponibiliza as funcionalidades de negócio da aplicação através do protocolo HTTP. 

-> @RestController: responsável por designar o bean de component que suporta requisições HTTP com bane na arquitetura REST.

-> @RequestMapping("prefix"): determina qual a URI comum para todos os recursos disponibilizados pelo controller

-> @GetMapping: Determina que o método aceitará requisições HTTP do tipo GET.

-> @PostMapping: Determina que o método aceitará requisições HTTP do tipo POST.

-> @PutMapping: Determina que o método aceitará requisições HTTP do tipo PUT.

-> @DeleteMapping: Determina que o método aceitará requisições HTTP do tipo DELETE.

-> @RequestBody: converte um JSON para o tipo do objeto esperado como parâmetro no método.

-> @PatchVariable: Consegue determinar que parte da URI será composta por parâmetros recebidos nas requisições.

=> CONTROLE DE USUÁRIOS
Vamos disponibilizar as funcionalidades de CRUD da entidade através de uma API.

==> SWAGGER
É uma linguagem de descrição de interface para descrever APIs RESTful expressas usando JSON. O Swagger é usado junto com um conjunto de ferramentas de softwares de código aberto para projetar, construir, documentar e usar serviços da Web RESTful.
