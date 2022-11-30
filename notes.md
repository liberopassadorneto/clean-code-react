# Desacoplando componentes

1. Quando eu tenho algo repetitivo
2. Quando eu consigo isolar algo do seu contexto (sem prejudicar o funcionamento original)
3. Reutilizar o component em outros lugares da aplicação

# Componentes puros

- Não dependem de nenhum dado externo (chamada api, variáveis globais, etc)

# Funções e eventos no React

- handle: funções que são disparadas por eventos de usuários. Ex.: handleCreateNewTodo()
- on: components que recebem funções como parâmetros. Ex.: onClick={onCreateNewTodo}

# Composição vs Customização

- Composição de componentes
- Customização: criar várias props para customizar o componente (depreciado!!)

# Condicionais no render

- Evite colocar muita operações javascript dentro do render
  Ex.:

```tsx
const isTodoListEmpty = todos.length === 0;

{
  isTodoListEmpty && <p>Nenhum todo cadastrado.</p>;
}
```
