# **Componente MenuInfo**
O componente MenuInfo é responsável por exibir as informações do usuário ou do grupo em um drawer lateral. Ele também gerencia a adição e remoção de membros de um grupo.
## **Descrição**
O MenuInfo exibe as informações do usuário ou do grupo em um drawer lateral. Ele contém dois subcomponentes: MenuPrivateUSer para exibir as informações do usuário e MenuInfoGroup para exibir as informações do grupo. Além disso, gerencia a adição e remoção de membros de um grupo utilizando os subcomponentes ModalAlert, AddMemberMutation e RemMemberMutation.

![Texto alternativo](../../../../imagens/menuinfoprivate.png)
## **Funcionalidades Principais**
- Exibição das informações do usuário ou do grupo em um drawer lateral.
- Gerenciamento da adição e remoção de membros de um grupo.
## **Subcomponentes**
- [`MenuPrivateUSer`](./MenuInfoPrivate/menuprivate.md): um componente para exibir informações sobre o perfil privado do usuário
- [`MenuInfoGroup`](./MenuInfoPrivate/menuprivate.md): um componente para exibir informações sobre o grupo de destinatários da conversa
- [`ModalAlert`](./Components/ModalAlert/ModalAlert.md):  um componente para exibir alertas modais de adição/remoção de membros
- [`AddMemberMutation`](./Components/ModalAlert/ModalAlert.md):  Mutação utilizada para adicionar membros ao grupo.
- [`RemMemberMutation`](./Components/ModalAlert/ModalAlert.md):  Mutação utilizada para remover membros do grupo.

## **Props Principais**
O componente MenuInfo utiliza os seguintes estados e hooks:

- `open`:  Indica se o drawer está aberto ou fechado.
- `onClose`:Função de retorno de chamada chamada quando o drawer é fechado.  

## **Exemplo de Uso**
```javascript
    <MenuInfo open={open} onClose={() => setOpen(false)} />

```
