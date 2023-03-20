---
title: "Ferramentas Adicionais"
chapter: true
weight: 10
locale: "pt-BR"
---
## Ferramentas Adicionais

#### Importar/Exportar

Você pode importar e exportar a configuração de fluxo. Quando você importa um arquivo, o Architect analisa o arquivo para determinar o tipo de dados de configuração que ele contém. Os prompts que você recebe dependem do tipo de arquivo que está importando. Você também pode exportar o arquivo de configuração de um fluxo criado anteriormente para uso em outro fluxo. Para obter mais informações, clique para expandir as seções apropriadas e clique novamente para fechá-la.
**Observação:** importar um fluxo de uma organização externa pode exigir algumas atualizações de configuração; mesmo se for para itens como ações de dados com nomes semelhantes. Até que você atualize quaisquer problemas de configuração, o Architect retorna erros de validação no fluxo.

#### Versão

Você pode acessar o histórico de versões de um fluxo no fluxo atualmente aberto ou na lista de fluxos na página inicial do Architect. Na caixa de diálogo Versões disponíveis, você pode visualizar uma lista de todas as versões disponíveis do fluxo, incluindo:
* Se uma versão é publicada
* A cópia de trabalho mais recente
* A última data de check-in de cada versão e o autor que fez check-in no fluxo
Ao abrir uma versão anterior de um fluxo, você pode executar tarefas adicionais. Por exemplo, você pode cancelar a publicação da versão atualmente publicada. Você também pode abrir qualquer versão e exportar a configuração ou usar Salvar como para criar uma cópia do fluxo atual e salvá-la com um novo nome.

#### Validação

Quando você configura um fluxo, o Genesys Architect verifica para detectar problemas. Se o fluxo contiver erros, o número de erros aparecerá em vermelho ou amarelo para indicar que você precisa atualizar uma ação ou operação de propriedade. Os erros de validação vermelha impedem o funcionamento do fluxo e devem ser resolvidos antes que o Architect o implemente para o processamento de chamadas. Os erros de validação amarelos incluem sugestões ou recomendações de práticas recomendadas, mas não impedem o funcionamento do fluxo.
Passe o mouse sobre o botão **Validar** . O Architect exibe uma lista de erros de validação e uma explicação de cada erro.

![Architect Tools](/images/Tools.jpg)

#### Depuração (Debug)

Use o recurso de depuração no Architect para testar uma versão separada de um fluxo antes de publicá-lo. Esse recurso permite ouvir o fluxo do ponto de vista do chamador, chamando-o da Genesys Cloud. No modo de depuração, o fluxo fornece informações adicionais do sistema ao autor do fluxo. Por exemplo, ações tomadas ou resultados de processos de decisão. Você pode discar um endereço SIP que chama especificamente o fluxo. O fluxo a ser depurado não pode conter erros de validação.
Para criar uma versão de depuração de um fluxo, abra o menu **Publicar** e selecione **Depurar.** A caixa de diálogo Depurar ativada é aberta com a confirmação de que o fluxo pode ser depurado. Copie o padrão de fluxo, abra uma chamada telefônica na interface de usuário do Genesys Cloud e cole o código como seu contato a ser chamado. Usaremos esse recurso quando for a hora de testar o fluxo.

![Architect Tools cont.](/images/Debug.jpg)