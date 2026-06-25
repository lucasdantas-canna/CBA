# Changelog — Prompts CBA

## v1 — 2026-06-25
- Versão inicial dos prompts: Val (orquestradora), Agente Cotação e Serviços,
  Agente Pedidos, Agente Financeiro, Agente Suporte e Geral.
- Agente Cotação: quando o cliente informa código/referência do produto, não
  aplica mais checklist técnico completo, pergunta apenas a quantidade.

## v2 — 2026-06-25
- Val: tratamento de imagem alterado. Ao receber imagem, não pede mais
  descrição em texto. Informa que não consegue visualizar e transfere
  diretamente para um vendedor, acionando o Agente Cotação e Serviços.
- Agente Cotação: nova fase 0-B para transferência direta por envio de
  imagem. Pula checklist, pula "Buscar Produto", pula coleta de dados
  cadastrais, aciona direto a tool "Cotação / Orçamento concluído" e encerra.
