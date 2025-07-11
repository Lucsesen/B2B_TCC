| **O Quê (What)** | **Quem (Who)** | **Por Que (Why)** |
|---|---|---|
| Gerar ordem de compra automaticamente | Comprador | Para não precisar monitorar o estoque manualmente e agilizar o processo de compra. |

**HU02: Geração Automática de Ordem de Compra ao atingir limite**

*   **Como um** comprador,
*   **Eu quero** que o sistema gere uma ordem de compra automaticamente para o fornecedor preferencial,
*   **Para que** eu não precise monitorar o estoque manualmente e o processo de compra seja agilizado.

**Critérios de Aceite:**

1.  Quando o saldo de um SKU se torna igual ou inferior ao ponto de reposição, uma OC deve ser criada.
2.  A OC deve conter o SKU, a quantidade padrão de compra e os dados do fornecedor preferencial.
3.  A OC deve ser criada com o status "Pendente de Aprovação".
4.  Um e-mail de notificação deve ser enviado para o comprador responsável.



