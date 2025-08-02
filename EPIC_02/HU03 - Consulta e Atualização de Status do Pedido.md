### HU03 — Consulta e Atualização de Status do Pedido

| **3 Ws** | **Conteúdo** |
|----------|--------------|
| **WHO? (Quem)** | **Vendedor B2B** (equipe interna) |
| **WHAT? (O Quê)** | **Acompanhar o status do pedido em um painel Kanban** e atualizar etapas intermediárias (ex.: faturado) |
| **WHY? (Por Quê)** | **Manter cliente e equipe informados** e reduzir dúvidas sobre andamento da entrega |

**História de Usuário Completa**  
> Como **Vendedor B2B**, quero **visualizar e atualizar o status do meu pedido em um painel Kanban**, para **acompanhar todo o ciclo até a entrega e informar o cliente prontamente**.

#### Descrição
Cada pedido percorre status pré-definidos: Novo → Em Aprovação → Aprovado → Faturado → Cancelado. O painel Kanban oferece visão rápida e permite transições autorizadas.

#### ✅ Critérios de Aceite
1. **Kanban**: colunas contendo cartões dos pedidos ordenados por data de criação.  
2. **Permissões**: vendedor pode mover cartões apenas entre estados permitidos (ex.: Aprovado → Faturado).  
3. **Atualização**: Atualizar os dados grava mudança, usuário e timestamp no histórico.  
4. **Detalhe do Pedido**: clique no cartão abre modal com itens, valores e timeline de status.  
5. **Notificações**: mudança para “Faturado” gera PDF da NF ou confirmação e envia e-mail ao cliente.  
6. **Pesquisa/Filtro**: campo para buscar pedidos por número ou cliente; filtros por período e status aplicados em tempo real.

![Mockup HU01](./HU3.png)
