# EPIC-02: Fluxo de Pedido de Venda (B2B)

| **Atributo**           | **Valor**                 |
|------------------------|---------------------------|
| **ID do Épico**        | EPIC-02                  |
| **Persona Principal**  | Vendedor B2B             |

### Descrição
Abrange **criação, aprovação e acompanhamento de pedidos**. Conecta estoque disponível, regras de negócio (“não vender sem estoque”) e comunicação com o cliente. O sucesso é medido pelo tempo médio de ciclo de pedido e taxa de pedidos aprovados sem retrabalho.

### Escopo e Funcionalidades Principais
- Formulário de **Novo Pedido** com validação de estoque em tempo real  
- **Cálculo automático** de impostos e frete (UF & valor)  
- **Workflow de aprovação** para pedidos > R$ X ou estoque crítico  
- **Geração de PDF** de confirmação + envio por e-mail ao cliente  
- Painel **Kanban** de status (Novo, Em Aprovação, Aprovado, Faturado, Cancelado)

### 📜 Histórias de Usuário
| ID  | Título                                                                            |
|-----|-----------------------------------------------------------------------------------|
| HU01 | Criação de Pedido e reserva de estoque                                           |
| HU02 | Aprovação automática/gestores para pedidos de alto valor                         |
| HU03 | Consulta e atualização de status de Pedido                                       |

### 🚀 Requisitos Não-Funcionais Chave
- **Transacionalidade**: reserva de estoque só confirma após aprovação  
- **Escalabilidade**: suportar picos de 100 pedidos simultâneos  
- **Segurança**: acesso restrito por papel (Vendedor não vê margem)

### ✅ Critérios de Aceite
1. Pedido não avança se quantidade solicitada exceder saldo disponível.  
2. Aprovação dispara e-mail para gestor e atualiza status no Kanban.  
3. PDF contém itens, impostos, totais e assinatura digital.
