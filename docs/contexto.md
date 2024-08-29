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

## Personas

### 1. Ana Luiza
   
Idade: 34 anos

Ocupação: Professora de escola primária

Tecnologia: Usuária ativa de smartphones e redes sociais

Objetivos: Quer um sistema eficiente e acessível para relatar problemas na comunidade, como iluminação pública e buracos nas ruas. Valoriza transparência e respostas rápidas.

Desafios: Dificuldades para acompanhar o progresso das solicitações devido à falta de informações claras.

Uso do Sistema: Utiliza o aplicativo móvel e o portal online para registrar e rastrear solicitações, frequentemente anexa fotos e descreve problemas detalhadamente.

### 2. Carlos Daniel
   
Idade: 45 anos

Ocupação: Coordenador de Atendimento ao Cidadão

Tecnologia: Familiarizado com softwares administrativos e sistemas integrados

Objetivos: Melhorar a eficiência no gerenciamento das solicitações e garantir que todas as demandas sejam atendidas adequadamente.

Desafios: Gerenciar grandes volumes de solicitações e garantir encaminhamento correto para os departamentos.

Uso do Sistema: Utiliza o painel administrativo para monitorar, categorizar e distribuir as solicitações. Analisa relatórios para identificar áreas que precisam de mais atenção.

### 3. Maria

Idade: 62 anos

Ocupação: Aposentada

Tecnologia: Usa um celular básico e e-mail ocasionalmente

Objetivos: Deseja um meio simples para registrar problemas como manutenção de parques ou coleta de lixo.

Desafios: Dificuldades com tecnologia e prefere métodos de comunicação mais tradicionais.

Uso do Sistema: Faz solicitações via telefone ou e-mail e recebe atualizações por SMS ou e-mail.

### 4. João Luiz
   
Idade: 50 anos

Ocupação: Chefe do Departamento de Infraestrutura

Tecnologia: Profissional experiente com conhecimentos em gestão de projetos e tecnologia

Objetivos: Utilizar dados das solicitações para planejar e priorizar projetos de infraestrutura, como reparos de estradas e construção de novas instalações.

Desafios: Necessita de informações precisas e integradas para decisões eficazes e alocação de recursos.

Uso do Sistema: Acessa relatórios detalhados e análises de tendências para otimizar a alocação de recursos e planejamento de projetos.

### 5. Laura Luiza

Idade: 38 anos

Ocupação: Coordenadora de Programas de Saúde

Tecnologia: Usada a sistemas integrados e gestão de dados

Objetivos: Integrar solicitações relacionadas à saúde pública com outros sistemas municipais e coordenar a resposta a questões como vacinação e controle de surtos.

Desafios: Coordenar com vários departamentos e garantir eficiência na integração de dados.

Uso do Sistema: Trabalha com a integração do sistema de solicitações com outros sistemas municipais, monitora o progresso e responde a solicitações específicas.

### 6. Pedro Augusto
    
Idade: 42 anos

Ocupação: Proprietário de uma pequena loja de roupas

Tecnologia: Usa um computador e smartphone para gerenciar negócios e comunicação

Objetivos: Quer um sistema eficiente para relatar problemas que afetam seu comércio, como questões de segurança pública ou manutenção urbana, e receber atualizações sobre o status das solicitações.

Desafios: Problemas urbanos que impactam diretamente seu negócio e a necessidade de respostas rápidas para minimizar impactos financeiros.

Uso do Sistema: Utiliza o portal online e o aplicativo móvel para registrar e acompanhar solicitações relacionadas ao seu comércio. Valoriza a capacidade de fornecer feedback e avaliar a resolução dos problemas.

## História de Usuário

Persona Pedro, um empresário local que enfrenta problemas urbanos que afetam seu comércio, quer um sistema eficiente para relatar esses problemas e acompanhar a resolução, para que possa minimizar os impactos negativos em seu negócio e manter a satisfação dos seus clientes.

