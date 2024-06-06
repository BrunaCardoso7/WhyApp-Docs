## **Componente MenuGroup**
O componente MenuGroup é responsável por exibir um menu lateral contendo informações e configurações relacionadas a um grupo de chat específico. Ele exibe uma lista de membros do grupo, permitindo visualizar quem está online e offline
## **Funcionalidades**
O componente MenuInfo aceita as seguintes propriedades:

- Exibe um botão para acessar o menu lateral do grupo.
- Quando o botão é clicado, o menu lateral é aberto, exibindo uma lista de membros do grupo.
- Os membros são separados entre online e offline.
- Cada membro é representado por um componente Contact, que exibe a imagem, nome e status do membro.
- Permite fechar o menu lateral clicando fora dele ou em um botão de fechar.

## **Propriedades**
O componente MenuGroup não recebe propriedades externas além das providas pelo contexto.
## **Contextos Utilizados**
- O componente `MenuGroup` utiliza o contexto ChatContext para acessar informações sobre o grupo de chat atual.

## **Hooks Utilizados**
O componente MenuInfo utiliza os seguintes estados e hooks:

- `useGetAllUsersList`: utilizado para obter a lista de todos os usuários.

# **Componentes Utilizados**
O componente MenuInfo renderiza os seguintes componentes:

- `Button`:  componente do Ant Design para renderizar um botão de ação.
- `Drawer`: componente do Ant Design para renderizar o menu lateral.
- `Flex`: componente do Ant Design para fornecer um layout flexível.
- `Contact`:  componente interno para representar os membros do grupo.
- # **Fluxo de Funcionamento**
- Ao clicar no botão de configurações, o menu lateral é aberto.
- O menu exibe o cabeçalho com o nome do grupo e uma lista de membros separados entre online e offline.
- Os membros são representados por componentes Contact.
- O menu pode ser fechado clicando fora dele ou em um botão de fechar.
