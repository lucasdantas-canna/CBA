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

## v3 — 2026-06-25
- Agente Cotação: nova fase 0-C para cliente com cotação já em aberto
  (cliente menciona cotação existente, envia PDF de cotação ou cita número
  de cotação já existente). Nesse caso, solicita apenas o número da cotação,
  sem checklist técnico e sem coleta de dados cadastrais, e encaminha direto
  para o vendedor.

## v4 — 2026-06-25
- Val: tratamento de documento alterado para ser igual ao de imagem. Não pede
  mais descrição em texto do documento. Informa que não consegue processar e
  transfere diretamente para um vendedor, acionando o Agente Cotação e Serviços.
- Agente Cotação: fase 0-B unificada para cobrir tanto imagem quanto documento
  (mesma resposta de transferência direta, sem checklist, sem coleta de dados).
