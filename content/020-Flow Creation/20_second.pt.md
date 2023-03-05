---
title: "Menu Inicial"
chapter: true
weight: 20
locale: "pt-BR"
---

## Menu Inicial

Quando você começar, seu menu inicial consistirá em dois nós, **Menu Principal** e **Desconectar**. Se você selecionar Menu principal, terá a opção de configurar uma **Saudação inicial** e um **Aviso de menu**. Este é o prompt de áudio e as opções disponíveis que seus clientes ouvirão quando ligarem para sua central de atendimento. Usaremos a conversão de texto em fala (TTS) do Genesys Architect em nosso tutorial, mas você também pode fazer upload de prompts de áudio pré-gravados para o fluxo.

Na caixa de ferramentas à direita, você verá **Menu** e **Tarefa**. Uma ação de **Menu** permite criar um submenu. Aqui é onde você atribuirá configurações comuns, como DTMF e reconhecimento de fala por opção. Use a ação **Tarefa** para criar opções de URA complexas. Uma ação de tarefa agrupa etapas relacionadas de um processo para criar uma rotina de fluxo. Um processo é composto pelas tarefas envolvidas, a sequência dessas tarefas e as ações que existem entre elas. Uma **Tarefa** usará os mesmos recursos de DTMF e Reconhecimento de fala que **Menus**. 

![Setting up Main Menu](/images/Menu.jpg)

Em nossa barra de ferramentas, clique em **Tarefa**, lá você encontrará nosso submenu de opções de tarefas. Nossas ferramentas do Architect usam a funcionalidade de arrastar e soltar para facilitar o uso. Clique no item de submenu **Tarefa** e arraste-o para **Desconectar** em nosso **Menu Principal**. Largue isso aí. Agora podemos adicionar o DTMF como “1” e digitar “Um (One)” em nosso campo **Reconhecimento de fala (Speech Recognition)**. Agora, nossos clientes podem realizar essa tarefa pressionando uma tecla em seu telefone ou simplesmente dizendo "um". Vamos também clicar no cabeçalho da tarefa, atualmente intitulado "Nova tarefa 1". Vamos renomeá-lo como "Help Desk".

Você notará à esquerda; nossa tarefa tem um ícone vermelho próximo a ela. Voltaremos para concluir esta tarefa no próximo módulo e mostraremos o que representa o ícone vermelho e como corrigi-lo

![Menu Options](/images/MenuOptions.jpg)