### HU02 — Aprovação de Pedidos de Alto Valor

| **3 Ws** | **Conteúdo** |
|----------|--------------|
| **WHO? (Quem)** | **Gerente Comercial** |
| **WHAT? (O Quê)** | **Aprovar ou rejeitar pedidos** que ultrapassam um limite de valor ou envolvem produtos críticos |
| **WHY? (Por Quê)** | **Garantir conformidade com políticas de risco e margem**, evitando vendas não autorizadas |

**História de Usuário Completa**  
> Como **Gerente Comercial**, quero **aprovar ou rejeitar pedidos que excedem R$ X ou envolvem estoque crítico**, para **assegurar que apenas vendas viáveis sejam processadas**.

#### Descrição
Pedidos que atingem certos limiares entram automaticamente em estágio *Em Aprovação*. Gestores recebem notificação e podem aprovar ou rejeitar diretamente pelo sistema.

#### ✅ Critérios de Aceite
1. **Gatilho**: pedidos > R$ X **ou** que deixem saldo de item crítico < ponto de reposição entram em “Em Aprovação”.  
2. **Notificação**: gerente recebe e-mail com link direto para o pedido.  
3. **Ação**: gerente clica em **Aprovar** ou **Rejeitar**; deve preencher observação obrigatória ao rejeitar.  
4. **Transação**: ao aprovar, reserva se torna definitiva; ao rejeitar, reserva é liberada imediatamente.  
5. **Registro**: decisão, usuário e data/hora gravados no histórico do pedido.  
6. **Feedback ao Vendedor**: status atualizado em tempo real no Kanban e e-mail automático.

---