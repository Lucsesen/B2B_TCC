### HU01 — Cadastro de Produto com Validações de Campo

| **3 Ws** | **Conteúdo** |
|----------|--------------|
| **WHO? (Quem)** | **Administrador de Produtos** |
| **WHAT? (O Quê)** | **Cadastrar um novo produto** preenchendo todos os campos obrigatórios com validação em tempo real |
| **WHY? (Por Quê)** | **Garantir a integridade do catálogo** e evitar erros que prejudiquem preços, estoque ou integrações |

**História de Usuário Completa**  
> Como **Administrador de Produtos**, quero **cadastrar um novo produto com todas as validações de campo**, para que **o catálogo permaneça preciso e confiável**.

#### Descrição
O cadastro de produto é o ponto de entrada para todas as demais operações de estoque e vendas. Validações imediatas evitam dados incoerentes (SKU duplicado, preço negativo, valores vazios) e reduzem retrabalho.

#### ✅ Critérios de Aceite
1. **Campos Obrigatórios**: Nome, SKU (único), Categoria, Unidade, Preço, Saldo Inicial.  
2. **Validação em Tempo Real**: campos numéricos só aceitam números positivos; preço exibe máscara “R$ 0,00”.  
3. **Unicidade do SKU**: tentativa de salvar SKU já existente gera mensagem de erro clara.  
4. **Confirmação**: após salvar, sistema exibe notificação de sucesso e produto aparece na lista.  
5. **Persistência**: dados permanecem após recarregar a página ou relogar.
