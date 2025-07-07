### HU01 — Criação de Pedido e Reserva de Estoque

| **3 Ws** | **Conteúdo** |
|----------|--------------|
| **WHO? (Quem)** | **Vendedor B2B** |
| **WHAT? (O Quê)** | **Criar um novo pedido** selecionando itens, quantidades e condições de entrega, com validação de estoque em tempo real |
| **WHY? (Por Quê)** | **Fechar a venda rapidamente e garantir a disponibilidade dos produtos** para o cliente |

**História de Usuário Completa**  
> Como **Vendedor B2B**, quero **criar um pedido e reservar automaticamente o estoque dos itens solicitados**, para que **o cliente tenha garantia de que receberá os produtos comprados**.

#### Descrição
O formulário de pedido deve ser simples, permitindo busca de produtos, exibição de saldo disponível e cálculo automático de impostos e frete conforme UF e valor do pedido.

#### ✅ Critérios de Aceite
1. **Busca de Produtos**: autocomplete por nome ou SKU com exibição de saldo disponível.  
2. **Validação de Estoque**: sistema impede adicionar quantidade maior do que o saldo; mostra alerta em tempo real.  
3. **Cálculo Automático**: impostos (ICMS/ISS) e frete calculados após inserir CEP do cliente.  
4. **Resumo do Pedido**: total de itens, impostos, frete e valor final antes de salvar.  
5. **Reserva**: ao salvar, quantidade solicitada é reservada por até 24 h (ou até aprovação) e exibida no log de movimento.  
6. **Confirmação**: notificação de sucesso + e-mail ao cliente com número do pedido.