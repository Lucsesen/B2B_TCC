# EPIC-01: Gestão de Produtos & Estoque (Back-office)

| **Atributo**           | **Valor**                     |
|------------------------|------------------------------|
| **ID do Épico**        | EPIC-01                      |
| **Persona Principal**  | Administrador de Produtos    |

### Descrição
Este épico cobre todo o ciclo de **cadastro, manutenção e visibilidade do estoque**. Garante que administradores possuam uma interface robusta para gerir SKUs, categorias, saldos e pontos de reposição. O sucesso é medido pela precisão dos dados e pela rapidez com que ajustes se propagam para pedidos, relatórios e reabastecimento.

### Escopo e Funcionalidades Principais
- CRUD completo de **Produtos**, **Categorias** e **Unidades de Medida**  
- **Importação/Exportação** em massa via CSV/Excel  
- **Movimentações** de estoque (entrada, saída, ajuste, inventário)  
- **Alertas** (visual + e-mail) quando estoque < ponto de reposição  
- **Log de auditoria** com histórico de alterações

### 📜 Histórias de Usuário
| ID  | Título                                                                                 |
|-----|----------------------------------------------------------------------------------------|
| HU01 | Cadastro de Produto com validações de campo                                           |
| HU02 | Atualização de Estoque manual ou via planilha                                         |
| HU03 | Visualização de Saldo e Histórico de Movimentos                                       |

### 🚀 Requisitos Não-Funcionais Chave
- **Desempenho**: listar 1 000 SKUs em ≤ 2 s  
- **Consistência**: transações atômicas para evitar discrepâncias  
- **Localização**: máscaras numéricas e monetárias “pt-BR”

### ✅ Critérios de Aceite
1. Administrador cria, edita e exclui produtos e vê as mudanças imediatamente.  
2. Importação de 1 000 linhas gera relatório de sucesso/erro por registro.  
3. Alerta de ponto de reposição dispara automaticamente e é registrado no log. 
