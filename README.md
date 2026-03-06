# Sistema de Receitas Culinárias

#### Sistema web para gerenciamento de receitas culinárias de uso próprio, permitindo que usuários façam cadastro, login e armazenem suas próprias receitas.

#### O sistema é dividido em Back-end e Banco de Dados, onde o usuário pode criar e listar receitas de forma segura.

---

# Equipe do Projeto

- Gabriele Alves
- Clarisse Gondim
- José Vianei

---

# Tecnologias Utilizadas

- Node.js
- Express
- CORS

---

# Instalação do Projeto

 ## instale as dependências:

 ```
   npm install express
   npm install cors
 ```
 # Como iniciar o servidor

## Execute o comando:
```
npm start
```

Após iniciar, o servidor estará disponível em:

http://localhost:3000


---

# Estrutura do Sistema

## O sistema é dividido em três partes principais:

1. Back-end

- Responsável pela lógica do sistema.

2. Funções:

- Implementação de endpoints da API

- Validação de dados

- Comunicação com o banco de dados

3. Banco de Dados

- Responsável pelo armazenamento das informações.

# Funcionalidades do Sistema


## Backend

- Valida os dados da receita

- Salva no banco de dados

Banco de Dados: 

- Armazena a receita vinculada ao ID da receita.

- Lista as receitas


# Rotas da API

## Endpoints
```

**Retorna todas as receitas cadastradas.** 

GET /receita/receitaTotal

Exemplo de acesso:

http://localhost:3000/receita/receitaTotal

Resposta

[
  {
    "id": 1,
    "nome": "Bolo de chocolate",
    "ingredientes": "farinha, ovos, chocolate",
    "modo_preparo": "Misturar tudo e assar"
  }
]

**Adiciona uma nova receita ao sistema.**


POST /receita/receitaCriar

Exemplo:

http://localhost:3000/receita/receitaCriar

Body (JSON)

{
  "nome": "Bolo simples",
  "ingredientes": "farinha, ovos, leite",
  "modo_preparo": "Misturar os ingredientes e levar ao forno"
}

```

# Testando a API

Você pode testar as rotas usando:

- Postman

- Insomnia

- Thunder Client (VS Code)