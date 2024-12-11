
# Projeto Disciplina: Requisitos de Software

Olá! Este repositório faz parte do projeto da disciplina de Requisitos de Software da UTFPR - Campus Cornélio Procópio. 

Link do Padlet: https://padlet.com/antonioferreira34/homebase-j86p0zccjk78nrvl

## 1. Introdução

***1.1.  Nome do Grupo***

Nome do grupo: HomeBase

Integrantes:

- Antonio Carlos Ferreira
- Gustavo Pukanski Schatzmann
- John Takeo Da Silva Uehara
- Luis Fernando Rodrigues De Oliveira
- Luiz Fernando Morerira Domenico

***1.2.  Nome do Sistema***

Nome do software: HomeBase

***1.3.  Propósito do Sistema***

Este documento apresenta os requisitos dos usuários a serem desenvolvidos pela HomeBase, fornecendo aos desenvolvedores as informações necessárias para o projeto e implementação, assim como para a realização dos testes e homologação do sistema.

O objetivo do sistema HomeBase é ser um sistema que auxilia empresas no cadastro e gestão de alojamentoss, acompanhamento de relatórios e estatísticas, notificações e alertas, interface de usuário amigável e acessível, reservas e alocação de acomodações e controle de faturas e custos.
Alguns dos benefícios que o sistema possui é a melhoria na gestão de recursos, eficiência e agilidade, relatórios e análises de dados.
Alguns dos problemas que o sistema visará auxiliar em resolver são desperdício de recursos e custos excessivos e gerenciamento ineficiente de alocação.
O comportamento geral do sistema é Maximizar a utilização dos alojamentos disponíveis, garantindo que as unidades não fiquem ociosas e sejam usadas de maneira eficiente, calcular os custos associados às estadias, gerar faturas e manter registros financeiros atualizados e Fornecer relatórios detalhados sobre ocupação, custos, e uso de alojamento, oferecendo uma visão clara para os gestores da empresa.


***1.2.  Público Alvo***

Este projeto é destinado a empresas que necessitam lidar com o gerenciamento de vários funcionários que deverão estar alojados em um local para exercer o trabalho temporariamente.

***1.3. Descrição dos usuários***

***Personas:***

Persona 1: 

