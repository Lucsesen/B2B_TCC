# EPIC-03: Reposição de Estoque & Ordens de Compra (Supply)

| **Atributo**           | **Valor**              |
|------------------------|------------------------|
| **ID do Épico**        | EPIC-03               |
| **Persona Principal**  | Almoxarife / Comprador |

### Descrição
Focado na **automação do reabastecimento**. Gere Ordens de Compra (OC) quando o ponto de reposição é atingido, integra-se com fornecedores e atualiza o estoque ao receber mercadorias. Sucesso é medido pela redução de rupturas e agilidade no ciclo OC → Recebimento.

### Escopo e Funcionalidades Principais
- Monitoramento contínuo de níveis de estoque e ponto de reposição  
- **Geração automática** ou manual de OC para fornecedor preferencial  
- Tela de **Recebimento**: conferência de quantidades e atualização de saldo  
- Relatório de **Lead Time** e rupturas por produto

### 📜 Histórias de Usuário
| ID  | Título                                                                    |
|-----|---------------------------------------------------------------------------|
| HU01 | Definir Ponto de Reposição por SKU                                       |
| HU02 | Geração Automática de Ordem de Compra ao atingir limite                  |
| HU03 | Recebimento de Mercadoria e ajuste de estoque                            |

### 🚀 Requisitos Não-Funcionais Chave
- **Confiabilidade**: falha de integração deve ter retry automático  
- **Auditabilidade**: trilha completa de quem gerou e recebeu cada OC  
- **Integração Externa**: API segue contrato JSON REST v1

### ✅ Critérios de Aceite
1. Sistema gera OC sempre que estoque ≤ ponto de reposição e registra no log.  
2. Recebimento parcial/total reflete imediatamente no saldo.  
3. Relatório de Lead Time mostra datas de OC, recebimento e dias corridos.  
