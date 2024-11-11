# APIs e Web Services
Facilitar a integração entre cidadãos e gestores municipais através de serviços web que promovem a comunicação eficiente e a gestão transparente das demandas públicas.

## Objetivos da API

* Gerenciamento centralizado de solicitações: Prover endpoints para que cidadãos enviem solicitações, reclamações e sugestões de forma organizada.

* Acompanhamento de demandas: Permitir que os gestores públicos atualizem o status das solicitações e que os cidadãos acompanhem essas mudanças em tempo real.

* Comunicação bidirecional: Facilitar notificações e mensagens automatizadas entre cidadãos e gestores, garantindo transparência e eficiência.

* Fornecer Relatórios e Análises: Disponibilizar relatórios detalhados e métricas sobre as solicitações, permitindo que prefeituras avaliem o desempenho, identificando áreas de melhorias.


## Arquitetura
![image](https://raw.githubusercontent.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-2-pe6-t3-g15-atende/refs/heads/main/docs/img/%7BApi%7D%20(2).png)

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

* ASP.NET Core: Para o desenvolvimento da API, garantindo desempenho, segurança e suporte a padrões modernos de arquitetura RESTful.

* MySQL: Banco de dados relacional para armazenamento de dados das solicitações e usuários, integrado ao ASP.NET Core via Entity Framework.

* Identity Server/Autenticação JWT: Para gerenciar autenticação e autorização, garantindo acesso seguro à API.

* JWT (JSON Web Tokens): Uma tecnologia de autenticação e autorização que permite criar tokens seguros para autenticar usuários e controlar o acesso a recursos da API. JWTs são compactas, seguras e fáceis de usar.

* Docker: Para empacotamento e implantação da API de forma portátil e escalável.

## API Endpoints

### Endpoint 1
- Método: GET
- URL: https://localhost:44374/api/Solicitacoes
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


    ```
### Endpoint 2
- Método: GET
- URL: https://localhost:44374/api/Solicitacoes/5

- Resposta:
  - Sucesso (200 OK)
    ```
    {
	"$id": "1",
	"titulo": "Buraco na pista",
	"descricao": "Buraco na pista na rua g,58 ",
	"dataCriacao": "2024-09-29T10:38:53.497",
	"dataAtualizacao": "2024-09-29T10:38:53.497",
	"status": 3,
	"id": 5
}
    ```

### Endpoint 3
- Método: Put
- URL: https://localhost:44374/api/solicitacoes/5

- Resposta:
  - Sucesso (200 OK)
    ```
      {
	"$id": "1",
	"titulo": "Buraco na pista",
	"descricao": "Buraco na pista na rua g,58 ",
	"dataCriacao": "2024-09-29T10:38:53.497",
	"dataAtualizacao": "2024-09-29T10:38:53.497",
	"status": 1,
	"id": 5
}
    ```

### Endpoint 4
- Método: POST
- URL: https://localhost:44374/api/Usuarios/login
-- Resposta:
  - Sucesso (200 OK)
    ```
    {
  "$id": "1",
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJuYW1laWQiOiIzIiwidW5pcXVlX25hbWUiOiJzdHJpbmciLCJlbWFpbCI6InVzZXJAZXhhbXBsZS5jb20iLCJyb2xlIjoiQ2xpZW50ZSIsIm5iZiI6MTcyNzczNDU2NSwiZXhwIjoxNzI3NzYzMzY1LCJpYXQiOjE3Mjc3MzQ1NjV9.TJwbGURR3WBzDHxe6VQ-idUhOx4sRp5VZIOU0xVDC2M"
}
    ```

  ### Endpoint 5
- Método: DELETE
- URL: https://localhost:44374/api/Solicitacoes/5
- Resposta:
  - Sucesso (401 Unauthorized)
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

Testes Unitários:

# Referências

Inclua todas as referências (livros, artigos, sites, etc) utilizados no desenvolvimento do trabalho.