![persona1](https://github.com/user-attachments/assets/c431028a-34d6-4c76-a1e7-dcc6b81a5919)

Persona 2: 

![persona2](https://github.com/user-attachments/assets/e48c0e3e-3c07-45dc-976b-8d21cb7f5a8f)



***Análise da situação atual: antes da introdução de sua solução***

*`1. O que as pessoas fazem?`*
    O locador realiza o controle, gerenciamento de recursos, serviços e se comunica com locatário em diferentes plataformas, não integradas entre si. 
    O locatário busca informações de forma online ou presencial, realiza reserva por telefone ou e-mail, reporta o problema diretamente com o locador.
      
*`2. Quais os artefatos envolvidos?`*
    Sem o uso do sistema proposto, alguns dos artefatos utilizados são formulários em papel, planilhas no excel, plano de negócio, e outros softwares voltados à funções específicas como     contabilidade e controle de gasto.
    
*`3. O que elas precisam saber?`*
    O locador precisa ter conhecimento do tempo de estadia do locatário, os recursos que serão necessários, quantas pessoas usufruirão o imóvel.
    O locatário precisa saber o local do imóvel, sua disponiibilidade, o valor que será cobrado pelo uso.

***Análise das tarefas depois: como serão executadas as suas tarefas com sua solução:***

*`1. O que as pessoas fazem?`*
    O locador informará os dados no HomeBase acerca dos funcionários, alojados, alojamentos, recursos e empresas parceiras.
    O locador, dessa forma, poderá, facilmente, visualizar os dados registrados, assim, podendo gerenciar efetivamento os alojamentos.
    
*`2. Quais os artefatos envolvidos?`*
    Alguns dos artefatos que fazem parte do contexto de desenvolvimento do sistema são o diagrama de caso de uso, Especificação de Requisitos de Software (SRS), histórias dos usuários,     diagrama de atividades e diagrama de classes.
    
*`3. O que elas precisam saber?`*
    O locador deverá ter conhecimento de ferramentas importantes da aplicação, como adicionar um número de funcionários, determinar os recursos que serão utilizados e suas quantidades,      informar dados do local, como disponibilidade, tamanho, localização, e registrar os valores envolvidos para o controle de gasto e receita; também é importante ter noção de como          realizar consultas, por meio de mecanismos de filtros, a fim de encontrar inconsistências e/ou erros, a fim de correção. 
    
***Cenário: Antes***

O locador mantém o registro ou de maneira manual ou utilizando ferramentas como Excel, google planinhas, e utiliza as mesmas ferramentas para a consulta e verificação dos dados.

***Cenário: Depois***

O locador utilizará o sistema HomeBase para realizar a inserção, alteração, verificação de dados acerca dos funcionários, dos recursos, dos alojamentos, dos alojados e do controle financeiro de maneira mais organizada.

## 2. Documentos gerais no repositório

***2.1. Requisitos Funcionais***

| Identificador | Descrição |Depende de|
|--	|--|--|
| RF01 |O software deve ter filtros de busca, nome, data, status do locatário e localização, para melhorar a eficiência da pesquisa. | |
| RF02 |O software deve oferecer uma opção de múltiplos critérios de busca, permitindo combinações de usuários. | |
| RF03 |O sistema deve permitir a criação de perfis diferentes para os diversos administradores do alojamento |RNF01 |
| RF04 |O software deve gerar automaticamente um relatório diário, informando o fluxo de alojados e quantidade de produtos que será necessário para serviços adicionais. Este relatório deve ser enviado para o email especificado pelo usuário.|RNF05 |
| RF05 |O software deve permitir a inserção de dados, como nome, CPF, RG e telefone do locatário.|RNF01, RNF09, RNF10 |
| RF06 |O software deve permitir que a empresa consulte os dados do locatário, com critérios de busca definidos, como nome, CPF ou número de contrato. O acesso a esses dados deve ser restrito a usuários autorizados, com controle de permissões e registro de auditoria para garantir a segurança e a privacidade das informações. |RNF01, RNF09, RNF10 |
| RF07 |O software deve permitir que o alojado envie um feedback sobre o alojamento por meio de um formulário de avaliação, que inclua campos como notas de satisfação e comentários. O feedback será armazenado em banco de dados seguro e acessível apenas para usuários autorizados, como a administração do sistema, e será associado ao respectivo alojamento para facilitar o acompanhamento.|RNF01, RNF09, RNF10 |
| RF08 |O software deve enviar notificações ao usuário sempre que houver uma atualização relevante para ele, como mudanças no status da reserva ou modificações nas condições do contrato. As notificações serão enviadas por e-mail e/ou aplicativo, conforme a preferência do usuário, e devem ser configuráveis pelo próprio usuário nas configurações da conta. |RNF07 |
| RF09 |O software deve permitir a comunicação direta entre o proprietário e o locatário por meio de um sistema de mensagens interno. O proprietário poderá iniciar a comunicação com o locatário a partir da visualização de seu contrato ou perfil, e o locatário poderá responder a mensagens relacionadas ao seu alojamento. O sistema deve garantir que todas as mensagens sejam registradas para fins de auditoria, sendo acessíveis apenas por ambas as partes envolvidas, salvo em situações excepcionais que requeiram mediação. |RNF01, RNF07, RNF10 |
| RF10 |O software deve realizar verificações automáticas para detectar e bloquear ataques comuns, como SQL Injection, Cross-Site Scripting (XSS) e Cross-Site Request Forgery (CSRF). | |

***2.2. Requisitos Não Funcionais***

| Identificador  |Descrição |Prioridade|
|--	|--|--|
| RNF01 | O sistema deve estar disponível 24 horas por dia. | Alta | |
| RNF02	| O sistema deve ser acessível em múltiplas plataformas (Windows, iOS, Android) sem perda de funcionalidades. | Alta |
| RNF03 | O sistema deve responder a qualquer ação do usuário em até 2 segundos, garantindo uma experiência fluida | Alta |
| RNF04 | A interface deve ser simples e intuitiva, permitindo que o dono do alojamento faça cadastros e acompanhe reservas sem necessidade de treinamento técnico. O tempo de treinamento necessário para o dono do alojamento e sua equipe aprenderem a usar o sistema deve ser inferior a 4 horas. | Alta |
| RNF05 | O sistema deve realizar backups automáticos diários para garantir a recuperação de dados em caso de falha ou perda | Alta |
| RNF06 | O sistema deve permitir atualizações periódicas e manutenção sem interrupção significativa das atividades, com um tempo de inatividade máximo de 2 horas. | Alta |
| RNF07 | O sistema deve oferecer suporte para múltiplos idiomas (Português, Inglês e Espanhol). | Baixa |
| RNF08 | Se o sistema for instalado localmente, ele deve ter um consumo de energia eficiente, minimizando o uso de recursos do hardware. | Média |
| RNF09 | O software deve seguir as regulamentações de proteção de dados, como a LGPD, para garantir a privacidade dos moradores e do proprietário | Alta |
| RNF10 | O software deve usar criptografia de ponta a ponta (end-to-end encryption) para garantir que os dados sensíveis não sejam acessíveis por partes não autorizadas, tanto em trânsito quanto em repouso. | Alta |

***2.3. Perguntas***

 1) Como os alojamentos são realizados atualmente sem um sistem para utilizar?
 2) Há planos visando a expansão das operações?
 3) Quão rápido ou ágil é a inserção de novos clientes alojados?
 4) Quais funcionalidades o sistema teria que o ajudaria?
 5) Como tais funcionalidades o ajudarão na prática?
 6) Qual a maior dificuldade no gerenciamento de recursos(móveis e entrega de alimentação)?
 7) Quanto tempo em média é gasto na atualização dos relatórios acerca dos alojados e dos recursos necessários?
 8) Como surgem as oportunidades de negócio?
 9) Como é a relação com os alojados?
 10) Como a inconsistência de informações é impedida?

