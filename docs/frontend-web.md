# Front-end Web
O front-end da aplicação foi desenvolvido para oferecer uma interface de fácil acesso e visualmente atraente, permitindo que cidadãos enviem solicitações, reclamações e sugestões de forma organizada. Projetado como uma ponte eficiente entre a população e a administração pública, ele facilita o engajamento cidadão e o rápido atendimento das demandas, promovendo uma comunicação direta e funcional

## Tecnologias Utilizadas
 * Para o desenvolvimento do front-end da aplicação, foram utilizadas as seguintes tecnologias:

 * Blade (Laravel): Motor de templates nativo do Laravel, utilizado para construir as interfaces de usuário de forma integrada com o back-end. O Blade permite a criação de layouts dinâmicos e reutilizáveis com sintaxe intuitiva, facilitando a manipulação de dados do backend e o controle de fluxo diretamente nas views.

 * Componentes Blade: Aproveitando o sistema de componentes do Blade, a interface é modularizada, melhorando a organização do código e a reutilização de elementos da interface, como botões, formulários e layouts, reduzindo redundâncias e mantendo a consistência visual.

 * Bootstrap: Framework CSS utilizado para criar uma base responsiva e moderna. Com suas classes predefinidas e grid flexível, o Bootstrap facilita a adaptação da interface para diferentes tamanhos de tela, oferecendo uma aparência visualmente agradável e compatível com diversos dispositivos.

 * Tabler Icons: Biblioteca de ícones utilizada para enriquecer a interface visual da aplicação. Com uma ampla gama de ícones disponíveis e um design moderno e minimalista, o Tabler Icons melhora a usabilidade, ajudando os usuários a identificar funções e ações no sistema de maneira rápida e intuitiva.

 * JavaScript: JavaScript puro foi utilizado para adicionar interatividade leve ao front-end e manipulação do DOM, onde necessário, facilitando uma navegação mais dinâmica e responsiva sem necessidade de recarregamento da página.

## Arquitetura

[Descrição da arquitetura das aplicação web, incluindo os componentes e suas interações.]

