# CBA Automação — Prompts dos Agentes

Prompts atuais do sistema multiagente de atendimento WhatsApp da CBA Automação
(Central Brasileira de Automação), construído em n8n + Chatwoot + Supabase + SIGE Cloud.

## Estrutura

- `prompts/val_orquestradora.txt` — Val, agente orquestrador. Recebe a mensagem do cliente,
  identifica a intenção e aciona o agente especialista correto.
- `prompts/agente_cotacao_servicos.txt` — Agente Cotação e Serviços. Qualifica tecnicamente
  pedidos de cotação de produtos e serviços, coleta dados cadastrais e valida CNPJ/CPF.
- `prompts/agente_pedidos.txt` — Agente Pedidos. Trata acompanhamento de pedidos já realizados,
  rastreio e coleta de material.
- `prompts/agente_financeiro.txt` — Agente Financeiro. Trata boletos e dados bancários.
- `prompts/agente_suporte_geral.txt` — Agente Suporte e Geral. Trata suporte técnico,
  vagas, parcerias e endereço.

## Observações

- Os agentes especialistas são acionados pela Val como tools dentro do AI Agent node (n8n).
- Memória de conversa: Postgres Chat Memory (Supabase), tabela `n8n_chat_histories`.
