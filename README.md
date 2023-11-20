# group_chat
Implementação de uma versão simplificada do sistema de gerenciamento de mensagens utilizando python.

RELATÓRIO

  O programa consiste em um sistema de troca de mensagens em Python,
com uso de um banco de dados SQLite para armazenamento eficiente. Seguindo o modelo
"SEND (receptor, mensagem)" e "RECEIVE (transmissor, mensagem)", o sistema permite o
envio de mensagens individuais ou em grupo.

  O banco de dados SQLite, denominado "sistema_mensagens.db," é a base do
sistema e possui uma tabela chamada "mensagens." Essa tabela armazena informações
essenciais, como remetente, destinatário, conteúdo da mensagem, prioridade, grupo, status
de visualização e data de envio.

  Foram implementadas funções que incluem a criação da tabela, envio de
mensagens, listagem de mensagens de remetentes específicos, listagem de mensagens
não lidas de destinatários, listagem de mensagens para destinatários, listagem de
mensagens para grupos e verificação de mensagens não lidas.

  A função "enviar_mensagem()"atende a dois cenários principais:
  
  - Mensagens Individuais: Quando destinatários individuais são especificados, a função cria
entradas separadas no banco de dados para cada destinatário, compartilhando o mesmo
conteúdo da mensagem.

- Mensagens em Grupo: Quando um grupo é o destinatário, a mensagem é registrada no
banco de dados com o nome do grupo, tornando-a visível para todos os membros do grupo.

A interface do sistema é interativa, com um menu que oferece opções para enviar,
ler e listar mensagens. As mensagens são gerenciadas automaticamente, incluindo
marcação como lidas quando visualizadas. Além disso, há uma opção para listar todas as
mensagens do banco
