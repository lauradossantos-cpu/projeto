# Plataforma Critéria — Gestão Financeira

O projeto foi estruturado a partir das abas da planilha enviada: Painel, Compras, Vendas, Despesas e Fluxo de Caixa.

## Protótipo visual — Critéria
Abra `frontend/index.html` no navegador. Ele permite navegar entre módulos, cadastrar lançamentos, consultar tabelas, apagar lançamentos de Compras, Vendas e Despesas com confirmação e exportar CSV. **Nesta primeira demonstração os dados ficam no armazenamento local do navegador**; portanto, ainda não são compartilhados entre pessoas ou computadores.

## Arquitetura prevista para a versão online multiusuário
- Front-end: HTML/CSS/JavaScript (pode evoluir para React).
- Back-end: Java 21 + Spring Boot 3, API REST.
- Banco de dados: PostgreSQL ou MySQL.
- Autenticação: usuários individuais, perfis e permissões.
- Hospedagem: servidor HTTPS com backup automático.

## Módulos mapeados da planilha
- Compras: ID do veículo, data, modelo, ano, placa, comprador, valor, pagamento e observações.
- Vendas: ID do veículo, data, modelo, ano, placa, vendedor, valor, recebimento e observações.
- Despesas: data, categoria, descrição, ID do veículo, fornecedor, valor, pagamento, status e observações.
- Fluxo de caixa: data, tipo, descrição, ID do veículo, entrada, saída e observações.
- Painel: totais, saldo e contagem de veículos.

## Próxima etapa técnica
Implementar persistência no banco, autenticação e API Java. Não publicar o protótipo com dados reais: a versão local não possui login, controle de acesso nem sincronização.
