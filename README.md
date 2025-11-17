# Desafio_Final_BootcampI
Repositorio BootcampI criação 3.0

Repositorio BootcampI criação

Link Apresentação(Site): https://gemini.google.com/share/9fefa05899a8

Link linkedin: https://www.linkedin.com/feed

Link GitHub: https://github.com/Vitor5-dotcom


# Projeto MER – Sistema de Pedidos

Este projeto apresenta a modelagem conceitual de um sistema de controle de pedidos,
incluindo dicionário de dados, regras de negócio e visões solicitadas.  
O diagrama MER foi desenvolvido no **brModelo**, seguindo boas práticas de modelagem.

### Principais pontos:
- Cadastro de clientes (PF e PJ com especialização).
- Controle de produtos, prateleiras e estoque.
- Registro de pedidos com itens relacionados a clientes e vendedores.
- Regras de negócio: cada pedido possui ao menos um produto; CPF/CNPJ são únicos; histórico de preços.
- Visões implementadas: clientes, capacidade de estoque por prateleira, saldo de produtos.


# Banco de Dados NoSQL – Estudo Comparativo

Este trabalho apresenta uma visão geral sobre bancos de dados NoSQL, destacando sua
importância em cenários de escalabilidade, flexibilidade de esquema e alto volume de dados.  
Também compara os modelos **relacional (PostgreSQL)** e **NoSQL (MongoDB)**.

### Conteúdo abordado:
- Fundamentos de NoSQL: chave-valor, documentos, colunar e grafos.
- Relação com OLTP e OLAP.
- Trade-offs de escalabilidade e consistência (teorema CAP).
- Comparação técnica entre PostgreSQL e MongoDB:
  - Modelo de dados e esquema.
  - Linguagem de consulta.
  - Escalabilidade e flexibilidade.
  - Transações e consistência.
  - Desempenho.
 
##Gestão de Usuários e Políticas de Segurança (Foco na Entrega Final)

Esta seção documenta a **robustez das políticas de segurança** implementadas neste repositório PortfolioHUB, com apoio da consultoria do Google Gemini, para controlar o acesso e proteger a integridade do código e dos dados.

### 1. Gestão de Usuários e Níveis de Acesso

O acesso ao repositório é rigorosamente controlado sob o **Princípio do Menor Privilégio**:

| Papel | Descrição | Permissão no GitHub |
| :--- | :--- | :--- |
| **Proprietário** (Vitor Davi) | Controle administrativo total do repositório. | **Admin** |
| **Colaboradores** | (Ex: Professores/Avaliadores) Acesso temporário para fins de avaliação. | **Read/Triage** (Leitura e Triagem) |
| **Público** | Qualquer pessoa acessando o portfólio. | **Read** (Leitura) |

### 2. Políticas de Segurança Implementadas

1.  **Autenticação de Dois Fatores (MFA):** Obrigatória para o Proprietário, garantindo a proteção contra acesso não autorizado.
2.  **Proteção de Branch (`main`):**
    * **Regra Essencial:** Commits diretos na branch `main` são **bloqueados**.
    * **Procedimento:** Toda alteração de código ou documentação deve ser feita via Pull Request (PR) a partir de uma branch secundária (`feature/` ou `bugfix/`). Isso garante rastreabilidade e impede corrupção acidental do portfólio principal.
3.  **Gerenciamento de Dados Sensíveis:**
    * **Política:** Nenhum dado sensível (chaves de API, tokens, senhas ou informações confidenciais) é permitido no repositório.
    * **Implementação:** Utilização do arquivo `.gitignore` para bloquear o upload de arquivos de configuração locais (como `.env` ou chaves JSON).

---
