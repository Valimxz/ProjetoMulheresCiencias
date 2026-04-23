<img src='/img/logo.png' alt='logo da empresa' width='50px' heidth='50px'/>

# *FIBONACCI MANAGEMENT SYSTEM*

# PROJETO DE SOFTWARE

## *Stakeholders*
|NOME|E-MAIL|
|:---|:---|
|José Augusto de Araujo Faria|jose.araujo@estudante.ifro.edu.br|
|Pedro Henrique Valim de Oliveira|henrique.valim@estudante.ifro.edu.br|
|Gustavo da Silva Moreira Xavier |xavier.gustavo@estudante.ifro.edu.br|
|Luiz Claudio Felipe Oliveira Bernardino dos Santos|santos.luiz@estudante.ifro.edu.br|
|Kauã Fhelipe Andrade Calgarotto|andrade.f@estudante.ifro.edu.br|


# Sumário

* [RESUMO DO PROJETO](#resumo-do-projeto)
* [INTRODUÇÃO](#introdução)
  * [PROPÓSITO DESTE DOCUMENTO](#propósito-deste-documento)
* [DESCRIÇÃO GERAL](#descrição-geral)
  * [USUÁRIOS DO SISTEMA](#usuários-do-sistema)
  * [ABRANGÊNCIA E SISTEMAS SIMILARES](#abrangência-e-sistemas-similares)
  * [SUPOSIÇÕES E DEPENDÊNCIAS](#suposições-e-dependências)
* [REQUISITOS DO SOFTWARE](#requisitos-do-software)
  * [REQUISITOS FUNCIONAIS](#requisitos-funcionais)
  * [REQUISITOS NÃO FUNCIONAIS](#requisitos-não-funcionais)
* [PROTOTIPAGEM](#prototipagem)
* [DIAGRAMA DE CLASSES](#diagrama-de-classes)
* [REFERÊNCIAS](#referências)

# RESUMO DO PROJETO
| ITEM | DESCRIÇÃO|
|:---|:---|
| NOME DO PROJETO | HubSmart |
| PRINCIPAL OBJETIVO | Ter o mesmo o mesmo conceito de como se fosse um shopping, fazer tudo em só lugar, o usuário após entrar ao site, terá acesso a uma assistente IA, previsão do tempo e um gerenciador de tarefas. |
| BENEFÍCIOS ESPERADOS | -Centralização de serviços em um único ambiente digital, trazendo mais praticidade-Melhoria na organização e produtividade com o gerenciador de tarefas,Experiência personalizada por meio da assistente IA com histórico de interações,Maior segurança e autonomia com sistema completo de login, cadastro e recuperação de senha.
| INÍCIO E TÉRMINO PREVISTOS | 01/02/2026 - 07/06/2026 |

[ [INÍCIO](#fibonacci-management-system) ]

# INTRODUÇÃO

## PROPÓSITO DESTE DOCUMENTO

Este documento destina-se aos clientes, engenheiros, gerentes e demais stakeholders deste projeto. O propósito deste documento é apresentar a descrição dos serviços e funções que o sistema **_Fibonacci Management System_** deve prover, bem como as suas restrições de operação e propriedades gerais, a fim de ilustrar uma descrição detalhada do sistema para um auxílio durante as etapas de análise, projeto e testes. O documento especifica todos os requisitos funcionais e não funcionais do sistema e contém a prototipagem, além de diagramas UML que foram construídos levando-se em conta as funcionalidades identificadas durante a fase de concepção do sistema.

[ [INÍCIO](#fibonacci-management-system) ]

# DESCRIÇÃO GERAL

## Usuários do sistema
|USUÁRIO|DESCRIÇÃO|
|:---|:---|
|**Usuário Padrão:**|Realizam as tarefas comuns a todos os usuários, tal como: logar e enviar mensagens. Todos demais usuários estendem as funcionalidades do UsuárioPadrão|

[ [INÍCIO](#fibonacci-management-system) ]

# Requisitos do Software

A especificação dos requisitos deste documento deve seguir as recomendações da norma IEEE Std-830-1998, levando em conta as recomentações do documento de [características dos requisitos](caracteristicas_requisitos.md).

| IDENTIFICADOR | NOME | DESCRIÇÃO | PRIORIDADE |
|:---|:---|:---|:---|
| RF-001 | Realizar Login | Permitir que o usuário acesse o sistema informando email e senha válidos | Alta |
| RF-002 | Cadastro de Usuário | Permitir que novos usuários criem uma conta informando seus dados | Alta |
| RF-003 | Recuperar Conta por Email | Permitir que o usuário solicite recuperação de conta via email | Alta |
| RF-004 | Enviar Token de Verificação | Enviar um código/token para validar a recuperação de conta | Alta |
| RF-005 | Verificar Token | Validar o token informado pelo usuário para permitir redefinição de senha | Alta |
| RF-006 | Redefinir Senha | Permitir que o usuário crie uma nova senha após validação | Alta |
| RF-007 | Redirecionamento Pós-Login | Direcionar o usuário para a página principal após login bem-sucedido | Alta |
| RF-008 | Exibir Conversa em Chat | O sistema deve exibir a conversa entre usuário e IA em formato de chat, organizando perguntas e respostas | Alta |
| RF-009 | Criar Nova Conversa | O sistema deve permitir que o usuário inicie uma nova conversa com a IA | Alta |
| RF-010 | Listar Histórico de Conversas | O sistema deve exibir a lista de conversas anteriores do usuário | Alta |
| RF-011 | Selecionar Conversa | O sistema deve permitir que o usuário selecione uma conversa do histórico | Alta |
| RF-012 | Excluir Conversa | O sistema deve permitir que o usuário exclua conversas do histórico | Média |
| RF-013 | Criar Tarefa | O sistema deve permitir que o usuário crie uma nova tarefa | Alta |
| RF-014 | Editar Tarefa | O sistema deve permitir que o usuário edite uma tarefa existente | Alta |
| RF-015 | Excluir Tarefa | O sistema deve permitir que o usuário exclua uma tarefa | Alta |
| RF-016 | Marcar Tarefa como Concluída | O sistema deve permitir que o usuário marque uma tarefa como concluída | Alta |
| RF-017 | Listar Tarefas | O sistema deve exibir todas as tarefas do usuário | Alta |
| RF-018 | Filtrar Tarefas | O sistema deve permitir filtrar tarefas por status (concluídas ou pendentes) | Média |
| RF-019 | Definir Prioridade | O sistema deve permitir definir prioridade para as tarefas (opcional) | Média |
| RF-020 | Mostrar Temperatura Atual | O sistema deve exibir a temperatura atual do local selecionado | Média |
| RF-021 | Exibir Condição Climática | O sistema deve mostrar o clima atual (sol, chuva, nublado, etc.) | Média |
| RF-022 | Previsão para Próximos Dias | O sistema deve exibir a previsão do tempo para os próximos dias | Média |
| RF-023 | Detectar ou Selecionar Localização | O sistema deve detectar automaticamente a localização do usuário ou permitir a escolha de uma cidade | Média |
| RF-024 | Atualização Automática do Clima | O sistema deve atualizar automaticamente as informações climáticas | Média |
| RF-025 | Sugerir Roupa | O sistema deve sugerir roupas com base nas condições climáticas | Média |


## Requisitos Não Funcionais
A tabela a seguir contém a relação com os Requisitos Não Funcionais identificados, contendo identificador, nome, descrição e prioridade:

| IDENTIFICADOR | NOME | DESCRIÇÃO |
|:---|:---|:---|
|RNF-001 |Nome do Requisito |Descreva aqui as informações sobre o requisito |
|RNF-002 |Nome do Requisito |Descreva aqui as informações sobre o segundo requisito |

[ [INÍCIO](#fibonacci-management-system) ]

# Prototipagem

[Protótipo criado no FIGMA em 2022 por estudantes](https://www.figma.com/file/iNC7wyX9zP7Kmn3BhiCFGf/Fals6Hood-(Prot%C3%B3tipo-criado-por-estudantes-em-2022)?node-id=0%3A1&t=B16hgeZP3MSURCCa-1)

![Imagem do Protótipo](/img/home.png)

[ [INÍCIO](#fibonacci-management-system) ]


# Diagrama de Classes

![Diagrama de Classes](/img/CDModelo.png)

[ [INÍCIO](#fibonacci-management-system) ]


# REFERÊNCIAS

Esta subseção apresenta as referências aos documentos que utilizamos no auxílio à construção deste documento.
* [UML](https://www.omg.org/spec/UML/2.5/About-UML/)
* [Práticas para Especificação de Requisitos IEEE-830](https://ieeexplore.ieee.org/document/720574)
