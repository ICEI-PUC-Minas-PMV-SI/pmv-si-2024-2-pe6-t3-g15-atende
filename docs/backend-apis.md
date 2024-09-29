# APIs e Web Services
A API "Atende Cidadão" visa integrar prefeituras e empresas parceiras, permitindo a visualização e gestão centralizada das solicitações dos cidadãos. Através da API, empresas podem oferecer serviços com base nas demandas públicas, promovendo parcerias público-privadas. 

## Objetivos da API

* Facilitar o Gerenciamento de Solicitações: Permitir que prefituras e empresas conveniadas registrem, visualizem, acompanhando detalhes, status e histórico de cada solicitação.

* Promover a Integração Público-Privada: Proporcionar uma plataforma para que empresas parceiras possam se conectar às prefeituras, oferecendo soluções e serviços com base nas demandas dos cidadãos, criando parcerias eficientes.

* Oferecer Transparência e Colaboração: Facilitar o compartilhamento de dados e status em tempo real entre prefeituras e empresas conveniadas, promovendo uma comunicação eficaz e garantindo transparência na gestão das solicitações.

* Facilitar a Oferta de Serviços Personalizados: Permitir que empresas analisem as solicitações dos cidadãos e ofereçam serviços especializados às prefeituras, de acordo com as demandas e problemas detectados.

* Fornecer Relatórios e Análises: Disponibilizar relatórios detalhados e métricas sobre as solicitações, permitindo que prefeituras e empresas conveniadas avaliem o desempenho, identificando áreas de melhoria e oportunidades de parceria.


## Arquitetura
![arq](https://raw.githubusercontent.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-2-pe6-t3-g15-atende/refs/heads/main/docs/img/%7BApi%7D.png)

## Modelagem da Aplicação
[Descreva a modelagem da aplicação, incluindo a estrutura de dados, diagramas de classes ou entidades, e outras representações visuais relevantes.]


## Fluxo de Dados

[Diagrama ou descrição do fluxo de dados na aplicação.]

## Requisitos Funcionais

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|----|
|RF-01| Cadastro das solicitações. | 
|RF-02| Gerenciamento das solicitações. | 
|RF-03| Gerenciamento dos serviços.  | 
|RF-04| Cadastros dos serviços.  | 

## Requisitos Não Funcionais

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|----|
|RF-01| A API deve ser capaz de lidar com um grande volume de solicitações, tanto de cidadãos quanto de empresas parceiras. | 
|RF-02| A API deve estar disponível 24 horas por dia, 7 dias por semana, com alta disponibilidade e tempo de resposta rápido.|
|RF-03| A API deve utilizar banco de dados relacional.|

## Tecnologias Utilizadas

* PHP: A linguagem de programação que serve como base para a construção da aplicação. O PHP é amplamente utilizado para desenvolvimento web, sendo conhecido por sua facilidade de aprendizado e grande comunidade.

* Laravel: Um framework PHP que agiliza o desenvolvimento de aplicações web, fornecendo uma estrutura robusta e organizada. Com o Laravel, é possível criar APIs RESTful de forma eficiente e segura.

* PostgreSQL: Um banco de dados relacional poderoso e escalável, ideal para armazenar grandes volumes de dados. O PostgreSQL é conhecido por sua confiabilidade e flexibilidade.

* Eloquent ORM: Fornecido pelo Laravel, o Eloquent ORM permite que você interaja com o banco de dados PostgreSQL utilizando objetos PHP. Isso simplifica significativamente a escrita de consultas SQL e o gerenciamento de dados.

* JWT (JSON Web Tokens): Uma tecnologia de autenticação e autorização que permite criar tokens seguros para autenticar usuários e controlar o acesso a recursos da API. JWTs são compactas, seguras e fáceis de usar.

## API Endpoints

[Liste os principais endpoints da API, incluindo as operações disponíveis, os parâmetros esperados e as respostas retornadas.]

### Endpoint 1
- Método: GET
- URL: /endpoint1
- Parâmetros:
  - param1: [descrição]
- Resposta:
  - Sucesso (200 OK)
    ```
    {
      "message": "Success",
      "data": {
        ...
      }
    }
    ```
  - Erro (4XX, 5XX)
    ```
    {
      "message": "Error",
      "error": {
        ...
      }
    }
    ```


## Considerações de Segurança

Será utilizada o uso de JWT (JSON Web Tokens), proporcionando uma forma eficaz de autenticação e autorização.

Autenticação com JWT: Após o login, o servidor gerará um JWT contendo as credenciais e permissões do usuário. Esse token será enviado nas requisições à API, garantindo que apenas usuários autenticados possam acessar os recursos protegidos.

Autorização de Acesso: O JWT permitirá o controle de permissões, verificando se o usuário tem as credenciais necessárias para realizar operações específicas, como registro de demandas, consulta de status ou acesso a dados administrativos.

Expiração e Assinatura de Tokens: Os tokens terão uma data de expiração para limitar o tempo de sessão, além de serem assinados, garantindo que não possam ser modificados ou reutilizados indevidamente, oferecendo uma camada adicional de segurança.

## Implantação

[Instruções para implantar a aplicação distribuída em um ambiente de produção.]

1. Defina os requisitos de hardware e software necessários para implantar a aplicação em um ambiente de produção.
2. Escolha uma plataforma de hospedagem adequada, como um provedor de nuvem ou um servidor dedicado.
3. Configure o ambiente de implantação, incluindo a instalação de dependências e configuração de variáveis de ambiente.
4. Faça o deploy da aplicação no ambiente escolhido, seguindo as instruções específicas da plataforma de hospedagem.
5. Realize testes para garantir que a aplicação esteja funcionando corretamente no ambiente de produção.

## Testes

[Descreva a estratégia de teste, incluindo os tipos de teste a serem realizados (unitários, integração, carga, etc.) e as ferramentas a serem utilizadas.]

1. Crie casos de teste para cobrir todos os requisitos funcionais e não funcionais da aplicação.
2. Implemente testes unitários para testar unidades individuais de código, como funções e classes.
3. Realize testes de integração para verificar a interação correta entre os componentes da aplicação.
4. Execute testes de carga para avaliar o desempenho da aplicação sob carga significativa.
5. Utilize ferramentas de teste adequadas, como frameworks de teste e ferramentas de automação de teste, para agilizar o processo de teste.

# Referências

Inclua todas as referências (livros, artigos, sites, etc) utilizados no desenvolvimento do trabalho.
