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

![image](https://github.com/user-attachments/assets/71c301fe-6165-443d-b8e4-d22d9d5ddcd2)

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

### Endpoint 1
- Método: GET
- URL: /api/servicos
- 
- Resposta:
  - Sucesso (200 OK)
    ```
    {
    "status": true,
    "message": "Serviços consultados com sucesso!",
    "servicos": {
        "current_page": 1,
        "data": [
            {
                "id": 3,
                "user_id": 1,
                "empresa": "EcoColeta",
                "cpf_cnpj": "233.280.938-90",
                "descricao": "Coleta e reciclagem de resíduos sólidos, promovendo a sustentabilidade urbana.",
                "status": "disponivel",
                "categoria_id": 5,
                "created_at": "2024-09-29T21:25:25.000000Z",
                "updated_at": "2024-09-29T21:25:25.000000Z"
            },
            {
                "id": 4,
                "user_id": 1,
                "empresa": "LuzCerta",
                "cpf_cnpj": "236.530.903-48",
                "descricao": "Manutenção da iluminação pública, garantindo segurança e eficiência.",
                "status": "disponivel",
                "categoria_id": 5,
                "created_at": "2024-09-29T21:25:25.000000Z",
                "updated_at": "2024-09-29T21:25:25.000000Z"
            },
            {
                "id": 5,
                "user_id": 1,
                "empresa": "Pavimenta Brasil",
                "cpf_cnpj": "869.778.902-82",
                "descricao": "Pavimentação e reparo de estradas e vias urbanas.",
                "status": "disponivel",
                "categoria_id": 2,
                "created_at": "2024-09-29T21:25:25.000000Z",
                "updated_at": "2024-09-29T21:25:25.000000Z"
            },
            {
                "id": 6,
                "user_id": 1,
                "empresa": "VerdeVivo",
                "cpf_cnpj": "071.880.548-56",
                "descricao": "Serviços de jardinagem e paisagismo para espaços públicos.",
                "status": "indisponivel",
                "categoria_id": 1,
                "created_at": "2024-09-29T21:25:25.000000Z",
                "updated_at": "2024-09-29T21:25:25.000000Z"
            },
            {
                "id": 7,
                "user_id": 1,
                "empresa": "ConstruMais",
                "cpf_cnpj": "703.247.960-39",
                "descricao": "Construção de equipamentos públicos, como escolas e centros de saúde.",
                "status": "disponivel",
                "categoria_id": 3,
                "created_at": "2024-09-29T21:25:25.000000Z",
                "updated_at": "2024-09-29T21:25:25.000000Z"
            },
            {
                "id": 8,
                "user_id": 1,
                "empresa": "Limpeza Total",
                "cpf_cnpj": "000.353.380-43",
                "descricao": "Gestão e manutenção de espaços verdes e parques públicos.",
                "status": "indisponivel",
                "categoria_id": 4,
                "created_at": "2024-09-29T21:25:25.000000Z",
                "updated_at": "2024-09-29T21:25:25.000000Z"
            },
            {
                "id": 9,
                "user_id": 1,
                "empresa": "Transito-Block",
                "cpf_cnpj": "687.654.286-53",
                "descricao": "Sinalização e gestão de trânsito para segurança urbana.",
                "status": "indisponivel",
                "categoria_id": 4,
                "created_at": "2024-09-29T21:25:25.000000Z",
                "updated_at": "2024-09-29T21:25:25.000000Z"
            },
            {
                "id": 10,
                "user_id": 1,
                "empresa": "Cultura em Foco",
                "cpf_cnpj": "784.491.782-49",
                "descricao": "Organização de eventos culturais e atividades comunitárias.",
                "status": "disponivel",
                "categoria_id": 5,
                "created_at": "2024-09-29T21:25:25.000000Z",
                "updated_at": "2024-09-29T21:25:25.000000Z"
            },
            {
                "id": 11,
                "user_id": 1,
                "empresa": "EducaAmbiente",
                "cpf_cnpj": "829.407.859-71",
                "descricao": "Educação ambiental e programas de conscientização comunitária.",
                "status": "indisponivel",
                "categoria_id": 3,
                "created_at": "2024-09-29T21:25:25.000000Z",
                "updated_at": "2024-09-29T21:25:25.000000Z"
            },
            {
                "id": 12,
                "user_id": 1,
                "empresa": "Dietrich LLC",
                "cpf_cnpj": "437.835.891-41",
                "descricao": "Assessoria em licenciamento ambiental e conformidade.",
                "status": "indisponivel",
                "categoria_id": 1,
                "created_at": "2024-09-29T21:25:25.000000Z",
                "updated_at": "2024-09-29T21:25:25.000000Z"
            }
        ],
        "first_page_url": "http://127.0.0.1:8000/api/servicos?page=1",
        "from": 1,
        "last_page": 1,
        "last_page_url": "http://127.0.0.1:8000/api/servicos?page=1",
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "http://127.0.0.1:8000/api/servicos?page=1",
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
        "path": "http://127.0.0.1:8000/api/servicos",
        "per_page": 10,
        "prev_page_url": null,
        "to": 10,
        "total": 10
    }
}

    ```
### Endpoint 2
- Método: POST
- URL: /api/register
- Parâmetros:
  - param1: name
  - param2: email
  - param3: password
- Resposta:
  - Sucesso (200 OK)
    ```
    {
    "status": true,
    "message": "Usuário criado com Sucesso",
    "token": "4|1qg97paiLgsSSSsRD6620mYaG3ZRwQpWIiE31bQRe637b2f1"
    }
    ```
  - Erro (401)
    ```
    {
      "message": "Error",
      "error": {
        {
        "status": false,
        "message": "Erro de validação",
        "errors": {
        "name": [
            "The name field is required."
        ],
        "email": [
            "The email has already been taken."
        ]
    }
}
      }
    }
    ```

### Endpoint 3
- Método: POST
- URL: /api/login
- Parâmetros:
  - param1: email
  - param2: password
- Resposta:
  - Sucesso (200 OK)
    ```
    {
    "status": true,
    "message": "Login realizado com sucesso!",
    "token": "1|Alnm3hwcoTWnd5vpuNFKiykwvHqrQeMb1XERtk5Z6577078d"
    }
    ```
  - Erro (401)
    ```
    {
      "message": "Error",
      "error": {
        {
          "status": false,
          "message": "Algo deu errado!"
        }
      }
    }
    ```

### Endpoint 4
- Método: POST
- URL: /api/servicos?nome_razaosocial=Empresa x&cpf_cnpj=144114141414&descricao=teste &categoria_id=1
- Parâmetros:
  - param1: nome_razaosocial
  - param2: cpf_cnpj
  - param3: descricao
  - param4: categoria_id
- Resposta:
  - Sucesso (200 OK)
    ```
    {
    "message": "Serviço criado com sucesso!"
    }
    ```
  - Erro (422)
    ```
    {
      "message": "Error",
      "error":
        {
    "message": "O campo CPF/CNPJ é obrigatório.",
    "errors": {
        "cpf_cnpj": [
            "O campo CPF/CNPJ é obrigatório."
        ]
    }
}
    }
    ```

  ### Endpoint 5
- Método: PUT
- URL: /api/servicos/update/1?nome_razaosocial=TESTE EMPRESA 2&cpf_cnpj=1231323333&descricao=Empresa Teste W
- Parâmetros:
  - param1: nome_razaosocial
  - param2: cpf_cnpj
  - param3: descricao
- Resposta:
  - Sucesso (200 OK)
    ```
    {
    "message": "Serviço atualizado com sucesso!"
    }
    ```
  - Erro (404)
    ```
    {
      "message": "Error",
      "error":
        {
    "message": "Serviço não encontrado"
        }
    }
    ```
  ### Endpoint 6
- Método: DELETE
- URL: /api/servicos/delete/1

- Resposta:
  - Sucesso (200 OK)
    ```
    {
    "message": "Serviço  deletado com sucesso!!"
    }
    ```
  - Erro (404)
    ```
    {
      "message": "Error",
      "error":
        {
    "message": "Serviço não encontrado"
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
