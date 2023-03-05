---
title: "Programação"
chapter: true
weight: 20
locale: "pt-BR"
---

## Programação

Definir e gerenciar cronogramas pode ser complicado. Para ajudar nesse processo, use agendamentos com grupos de agendamento para permitir mais flexibilidade na forma como sua organização gerencia as horas de roteamento. Horários são os blocos de tempo para os quais uma rota de chamada é selecionada. Grupos de agendamento permitem combinar vários agendamentos e associá-los a uma definição de roteamento singular. Você pode atribuir os horários em um fuso horário designado e agrupá-los por tipo. Os tipos são limitados a Horário Aberto, Horário Fechado ou Feriado.

Ainda em **Roteamento**, clique em **Programação**. Em seguida, clique na guia **Programações**. Clique em **+Adicionar Programação.** Vamos nomear esse agendamento como "Workshop aberto".

Vamos ativar a **Repetitção de Evento** e repeti-lo uma vez por dia, pois esse é o horário de funcionamento de nossas centrais de atendimento. Definiremos os parâmetros de horário como 7h às 17h. Se você for testar esse fluxo, certifique-se de atribuir horas à sua programação que correspondam ao seu teste.

![Routing Schedule](/images/Schedule.jpg)

Deixaremos os critérios adicionais por enquanto, clique em **Salvar.**

Retorne ao Menu Principal **Programação** e desta vez crie um **Grupo de Programações** na parte superior. Clique em **+Agendar Grupo** e nomeie-o como “Grupo de Workshop”. À direita, adicionaremos um fuso horário e, em **Programações**, adicionaremos um em **Aberto.**

Você verá um menu suspenso e podemos escolher o “Workshop Open”, que criamos anteriormente. Você pode adicionar parâmetros de tempo adicionais em **Fechado** e **Feriado**, mas por enquanto vamos economizar.

Vamos retornar ao nosso fluxo de chamadas de entrada escolhendo **Administração > Architect > Fluxo de Entrada > “Workshop – Seu Nome”.** Agora, em nossa tarefa de help desk, abra **Logical** na barra de ferramentas. Você deve ver uma opção para **Avaliar grupo de programação**, arraste e solte-a na parte superior do fluxo, acima de **Transferir para DAC.** À direita, escolha **Grupo de Programação** como Workshop Group . Agora você verá que seu fluxo pode se ramificar com base no horário de sua central de atendimento. Embora não precisemos adicionar caminhos adicionais aqui, sinta-se à vontade para adicionar quaisquer tipos de transferência adicionais na barra de ferramentas. 

![Routing Schedule Group](/images/ScheduleGroup.jpg)