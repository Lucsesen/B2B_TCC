# EPIC-04: Catálogo de Produtos (Cliente B2B)

| **Atributo**           | **Valor**            |
|------------------------|----------------------|
| **ID do Épico**        | EPIC-04             |
| **Persona Principal**  | Cliente B2B (Usuário autenticado) |

### Descrição
Este épico disponibiliza uma **vitrine simples** para que clientes logados consultem produtos em estoque, preços e prazos de entrega antes de montar o pedido.

### Escopo e Funcionalidades Principais
- **Autenticação** básica (e-mail + senha ou link mágico)  
- Página de **Lista de Produtos** com paginação e pesquisa por nome/categoria  
- **Detalhe do Produto**: foto, descrição, preço, saldo disponível  
- **Filtro rápido** por categoria, faixa de preço e disponibilidade  
- **Favoritos / Lista de Desejos** (opcional) para facilitar pedido futuro  

### 📜 Histórias de Usuário
| ID   | Título                                                    |
|------|-----------------------------------------------------------|
| HU01 | Login do Cliente e acesso ao Catálogo                     |
| HU02 | Pesquisa e Filtragem de Produtos                          |
| HU03 | Visualização de Detalhes de Produto                       |

### 🚀 Requisitos Não-Funcionais Chave
- **Performance**: pesquisa retorna < 2 s em até 5 000 SKUs  
- **Responsividade**: UI utilizável em celulares (layout de cards)  
- **Acessibilidade**: contraste adequado e navegação por teclado  

### ✅ Critérios de Aceite
1. Cliente autenticado consegue listar e filtrar produtos sem erros.  
2. Página de detalhes exibe informações corretas do SKU selecionado.  
3. Pesquisa por nome parcial devolve resultados relevantes em tempo.  