Contexto: Pedro, proprietário de uma pequena loja de roupas, percebeu que a calçada em frente ao seu estabelecimento está danificada, dificultando o acesso dos clientes e afetando suas vendas. Ele precisa que a prefeitura conserte a calçada o mais rápido possível.

Passos:

Acesso ao Sistema: Pedro abre o aplicativo móvel da prefeitura em seu smartphone, que é mais conveniente para ele durante o horário de trabalho.

Registro da Solicitação: No aplicativo, Pedro seleciona a opção para registrar uma nova solicitação. Ele descreve o problema da calçada danificada, tira e anexa fotos da área afetada, e usa o mapa interativo para marcar a localização exata da sua loja.

Recebimento do Protocolo: Após enviar a solicitação, Pedro recebe imediatamente um número de protocolo via SMS e e-mail, confirmando que sua solicitação foi registrada com sucesso.

Acompanhamento em Tempo Real: Pedro acompanha o status da solicitação através do aplicativo, recebendo atualizações automáticas sobre o progresso. Ele vê confirmações de que a solicitação foi recebida, está em análise e, finalmente, que o trabalho está em andamento.

Feedback e Avaliação: Após a conclusão do serviço e o conserto da calçada, Pedro recebe uma notificação informando que o problema foi resolvido. Ele é convidado a avaliar o serviço e fornecer feedback sobre sua experiência.

Benefícios:

Transparência: Pedro tem visibilidade completa sobre o status da sua solicitação, aumentando sua confiança na eficiência da prefeitura.
Eficiência: O processo ágil de registro e acompanhamento reduz o tempo de resposta e ajuda a resolver o problema de maneira eficaz.
Satisfação: Pedro sente-se valorizado e satisfeito com o atendimento, sabendo que sua solicitação foi tratada de forma rápida e eficaz.


# Especificações do Projeto

## Requisitos

As tabelas que se seguem apresentam os requisitos funcionais e não funcionais que detalham o escopo do projeto. Para determinar a prioridade de requisitos, aplicar uma técnica de priorização de requisitos e detalhar como a técnica foi aplicada.

### Requisitos Funcionais

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|----|
|RF-01| Permitir inclusão, edição, exclusão e consulta dos dados das solicitações, usuários, finalidades, unidades, setores e bairros; | ALTA | 
|RF-02| Enviar e-mail para os usuários quando for incluída uma nova requisição;   | ALTA |
|RF-03| Enviar sms para os usuários quando for incluída uma nova requisição;  | MÉDIA |
|RF-04| O sistema deve permitir o cadastro de cidadãos, solicitando informações básicas como nome, CPF, endereço, e-mail, e telefone; | ALTA |
|RF-05| O sistema deve permitir que os cidadãos se autentiquem usando um login e senha;  | ALTA |
|RF-06| Permitir que sejam enviados feedbacks referentes às solicitações;  | MÉDIA |
|RF-07| Emitir Relatórios, incluindo estatísticas como tipo de requisição, tempo médio de resposta;  | MÉDIA |
|RF-08| O cidadão deve poder enviar novas requisições diretamente pelo sistema, podendo categorizar o tipo de requisição (sugestões, reclamações, denúncias, etc.).  | ALTA |


### Requisitos não Funcionais

|ID     | Descrição do Requisito  |Prioridade |
|-------|-------------------------|----|
|RNF-01| Possuir autenticação por login e senha | ALTA | 
|RNF-02| O sistema deve ser intuitivo e fácil de usar, garantindo uma boa experiência para usuários com diferentes níveis de familiaridade com tecnologia;   | ALTA |
|RNF-03| Deve possuir uma interface responsiva que funcione bem em dispositivos móveis e desktops;   | ALTA |
|RNF-04| O sistema deve garantir a proteção dos dados dos cidadãos, implementando criptografia para dados sensíveis como senhas;   | ALTA |
|RNF-05| O sistema deve conter níveis de acesso, o nível cidadão-colaborador e o nível para gestão. Em cada um dos níveis serão apresentadas opções disponíveis para cada perfil;  | MÉDIA |
|RNF-06| O sistema deve ser compatível com os principais navegadores web (Chrome, Firefox, Safari, Edge) e funcionar em diferentes sistemas operacionais;  | MÉDIA |

