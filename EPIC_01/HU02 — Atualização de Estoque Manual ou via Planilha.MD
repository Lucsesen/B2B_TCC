### HU02 — Ajuste Manual de Saldo de Estoque

| **3 Ws** | **Conteúdo** |
|----------|--------------|
| **WHO? (Quem)** | **Almoxarife** |
| **WHAT? (O Quê)** | **Registrar manualmente entradas ou saídas de estoque** por SKU, indicando quantidade e motivo |
| **WHY? (Por Quê)** | **Manter os saldos corretos** após recebimentos, devoluções ou perdas pontuais, evitando ruptura ou super-estoque |

**História de Usuário Completa**  
> Como **Almoxarife**, quero **ajustar o saldo de estoque de forma manual** (entrada ou saída), para **garantir que o sistema reflita a quantidade real disponível no depósito**.

#### Descrição
Ocorrências diárias — como devoluções de clientes, perdas por avaria ou recebimentos não previstos — exigem correções rápidas de quantidade. A interface deve permitir ao Almoxarife efetuar o ajuste em poucos cliques, com validação imediata e rastreabilidade.

#### ✅ Critérios de Aceite
1. **Formulário de Ajuste**: campos SKU (auto-completar), Quantidade (valor positivo ou negativo) e Motivo (texto livre obrigatório).  
2. **Validação em Tempo Real**:  
   - Quantidade não pode ser zero.  
   - Para saídas, quantidade não pode exceder o saldo atual.  
3. **Confirmação**: após salvar, sistema mostra notificação de sucesso e atualiza o saldo na tela de listagem de produtos.  
4. **Log de Movimentação**: cada ajuste gera registro contendo usuário, data/hora, quantidade e motivo.  
5. **Permissões**: somente usuários com papel Almoxarife ou Administrador podem realizar ajustes.  
6. **Persistência**: alterações permanecem após recarregar a página ou relogar.  
