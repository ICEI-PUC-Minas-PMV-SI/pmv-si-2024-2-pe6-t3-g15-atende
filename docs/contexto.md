# Introdução

O cenário dos processos administrativos evoluiu significativamente ao longo dos anos, com a tecnologia se tornando essencial para otimizar processos e melhorar a comunicação nas organizações. Essa evolução tecnológica não só aprimorou a eficiência operacional, mas também destacou a importância da satisfação do cliente no setor privado, com estratégias voltadas para a geração de valor e fidelização. No contexto governamental, o desafio de atender e comunicar-se efetivamente com os cidadãos permanece constante, exigindo que as estratégias públicas estejam alinhadas às expectativas da população. 

A informação, organizada e recuperada por Sistemas de Informação, é crucial para a gestão pública tomar decisões estratégicas baseadas no perfil dos cidadãos. 	Este trabalho propõe o desenvolvimento de um sistema de informação de Ouvidoria que auxilie no processo de organização das requisições dos cidadãos e ainda no processo de comunicação governo/cidadão, ou vice-versa. Dessa maneira, é possível traçar o perfil da população e aumentar a satisfação dos serviços prestados pela gestão pública. 

## Problema
Em geral, no setor público, a insatisfação dos cidadãos quanto à qualidade do serviço prestado é alarmante, tanto no que diz respeito à ineficiência, ineficácia e/ou a falta de respostas direcionadas, quanto às solicitações. Resultando na desmotivação deles em expressar suas preferências, em servidores públicos que deixam a desejar na execução de seus trabalhos e, consequentemente, em serviços que deixam de ser oferecidos como realmente deveriam. 

 Com grande frequência, percebem-se manifestos de cidadãos em redes sociais como o Facebook, onde, na maioria das vezes, são declarações negativas e não há ninguém responsável por responder esse manifesto, aumentando ainda mais o descontentamento da população quanto ao problema e causando uma grande repercussão. 

Outro empecilho encontrado nesse aspecto é a carência de um setor específico para o tratamento de questões relacionadas aos cidadãos, levando em conta que cada requisição, na maior parte das prefeituras, é feita em setores individuais, dificultando o processo de gestão das informações. 

## Objetivos

O objetivo geral deste trabalho é desenvolver um sistema web de ouvidoria para a Gestão Pública, permitindo assim que a população tenha participação efetiva no processo de gestão das cidades, de forma a otimizar a interação entre os cidadãos e os gestores municipais. 

Objetivos específicos:  

Os objetivos específicos deste trabalho são: 

1)	identificar quais os meios utilizados para gerenciamento de requisições enviadas pelos cidadãos; 

2)	reconhecer os fatores que motivam os cidadãos a expressar suas opiniões perante a prefeitura; 

3)	averiguar a conveniência de um sistema que estruture solicitações da população; 

4)	melhorar o processo de comunicação cidadão-prefeitura; 

5)	permitir registro da participação dos cidadãos com a prefeitura; 

6)	identificar os requisitos necessários para que o sistema se adéque ao perfil dos cidadãos e prefeituras (funcionalidades do sistema); 

## Justificativa

O atendimento efetivo e a participação ativa dos cidadãos na gestão das prefeituras são desafios constantes para os gestores. Assim como na rede privada, onde cliente é considerado a chave para o sucesso de uma organização, as gestões públicas vêm amadurecendo este conceito, buscando melhorar o relacionamento com os cidadãos por meio da aproximação e da obtenção de conhecimento. 

Melhorando assim o gerenciamento das relações com os cidadãos através de um sistema de informação web que possibilite aos gestores públicos a obtenção de informações relevantes para a tomada de decisão, direcionando-a ao perfil e necessidades explícitas da população. 

## Público-Alvo

Cidadãos, Servidores Públicos Operacionais, Gestores Públicos, Técnicos de Suporte e TI, Supervisores de Atendimento ao Cidadão 

# Especificações do Projeto

## Requisitos

As tabelas que se seguem apresentam os requisitos funcionais e não funcionais que detalham o escopo do projeto. Para determinar a prioridade de requisitos, aplicar uma técnica de priorização de requisitos e detalhar como a técnica foi aplicada.

### Requisitos Funcionais

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|----|
|RF-001| Permitir inclusão, exclusão e consulta dos dados das solicitações, usuários, finalidades, unidades, setores e bairros; | ALTA | 
|RF-002| Enviar e-mail para os usuários quando for incluída uma nova requisição;   | ALTA |
|RF-003| Enviar sms para os usuários quando for incluída uma nova requisição;  | MÉDIA |
|RF-004| Permitir que sejam enviados feedbacks referentes às solicitações.  | MÉDIA |
|RF-005| Emitir Relatórios  | MÉDIA |


### Requisitos não Funcionais

|ID     | Descrição do Requisito  |Prioridade |
|-------|-------------------------|----|
|RF-001| Possuir autenticação por login e senha | ALTA | 
|RF-002| O sistema deve trabalhar com ícones e cores que facilitem a utilização;   | ALTA |
|RF-003| O sistema deve conter botões de redirecionamento para as páginas de principais funções do website, com o intuito de melhorar a usabilidade do site;   | MÉDIA |
|RF-004| As senhas dos usuários deverão ser criptografadas;   | MÉDIA |
|RF-005| O sistema deve conter níveis de acesso, o nível cidadão-colaborador e o nível para gestão. Em cada um dos níveis serão apresentadas opções disponíveis para cada perfil;  | MÉDIA |

## Restrições

O projeto está restrito pelos itens apresentados na tabela a seguir.

|ID| Restrição                                             |
|--|-------------------------------------------------------|
|01| O projeto deverá ser entregue até o final do semestre |

Enumere as restrições à sua solução. Lembre-se de que as restrições geralmente limitam a solução candidata.

> **Links Úteis**:
> - [O que são Requisitos Funcionais e Requisitos Não Funcionais?](https://codificar.com.br/requisitos-funcionais-nao-funcionais/)
> - [O que são requisitos funcionais e requisitos não funcionais?](https://analisederequisitos.com.br/requisitos-funcionais-e-requisitos-nao-funcionais-o-que-sao/)

# Catálogo de Serviços

Descreva aqui todos os serviços que serão disponibilizados pelo seu projeto, detalhando suas características e funcionalidades.

# Arquitetura da Solução

Definição de como o software é estruturado em termos dos componentes que fazem parte da solução e do ambiente de hospedagem da aplicação.

![arq](https://github.com/user-attachments/assets/b9402e05-8445-47c3-9d47-f11696e38a3d)


## Tecnologias Utilizadas

Descreva aqui qual(is) tecnologias você vai usar para resolver o seu problema, ou seja, implementar a sua solução. Liste todas as tecnologias envolvidas, linguagens a serem utilizadas, serviços web, frameworks, bibliotecas, IDEs de desenvolvimento, e ferramentas.

Apresente também uma figura explicando como as tecnologias estão relacionadas ou como uma interação do usuário com o sistema vai ser conduzida, por onde ela passa até retornar uma resposta ao usuário.

## Hospedagem

Explique como a hospedagem e o lançamento da plataforma foi feita.

> **Links Úteis**:
>
> - [Website com GitHub Pages](https://pages.github.com/)
> - [Programação colaborativa com Repl.it](https://repl.it/)
> - [Getting Started with Heroku](https://devcenter.heroku.com/start)
> - [Publicando Seu Site No Heroku](http://pythonclub.com.br/publicando-seu-hello-world-no-heroku.html)
