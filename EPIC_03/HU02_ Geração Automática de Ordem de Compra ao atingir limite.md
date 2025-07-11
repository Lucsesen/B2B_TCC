### HU02 — Geração Automática de Ordem de Compra ao atingir limite

| **3 Ws** | **Conteúdo** |
|----------|--------------|
| **WHO? (Quem)** | **Comprador** |
| **WHAT? (O Quê)** | **Que o sistema gere uma ordem de compra automaticamente para o fornecedor preferencial** |
| **WHY? (Por Quê)** | **Para não precisar monitorar o estoque manualmente e o processo de compra seja agilizado.** |

**História de Usuário Completa**
> Como **comprador**, quero **que o sistema gere uma ordem de compra automaticamente para o fornecedor preferencial**, para que **eu não precise monitorar o estoque manualmente e o processo de compra seja agilizado**.

#### Descrição
A geração automática de ordens de compra otimiza o processo de reabastecimento, reduzindo a carga de trabalho manual e minimizando o risco de falta de estoque. Isso garante que os produtos estejam sempre disponíveis para atender à demanda.

#### ✅ Critérios de Aceite
1.  Quando o saldo de um SKU se torna igual ou inferior ao ponto de reposição, uma OC deve ser criada.
2.  A OC deve conter o SKU, a quantidade padrão de compra e os dados do fornecedor preferencial.
3.  A OC deve ser criada com o status "Pendente de Aprovação".
4.  Um e-mail de notificação deve ser enviado para o comprador responsável.



