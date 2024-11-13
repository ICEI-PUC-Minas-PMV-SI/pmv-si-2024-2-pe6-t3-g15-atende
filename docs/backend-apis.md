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

![image](https://raw.githubusercontent.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-2-pe6-t3-g15-atende/refs/heads/main/docs/img/atende_db.png)

## Fluxo de Dados

[Diagrama ou descrição do fluxo de dados na aplicação.]

## Requisitos Funcionais

|ID    | Descrição do Requisito  |     |
|------|-----------------------------------------|----|
|RF-01| Cadastro das solicitações. | 
|RF-02| Gerenciamento das solicitações. | 

## Requisitos Não Funcionais

|ID    | Descrição do Requisito  |     |
|------|-----------------------------------------|----|
|RF-01| A API deve ser capaz de lidar com um grande volume de solicitações. | 
|RF-02| A API deve estar disponível 24 horas por dia, 7 dias por semana, com alta disponibilidade e tempo de resposta rápido.|
|RF-03| A API deve utilizar banco de dados relacional.|

## Tecnologias Utilizadas

* PHP: A linguagem de programação que serve como base para a construção da aplicação. O PHP é amplamente utilizado para desenvolvimento web, sendo conhecido por sua facilidade de aprendizado e grande comunidade.

* Laravel: Um framework PHP que agiliza o desenvolvimento de aplicações web, fornecendo uma estrutura robusta e organizada. Com o Laravel, é possível criar APIs RESTful de forma eficiente e segura.

* PostgreSQL: Um banco de dados relacional poderoso e escalável, ideal para armazenar grandes volumes de dados. O PostgreSQL é conhecido por sua confiabilidade e flexibilidade.
  
* Eloquent ORM: Fornecido pelo Laravel, o Eloquent ORM permite que você interaja com o banco de dados PostgreSQL utilizando objetos PHP. Isso simplifica significativamente a escrita de consultas SQL e o gerenciamento de dados.

* JWT (JSON Web Tokens): Uma tecnologia de autenticação e autorização que permite criar tokens seguros para autenticar usuários e controlar o acesso a recursos da API. JWTs são compactas, seguras e fáceis de usar.

* Docker: Para empacotamento e implantação da API de forma portátil e escalável.

## API Endpoints

### Endpoint 1
- Método: GET
- URL: `/api/solicitacoes`
- Descrição: Retorna uma lista de solicitações com paginação.
- Resposta:
  - Sucesso (200 OK)
    ```
    {
      "status": true,
      "message": "Solicitações consultadas com sucesso!",
      "solicitacoes": {
        "current_page": 1,
        "data": [
          {
            "id": 3,
            "user_id": 1,
            "endereco": "Avenida Principal, 100",
            "descricao": "Reparação de buraco na via.",
            "status": "pendente",
            "id_categoria": 2,
            "data_cadastro": "2024-11-12T21:25:25.000000Z",
            "data_atualizacao": "2024-11-12T21:25:25.000000Z"
          },
          {
            "id": 4,
            "user_id": 1,
            "endereco": "Rua Flores, 50",
            "descricao": "Solicitação de poda de árvores.",
            "status": "em andamento",
            "id_categoria": 1,
            "data_cadastro": "2024-11-12T21:25:25.000000Z",
            "data_atualizacao": "2024-11-12T21:25:25.000000Z"
          }
        ],
        "first_page_url": "http://127.0.0.1:8000/api/solicitacoes?page=1",
        "from": 1,
        "last_page": 1,
        "last_page_url": "http://127.0.0.1:8000/api/solicitacoes?page=1",
        "links": [
          {
            "url": null,
            "label": "&laquo; Previous",
            "active": false
          },
          {
            "url": "http://127.0.0.1:8000/api/solicitacoes?page=1",
            "label": "1",
            "active": true
          },
          {
            "url": null,
            "label": "Next &raquo;",
            "active": false
          }
        ],
        "next_page_url": null,
        "path": "http://127.0.0.1:8000/api/solicitacoes",
        "per_page": 10,
        "prev_page_url": null,
        "to": 2,
        "total": 2
      }
    }
    ```

### Endpoint 2
- Método: POST
- URL: `/api/solicitacoes`
- Parâmetros:
  - `descricao` (string, obrigatório)
  - `endereco` (string, obrigatório)
  - `id_categoria` (inteiro, obrigatório)
  - `imagem` (arquivo de imagem, opcional)
- Resposta:
  - Sucesso (201 Created)
    ```
    {
      "status": true,
      "message": "Solicitação criada com sucesso!",
      "solicitacao": {
        "id": 5,
        "user_id": 1,
        "endereco": "Rua Nova, 123",
        "descricao": "Reparação na calçada",
        "status": "pendente",
        "id_categoria": 3,
        "data_cadastro": "2024-11-12T21:25:25.000000Z",
        "data_atualizacao": null
      }
    }
    ```
  - Erro (422 Unprocessable Entity)
    ```
    {
      "status": false,
      "message": "Erro de validação",
      "errors": {
        "descricao": ["O campo descrição é obrigatório."],
        "endereco": ["O campo endereço é obrigatório."]
      }
    }
    ```

### Endpoint 3
- Método: GET
- URL: `/api/solicitacoes/{id}`
- Parâmetros: `id` (ID da solicitação)
- Resposta:
  - Sucesso (200 OK)
    ```
    {
      "status": true,
      "message": "Solicitação consultada com sucesso!",
      "solicitacao": {
        "id": 3,
        "user_id": 1,
        "endereco": "Avenida Principal, 100",
        "descricao": "Reparação de buraco na via.",
        "status": "pendente",
        "id_categoria": 2,
        "data_cadastro": "2024-11-12T21:25:25.000000Z",
        "data_atualizacao": "2024-11-12T21:25:25.000000Z"
      }
    }
    ```
  - Erro (404 Not Found)
    ```
    {
      "status": false,
      "message": "Solicitação não encontrada"
    }
    ```

### Endpoint 4
- Método: PUT
- URL: `/api/solicitacoes/update/{id}`
- Parâmetros:
  - `descricao` (string, obrigatório)
  - `endereco` (string, obrigatório)
  - `id_categoria` (inteiro, obrigatório)
  - `imagem` (arquivo de imagem, opcional)
- Resposta:
  - Sucesso (200 OK)
    ```
    {
      "status": true,
      "message": "Solicitação atualizada com sucesso!"
    }
    ```
  - Erro (404 Not Found)
    ```
    {
      "status": false,
      "message": "Solicitação não encontrada"
    }
    ```

### Endpoint 5
- Método: DELETE
- URL: `/api/solicitacoes/delete/{id}`
- Parâmetros: `id` (ID da solicitação)
- Resposta:
  - Sucesso (200 OK)
    ```
    {
      "status": true,
      "message": "Solicitação deletada com sucesso!"
    }
    ```
  - Erro (404 Not Found)
    ```
    {
      "status": false,
      "message": "Solicitação não encontrada"
    }
    ```
"""
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

Testes Unitários:

Verificam o funcionamento individual de funções e métodos relacionados à criação, atualização, listagem e exclusão de serviços. Os testes realizados incluem:
* it_can_create_a_servico(): Testa a criação de um serviço e verifica se os dados são armazenados corretamente no banco de dados.
* it_can_update_a_servico(): Testa a atualização de um serviço existente, garantindo que os dados sejam alterados corretamente.
* it_can_list_servicos(): Testa a listagem de serviços, garantindo que a estrutura da resposta JSON esteja correta.
* it_can_delete_a_servico(): Testa a exclusão de um serviço, verificando se ele foi removido do banco de dados.
  
Ferramentas Utilizadas:

* PHPUnit: Para implementar e executar testes unitários e de integração no Laravel.
* Postman: Para automação de testes de API e testes manuais.

# Referências

Inclua todas as referências (livros, artigos, sites, etc) utilizados no desenvolvimento do trabalho.
