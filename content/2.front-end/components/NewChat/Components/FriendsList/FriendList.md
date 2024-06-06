## **Componente FriendsList**
O FriendsList exibe a lista de amigos do usuário e oferece a funcionalidade de adicionar ou remover amigos. Ele também permite que o usuário inicie uma conversa com um amigo clicando em seu perfil.

## **Funcionalidades**
O componente MenuInfo aceita as seguintes propriedades:

- **Exibição da Lista de Amigos** : O componente exibe a lista de amigos do usuário, cada um representado por um cartão com o nome e a foto do amigo.
- **Adição ou Remoção de Amigos**: Cada cartão de amigo possui um botão que permite ao usuário adicionar ou remover o amigo da lista.
- **Início de Conversa**: Ao clicar no perfil de um amigo, o usuário pode iniciar uma conversa com esse amigo.

## **Propriedades**

- `onClose: () => void`: Função de retorno de chamada chamada quando o componente é fechado.
# **Componentes Utilizados**
O componente MenuInfo renderiza os seguintes componentes:

- `setRecipient`:  Este hook do contexto ChatContext é usado para definir o destinatário da conversa quando o usuário clica no perfil de um amigo para iniciar uma conversa.
- `useGetFriendsList`: Este hook personalizado é utilizado para obter a lista de amigos do usuário atual.
- `RemoveFriendMutation`: Esta mutação é usada para remover um amigo da lista de amigos do usuário.
  
```javascript
    <FriendsList onClose={onClose} />
```