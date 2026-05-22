# MMC Catálogo Público

Catálogo público de plataformas elevatórias, muncks e guindastes da MMC Locações.

## Acessos

- **URL pública:** https://mmc-catalogo.vercel.app/
- **Ficha individual:** `/?manual={slug}` (exemplo: `/?manual=jlg-450aj`)

## Como funciona

Site estático que lê a tabela `manuais` do Supabase. Mostra apenas registros com `publico=true`. Não tem rotas administrativas — qualquer URL fora do catálogo cai na home (que mostra a grade de todos os modelos).

## Por que separado do CRM

Foi separado do `mmc-crm.vercel.app` por segurança: clientes que recebem o link do catálogo nunca caem no CRM, mesmo se apagarem a query string. Esse projeto não tem nada do CRM — só código de leitura pública.

## Para adicionar/editar manual

Use o painel CRM em https://mmc-crm.vercel.app/ → aba Manuais. As mudanças aparecem aqui automaticamente (lê do mesmo Supabase).
