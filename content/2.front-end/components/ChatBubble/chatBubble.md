# **Componente ChatBubble**
O ChatBubble exibe uma bolha de chat que contém uma mensagem. Ele diferencia automaticamente as mensagens enviadas pelo usuário atual das mensagens recebidas de outros usuários.
# **Funcionalidades Principais**
- `mensagem: string`: A mensagem a ser exibida na bolha de chat
- `fromUserId: string`: O ID do usuário que enviou a mensagem.
- `createdAt: Date | undefined`: O horário de envio da mensagem.
  
# **Componentes**
O componente ChatBubble renderiza os seguintes componentes:

- `SentAt`: um componente que exibe a data e hora de envio da mensagem.
- `children`: Conteúdo que é envilvido pelo chat bubble.

# **Exemplo de uso**

- `userId`: obtido dos cookies usando Cookies.get('userId').
```javascript
    <ChatBubble
        mensagem={chat.mensagem}
        createdAt={chat.createdAt}
        fromUserId={chat.fromUserId}
        >
        <Highlighter
            style={{
            color: '#FFFFFF',
            paddingRight: '1.5rem',
            maxWidth: '16rem',  
            fontSize: '1rem',
            lineHeight: 1.5,
            margin: '0px',
            }}
            activeClassName="Active"
            activeIndex={localActiveIndex}
            autoEscape={true}
            highlightClassName="Highlight"
            searchWords={[searchTerm]}
            textToHighlight={chat.mensagem}
        />
    </ChatBubble>
```