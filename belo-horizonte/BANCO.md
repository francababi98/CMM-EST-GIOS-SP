# Banco de dados — Belo Horizonte

O sistema de BH vai usar o **mesmo projeto Supabase** que o de São Paulo
(nada de conta nova, nada de custo — continua no plano gratuito).
As tabelas de BH têm o sufixo `_bh`, então não mexem em nada do SP.

## Passo a passo para criar o banco (uma vez só)

1. Acesse **https://supabase.com** e entre no projeto (o mesmo do SP).
2. No menu da esquerda, clique em **SQL Editor**.
3. Clique em **New query**.
4. Abra o arquivo **`schema.sql`** (nesta mesma pasta), copie **todo** o conteúdo e cole no editor.
5. Clique em **RUN** (ou `Ctrl+Enter`).

Pronto. Isso cria duas tabelas:

- **`campos_bh`** — o cadastro dos campos de estágio.
- **`alocacoes_bh`** — a distribuição das turmas nos campos.

> Pode rodar o `schema.sql` mais de uma vez sem problema: ele não apaga
> nem duplica dados, só garante que as tabelas existam.

## Depois de criar

Quando as tabelas estiverem criadas, o próximo passo é **conectar o site
a elas** (fazer o cadastro salvar e carregar do banco em vez de ficar só
na tela). Isso é rápido e a gente testa junto para confirmar que está
salvando de verdade.

## Custo

Zero. É o mesmo projeto gratuito do SP; duas tabelas pequenas a mais não
geram cobrança.