## Restrições

O projeto está restrito pelos itens apresentados na tabela a seguir.

|ID| Restrição                                             |
|--|-------------------------------------------------------|
|RES-01| O projeto deverá ser entregue até o final do semestre |
|RES-02| Utilização de tecnologias gratuitas ou de parceria com a PUC |
|RES-03| Falta de capital monetário para o desenvolvimento do projeto |


## Catálogo de Serviços

### **1. Cadastro e Gerenciamento de Requisições**

**Descrição:** Permite aos usuários registrar novas requisições, visualizar e editar requisições existentes, bem como excluí-las quando necessário.

**Funcionalidades:**

**•	Cadastro de Requisições:** Usuários podem registrar novas solicitações de serviços ou reclamações.

**•	Visualização de Requisições:** Usuários podem consultar o status e os detalhes das requisições feitas.

**•	Edição de Requisições:** Permite atualizar as informações das requisições existentes.

**•	Exclusão de Requisições:** Usuários podem remover requisições, caso necessário.

**•	Filtragem e Pesquisa:** Opções para buscar requisições por data, tipo, status e outros critérios.

**Público-Alvo:** Cidadãos, Gestores Públicos, Servidores Públicos Operacionais

### **2. Notificações por E-mail e SMS**

**Descrição:** Envia notificações automatizadas para os usuários sobre o status das suas requisições.

**Funcionalidades:**

**•	Notificação por E-mail:** Envio de e-mails quando novas requisições são registradas ou atualizadas.

**•	Notificação por SMS:** Envio de mensagens SMS para manter os usuários informados sobre o progresso de suas requisições 

**•	Público-Alvo: Cidadãos**

### **3. Feedback das Solicitações**

**Descrição:** Permite que os cidadãos enviem feedbacks sobre o atendimento recebido e a resolução das suas requisições.

**Funcionalidades:**

**•	Envio de Feedback:** Opção para enviar comentários e avaliações sobre o serviço prestado.

**•	Visualização de Feedbacks:** Os gestores podem visualizar e analisar os feedbacks recebidos para melhoria contínua.

**Público-Alvo:** Cidadãos, Gestores Públicos

### **4. Geração de Relatórios**

**Descrição:** Criação de relatórios detalhados sobre as requisições, feedbacks e outras métricas relevantes para análise e tomada de decisão.

**Funcionalidades:**

**•	Relatórios Personalizados:** Geração de relatórios com filtros específicos (por data, tipo de requisição, setor responsável, etc.).

**•	Exportação de Relatórios:** Opção para exportar relatórios em formatos como PDF, Excel, etc.

**Público-Alvo:** Gestores Públicos, Supervisores

### **5. Autenticação e Controle de Acesso**

**Descrição:** Sistema de autenticação para acesso ao sistema e controle de acesso baseado em perfis.

**Funcionalidades:**

**•	Login e Senha:** Requer autenticação por login e senha para acesso ao sistema.

**•	Controle de Acesso:** Definição de níveis de acesso (cidadão-colaborador e gestão) e restrição de funcionalidades com base no perfil do usuário.

**Público-Alvo:** Todos os usuários

### **6. Interface Amigável e Navegação**

**Descrição:** Interface do usuário que facilita a navegação e a interação com o sistema.

**Funcionalidades:**

**•	Design Intuitivo:** Utilização de ícones e cores que tornam a navegação mais intuitiva.

**•	Botões de Redirecionamento:** Facilita o acesso às principais funcionalidades do sistema.

**Público-Alvo:** Todos os usuários

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
