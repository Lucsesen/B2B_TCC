### HU03 — Visualização de Saldo e Histórico de Movimentos

| **3 Ws** | **Conteúdo** |
|----------|--------------|
| **WHO? (Quem)** | **Administrador** |
| **WHAT? (O Quê)** | **Consultar o saldo atual de um produto e seu histórico de movimentos** |
| **WHY? (Por Quê)** | **Auditar discrepâncias** e tomar decisões de compra ou venda baseadas em dados confiáveis |

**História de Usuário Completa**  
> Como **Administrador**, quero **ver o saldo atual e o histórico de movimentações de um produto**, para **investigar divergências e assegurar conformidade**.

#### Descrição
A funcionalidade oferece transparência sobre como o estoque chegou ao valor atual: entradas, saídas, ajustes e datas correspondentes.

#### ✅ Critérios de Aceite
1. **Saldo Atual**: valor numérico exibido no topo da página do produto.  
2. **Tabela de Movimentos**: lista paginada com Data/Hora, Tipo (Entrada/Saída/Ajuste), Quantidade, Usuário e Observação.  
3. **Filtros**: por intervalo de datas e tipo de movimento; resultados atualizam sem recarregar a página.  
4. **Exportar CSV**: histórico filtrado pode ser baixado em ≤ 5 s para até 10 000 registros.  
5. **Permissões**: somente perfis Administrador acessam o histórico completo.