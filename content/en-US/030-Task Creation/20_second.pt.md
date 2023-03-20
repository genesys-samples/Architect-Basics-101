---
title: "Criação de Fluxo"
chapter: true
weight: 20
locale: "pt-BR"
---

## Criação de Fluxo

Normalmente, a primeira etapa em um fluxo de chamada será identificar nosso cliente. Isso será feito com uma chamada de dados por meio de ação de dados em um CRM ou uma pesquisa de tabela de dados para extrair o registro do cliente. Isso enviará informações relevantes sobre o cliente a um agente para ajudar a orientar a jornada do cliente. Avisos de áudio também podem ser usados ao longo do caminho para cumprimentar ou orientar o cliente. Aqui pode ser apresentada a variável vinculada ao cadastro do cliente. Por exemplo, o fluxo pode fazer referência ao nome do cliente para reproduzir em um prompt de áudio personalizado. Depois que um cliente é identificado, a decisão do que deve ser apresentado ao agente é feita com uma tela pop-up. O Genesys Cloud CX oferece uma ferramenta de script nativa para criar scripts configuráveis ou pode fazer referência a integrações de terceiros para exibir o registro do cliente ao agente.

Nosso objetivo neste tutorial é enviar a chamada de entrada diretamente para o agente. Isso pode ser feito com **Transferir > Transferir para DAC**. Como a **Tarefa** anterior. Isso pode ser arrastado e solto na linha do tempo do fluxo. 

NEm seguida, faremos referência à fila à qual nosso agente pertence. Se você ainda não configurou uma fila, pode seguir os passos aqui, https://help.mypurecloud.com/articles/create-queue/

![Transfer to ACD](/images/Transfer.jpg)

**Observação: erros de validação em vermelho impedem a publicação de um fluxo e devem ser resolvidos antes que o Genesys Architect o implemente para processamento de chamadas. Em amarelo são sugestões ou recomendações de práticas recomendadas, mas não impedem o funcionamento de um fluxo.**

Você notará que nossos prompts de áudio **Pré-transferência** e **Falha na transferência** estão marcados em amarelo. Embora o fluxo ainda seja publicado, podemos nos livrar deles digitando um prompt para cada um. Digite "transferindo" em **Áudio pré-transferência** e "falha ao transferir" em **Falha ao transferir áudio**. Você não deve mais ter marcadores de validação amarelos.

Finalmente, um marcador de validação vermelho deve permanecer. Isso ocorre porque, se o fluxo não conseguir se conectar com êxito a uma fila, o caminho não terá outro lugar para ir. Podemos resolver isso fornecendo um nó **Desconectar**, pular para outro menu ou tarefa ou criar um loop. Para o workshop de hoje, vamos arrastar e soltar um **Desconectar** da barra de ferramentas.

Estamos prontos para **Salvar e publicar**

![Transfer to ACD](/images/Validate.jpg)