***2.4. Entrevista***

link da entrevista: https://drive.google.com/file/d/1ci5w6SYvhhyhM8anPmDX3EpIFLMlYFH5/view?usp=drive_link

***2.5. Histórias do Usuário***

**US001**  
- **Como** um usuário dono da empresa principal,  
- **Eu** quero me cadastrar no sistema,  
- **Para** gerenciar os dados acerca dos recursos alocados, quais funcionários estarão alojados, o tempo de estadia e o custo da operação.

**US002**  
- **Como** um usuário dono da empresa principal,  
- **Eu** quero registrar e atualizar informações de acordo com o feedback recebido dos funcionários e da empresa parceira,  
- **Para** garantir que o sistema reflita as necessidades e opiniões de todas as partes envolvidas.

**US003**  
- **Como** um usuário dono da empresa principal,  
- **Eu** quero visualizar relatórios detalhados sobre ocupação e custos,  
- **Para** monitorar o desempenho financeiro e operacional do meu negócio.

**US004**  
- **Como** um usuário dono da empresa principal,  
- **Eu** quero configurar notificações automáticas sobre a necessidade de recursos,  
- **Para** otimizar os processos de logística e evitar desperdícios.

**US005**  
- **Como** um usuário dono da empresa principal,  
- **Eu** quero rastrear em tempo real quais recursos estão sendo mais utilizados,  
- **Para** ajustar a oferta e reduzir custos.

**US006**  
- **Como** um funcionário alojado,  
- **Eu** quero poder registrar solicitações, como manutenção ou troca de quarto,  
- **Para** garantir melhores condições durante minha estadia.

**US007**  
- **Como** um funcionário alojado,  
- **Eu** quero acessar informações detalhadas sobre serviços adicionais disponíveis,  
- **Para** planejar e usufruir melhor dos recursos durante minha estadia.

**US008**  
- **Como** uma empresa parceira,  
- **Eu** quero consultar o histórico de feedbacks enviados pelos meus funcionários,  
- **Para** identificar áreas de melhoria na relação com o alojamento.

**US009**  
- **Como** uma empresa parceira,  
- **Eu** quero cadastrar informações sobre turnos e horários de trabalho dos meus funcionários,  
- **Para** facilitar a organização e compatibilidade com o alojamento.

**US010**  
- **Como** uma empresa parceira,  
- **Eu** quero acessar relatórios consolidados sobre as estadias dos meus funcionários,  
- **Para** justificar despesas e apresentar dados à diretoria.



***2.6. Diagramas de Caso de Uso e Especificações***

*<Imagem, arquivo (PDF), link com Diagrama de Caso de Uso.>*

***2.7. Diagramas de Atividades***

*<Imagem, arquivo (PDF), link com Diagrama de Atividades.>*

***2.8. Matrizes de Rastreabilidade***

*<Imagem, arquivo (PDF), link com Matriz de Rastreabilidade.>*

***2.9. Protótipos***

*<Imagem, arquivo (PDF), link com Protótipo.>*

## Referências

*<Esta seção é destinada à descrição das referências utilizadas pelo documento, como por exemplo, URLs e livros. Ver exemplo a seguir:>*

[1] “Glossário da _USina_”, <_id_doc glossário_>, Versão <_versão_>. Localização: <_localização_>.
