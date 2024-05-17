## Mapeando o domínio

# Quais são as entidades de domínio?
- Produto (UUID)
- Estoque
- Venda
- Ordem
- Fornecedor

# Quais são as ações (casos de uso) que essa aplicação deve ter?
- Criação de Produto: Associado a um estoque.
- Rastreamento de Produto por ID e Parâmetros Opcionais: Utilizando o Unique ID (UUID) para rastrear o produto, com filtros adicionais como cor, tamanho, entre outros.
- Criação de Estoque: Associado a um produto.
- Controle de Estoque: Permite definir limites mínimos e máximos de estoque. Inclui uma funcionalidade que, ao atualizar o estoque, verifica a quantidade restante. Em caso de pouco
estoque, chama uma função 'alert' que avisa que o estoque atual está baixo.
- Envio de Alertas de Estoque: Integração com sistemas pré-existentes de gerenciamento de estoque, envio de alertas por e-mail e notificação no sistema.
- Visualização do Histórico de Estoque: Deve ser possível ver as tendências do estoque, ou seja, métricas que retornem quais produtos têm maior demanda, em uma ordem do mais   requisitado ao menos requisitado.
- Visualização do Histórico de Vendas: Deve ser possível filtrar por período de tempo, retornar o lucro gerado por produto e os produtos mais vendidos.
- Criação de Ordem de Compra Automática: Baseada em histórico de estoque e vendas.
- Gerenciamento de Ordem de Compra Automática: Realiza compras automáticas baseadas em métricas do histórico de estoque e na quantidade de estoque.
- Integração com Fornecedor: Recebe atualizações sobre prazos de entrega e novas remessas.





