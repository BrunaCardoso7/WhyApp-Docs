## **Componente GroupsList**
O componente GroupsList é responsável por exibir a lista de grupos de chat do usuário, permitindo a interação para selecionar um grupo ou criar um novo grupo. Ele permite ao usuário visualizar todos os grupos de chat disponíveis, selecionar um grupo para iniciar uma conversa e criar novos grupos.
## **Propriedade**
O componente GroupsList aceita as seguintes propriedades:

- `onClose`:  uma função para fechar o drawer ou modal de exibição da lista de grupos.
## **Estado e Hooks Utilizados**
O componente GroupsList utiliza os seguintes estados e hooks:

- `setRecipientGroup`: uma função do contexto ChatContext para definir o grupo de destinatários da conversa.
- `groupsList`: a lista de grupos de chat do usuário, obtida pelo hook useGetGroupsChats.      
- `groupsLoading`: um estado booleano que indica se a lista de grupos está carregando.
- `groupsError`:  um estado que armazena erros na obtenção da lista de grupos.

# **Funções Utilizadas**
O componente MenuInfo renderiza os seguintes componentes:

- `setRecipientGroup`: uma função para definir o grupo selecionado como destinatário da conversa.
- `onClose`: uma função para fechar o drawer ou modal de exibição da lista de grupos.
- # **Componentes Renderizados**
  
- `Flex`:  um componente de layout para organizar elementos em uma coluna.
- `UserCard`:  um componente que exibe as informações de um grupo em um cartão.
- `CreateNewGroupButton`: um componente para criar um novo grupo de chat.


