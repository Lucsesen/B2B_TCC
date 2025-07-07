# EPIC-05: Relatórios & Dashboards Básicos

| **Atributo**           | **Valor**          |
|------------------------|--------------------|
| **ID do Épico**        | EPIC-05           |
| **Persona Principal**  | Gerente Operacional |

### Descrição
Fornece um conjunto **enxuto de relatórios** para monitorar estoque e pedidos, permitindo aos gestores avaliar rapidamente a saúde da operação sem recorrer a ferramentas externas de BI.

### Escopo e Funcionalidades Principais
- **Dashboard Resumido** na home do back-office:  
  - Valor total de estoque  
  - Pedidos por status (gráfico de barras)  
  - Top 5 SKUs com menor saldo  
- **Relatório CSV/Excel** de giro de estoque (exportável)  
- Filtros por intervalo de datas e categoria de produto  
- Atualização automática diária (ou manual on-demand)

### 📜 Histórias de Usuário
| ID   | Título                                                     |
|------|------------------------------------------------------------|
| HU01 | Visualizar Dashboard Resumido                              |
| HU02 | Exportar Relatório de Giro de Estoque                      |
| HU03 | Aplicar Filtros de Data e Categoria em Relatórios          |

### 🚀 Requisitos Não-Funcionais Chave
- **Simples**: dashboards gerados com recursos nativos da plataforma  
- **Atualização**: consultas 100 % baseadas em dados já armazenados — sem ETL externo  
- **Tempo de Geração**: exportação CSV ≤ 10 s para 10 000 registros  

### ✅ Critérios de Aceite
1. Dashboard mostra métricas corretas baseadas nos últimos dados.  
2. Exportação gera arquivo CSV/Excel com colunas e formatação definidas.  
3. Filtros alteram resultados em tempo real sem recarregar a página.  
