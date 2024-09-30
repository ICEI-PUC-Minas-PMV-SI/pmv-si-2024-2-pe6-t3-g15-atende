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

![image](https://github.com/user-attachments/assets/71c301fe-6165-443d-b8e4-d22d9d5ddcd2)

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
- URL: /api/solicitacoes
- 
- Resposta:
  - Sucesso (200 OK)
    ```
    {
	"$id": "1",
	"items": {
		"$id": "2",
		"$values": [
			{
				"$id": "3",
				"titulo": "string",
				"descricao": "string",
				"dataCriacao": "2024-09-29T10:00:57.638",
				"dataAtualizacao": "2024-09-29T10:00:57.638",
				"status": 0,
				"id": 2
			},
			{
				"$id": "4",
				"titulo": "string",
				"descricao": "string",
				"dataCriacao": "2024-09-29T10:08:28.811",
				"dataAtualizacao": "2024-09-29T10:08:28.811",
				"status": 0,
				"id": 4
			},
			{
				"$id": "5",
				"titulo": "Buraco na pista",
				"descricao": "Buraco na pista na rua g,58 ",
				"dataCriacao": "2024-09-29T10:38:53.497",
				"dataAtualizacao": "2024-09-29T10:38:53.497",
				"status": 3,
				"id": 5
			},
			{
				"$id": "6",
				"titulo": "Rua Alagada",
				"descricao": "Rua alagando",
				"dataCriacao": "2024-09-29T12:28:02.713",
				"dataAtualizacao": "2024-09-29T12:28:02.713",
				"status": 0,
				"id": 6
			},
			{
				"$id": "7",
				"titulo": "Lampada com Defeito",
				"descricao": "Tem uma lampada queimada",
				"dataCriacao": "0001-01-01T00:00:00",
				"dataAtualizacao": null,
				"status": 0,
				"id": 7
			}
		]
	},
	"currentPage": 1,
	"pageSize": 10,
	"totalCount": 5
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

Testes Unitários:

# Referências

Inclua todas as referências (livros, artigos, sites, etc) utilizados no desenvolvimento do trabalho.