## Modelagem da Aplicação
* Início
![image](https://raw.githubusercontent.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-2-pe6-t3-g15-atende/refs/heads/main/docs/img/inicio%20.png)
* Register
![image](https://raw.githubusercontent.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-2-pe6-t3-g15-atende/refs/heads/main/docs/img/register.png)
* Login
![image](https://raw.githubusercontent.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-2-pe6-t3-g15-atende/refs/heads/main/docs/img/login.png)
* Dashboard
![image](https://raw.githubusercontent.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-2-pe6-t3-g15-atende/refs/heads/main/docs/img/dashboard.png)
* Solicitações Recentes
![image](https://raw.githubusercontent.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-2-pe6-t3-g15-atende/refs/heads/main/docs/img/solicitacoesrecentes.png)
* Nova Solicitação
![image](https://raw.githubusercontent.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-2-pe6-t3-g15-atende/refs/heads/main/docs/img/nova%20solicitacao.png)
* Visualizar Solicitação
![image](https://raw.githubusercontent.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-2-pe6-t3-g15-atende/refs/heads/main/docs/img/ver%20solicitacao.png)
* Editar Solicitação
![image](https://raw.githubusercontent.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-2-pe6-t3-g15-atende/refs/heads/main/docs/img/editar%20solicitacao.png)
* Perfil
![image](https://raw.githubusercontent.com/ICEI-PUC-Minas-PMV-SI/pmv-si-2024-2-pe6-t3-g15-atende/refs/heads/main/docs/img/perfil.png)

## Projeto da Interface Web
[Descreva o projeto da interface Web da aplicação, incluindo o design visual, layout das páginas, interações do usuário e outros aspectos relevantes.]

### Wireframes
* Tela de Login: Campos de "Usuário" e "Senha" com uma opção para manter-se conectado e um link para recuperação de senha, facilitando o acesso para usuários que retornam.

* Tela Inicial (Página Informativa): Explica os objetivos do sistema, destacando o propósito de facilitar a comunicação entre cidadãos e a gestão pública. Apresenta botões de "Entrar" e "Criar Cadastro" para fácil navegação.

* Tela de Registro: Formulário detalhado para registro de novos usuários, incluindo campos obrigatórios como nome, CPF/CNPJ, e-mail, senha, confirmação de senha, estado, cidade, CEP e endereço. Isso permite que a plataforma colete as informações necessárias para a identificação e o contato dos usuários.

* Dashboard: Página principal para usuários logados, com gráficos e tabelas de solicitações. Inclui seções de "Solicitações Recentes" e "Resumo de Gastos", organizando as informações de forma visual para fácil acompanhamento.

* Tela de Perfil de Usuário: Permite ao usuário verificar e editar suas informações básicas, como nome e e-mail. Também exibe a opção de salvar as alterações para atualizar as informações no sistema.

* Tela de Alteração de Senha: Disponível na seção de perfil, permite ao usuário atualizar a senha. O formulário exige a senha atual, a nova senha e a confirmação da nova senha, garantindo segurança na atualização.

* Nova Solicitação: Formulário que permite a criação de uma nova solicitação pública, com campos para endereço, descrição, categoria, e upload de imagem opcional. Botões para "Voltar" e "Criar Solicitação" facilitam a navegação.

* Visualizar e Editar Solicitação: Exibe todos os detalhes de uma solicitação, com a opção de editar campos específicos. Essa funcionalidade permite que o administrador ou responsável mantenha o status atualizado conforme a solicitação avança.

* Detalhes da Solicitação: Página que mostra informações completas sobre uma solicitação específica, incluindo endereço, descrição, categoria, status, data de cadastro e última atualização. A imagem associada à solicitação também é exibida.

### Design Visual
O design da aplicação é moderno e amigável, com uma paleta de cores que transmite profissionalismo e confiabilidade.

* Cores: Tons de azul são usados para elementos de ação (botões de confirmação e destaque), enquanto tons neutros de cinza e branco predominam no fundo, trazendo leveza à interface.

* Tipografia: Fontes simples e claras garantem uma leitura confortável. Os títulos são destacados em negrito para melhor hierarquia visual.

* Ícones e Elementos Gráficos: Ícones ajudam a identificar rapidamente as funções de cada botão, como os botões "Salvar", "Voltar" e "Editar". Gráficos de barra e de círculo representam dados de solicitações e gastos no dashboard.

### Layout Responsivo
Desenvolvemos a interface para ser completamente responsiva, capaz de se adaptar a diversos tamanhos de tela, como desktops, tablets e smartphones. Os layouts e os componentes se ajustam automaticamente, assegurando que elementos como botões, campos de texto e menus estejam sempre visíveis e bem distribuídos, promovendo uma experiência de uso fluida e consistente em qualquer dispositivo..

### Interações do Usuário
* Feedback Visual: Ao interagir com campos de formulário, botões ou ícones, há um feedback visual (mudança de cor ou borda) para indicar a área selecionada.

* Transições Suaves: As páginas mudam suavemente, mantendo a experiência agradável ao usuário ao navegar entre seções, como de "Login" para o "Dashboard".

* Mensagens de Erro e Sucesso: Ao realizar ações como atualização de senha ou envio de uma nova solicitação, o usuário recebe mensagens de feedback indicando sucesso ou erros no preenchimento.

* Notificações: Ícones de notificação informam o usuário sobre atualizações e mudanças importantes nas solicitações, melhorando a usabilidade e a experiência de engajamento.

## Fluxo de Dados

O fluxo de dados está estruturado para garantir a eficiência e segurança na troca de informações entre usuários e o sistema. O fluxo segue as seguintes etapas:

1- Registro: Usuários inserem informações pessoais como CPF/CNPJ e dados de endereço. O sistema valida as informações e armazena no banco de dados para futura identificação.

2- Autenticação: Os usuários podem acessar a plataforma com as credenciais criadas. A autenticação garante que apenas usuários cadastrados possam acessar as funções de criação e gestão de solicitações.

3-Criação de Solicitações: Após o login, os usuários podem criar novas solicitações preenchendo o formulário e anexando imagens, se desejado. O sistema armazena a solicitação e exibe no painel do usuário.

4- Atualização de Perfil e Senha: Na área de perfil, os usuários podem atualizar suas informações de contato ou redefinir a senha. A alteração de senha exige a confirmação da senha atual para maior segurança.

5- Consulta e Edição de Solicitações: Usuários e administradores podem visualizar, editar e atualizar o status das solicitações, mantendo o acompanhamento atualizado.

6- Visualização de Resumo e Análise de Dados: No dashboard, gráficos e tabelas mostram resumos das solicitações e dos gastos associados. Isso permite uma análise visual rápida do volume de solicitações e da evolução dos gastos, auxiliando na tomada de decisões.

## Requisitos Funcionais

|ID    | Descrição do Requisito  |     |
|------|-----------------------------------------|----|
|RF-01| Usuários devem ser capazes de se registrar com informações pessoais (nome, CPF/CNPJ, endereço, e-mail, senha). | 
|RF-02| Implementar login com autenticação por e-mail e senha. | 
|RF-03| Permitir recuperação de senha para usuários que a esqueceram. |
|RF-03| Usuários podem criar novas solicitações, inserindo detalhes como endereço, descrição, categoria e imagem opcional. |
|RF-04| Exibir uma lista de solicitações recentes, com filtros por status e data.. |

## Requisitos Não Funcionais

|ID    | Descrição do Requisito  |     |
|------|-----------------------------------------|----|
|RF-01| A aplicação deve carregar as principais páginas (login, dashboard, lista de solicitações) em menos de 5 segundos em redes de internet comuns. | 
|RF-02| Implementar criptografia para senhas de usuários e dados sensíveis.|
|RF-03| Utilizar autenticação baseada em token para proteger sessões de usuário.|
|RF-04| A interface deve ser intuitiva e acessível, com design responsivo para diferentes dispositivos, incluindo desktops, tablets e smartphones.|
|RF-05| Garantir que todos os elementos da interface estejam claramente identificados e fáceis de usar para diferentes tipos de usuário.|


## Considerações de Segurança

* Cross-Site Request Forgery (CSRF): Implementação de tokens CSRF para prevenir requisições não autorizadas.
* Criptografia: Dados sensíveis, como senhas, devem ser criptografados antes do armazenamento.
* Controle de acesso para diferentes papéis de usuário (usuário comum e administrador) para proteger ações específicas.

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
