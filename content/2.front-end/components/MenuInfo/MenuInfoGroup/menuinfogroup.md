## **Componente MenuInfoGroup**
O componente MenuInfoGroup é utilizado para exibir informações detalhadas sobre um grupo específico em um menu lateral. Ele apresenta a imagem do grupo, nome, número de membros, descrição, lista de membros, e opções para silenciar notificações, adicionar e remover membros do grupo, e excluir o grupo.

![Texto alternativo](../../../../../imagens/menuinfogroup.png)
## **Propriedade**
O componente MenuInfoGroup aceita as seguintes propriedades:

- `recipientGroup`:  um objeto que representa o grupo cujas informações serão exibidas. Deve seguir a estrutura do modelo RecipientGroup.
- `onClose`:  uma função que é chamada quando o menu deve ser fechado.
- `setOpenModal`: ma função para abrir um modal.
- `openModal`:  uma função para fechar o drawer
- `setTagModal`:   uma função para definir o título e a subtitulo do modal.
- `setprofileInfoMenuOpen`:  uma função para abrir ou fechar o menu de informações do grupo.
- `setIsModalOpen`:   uma função para definir se o modal está aberto ou fechado

## **Estado**
O componente MenuInfoGroup utiliza o estado interno para controlar se o modal está aberto ou fechado.

# **Componentes Renderizados**
- `ProfileImage`: componente que exibe a imagem do grupo.
- `NameProfile`: componente que exibe o nome do grupo.
- `SilenceNotifications`: componente que permite silenciar as notificações do grupo.
- `ButtonAddMember`:  componente que exibe um botão para adicionar membros ao grupo.
- `ButtonRemoveMember`:  componente que exibe um botão para remover membros do grupo.
- `ButtonDeleteGroup`: componente que exibe um botão para excluir o grupo.
- `DescriptionUsers`:  componente que exibe a descrição do grupo.
- `Contact`:  componente que representa um membro do grupo.
```javascript
   <MenuInfoGroup
        recipientGroup={recipientGroup}
        onClose={onClose}
        setOpenModal={setIsModalOpen}
        openModal={openModal}
        setTagModal={setTagModal}
        setprofileInfoMenuOpen={setprofileInfoMenuOpen}
        setIsModalOpen={setIsModalOpen}
    />
```