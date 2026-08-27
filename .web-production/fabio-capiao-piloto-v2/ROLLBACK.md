# ROLLBACK

Criado em: 27/08/2026

## Baseline

- repositório: `advanx-tecnologia/pages-clientes`
- branch base: `main`
- commit anterior: `0c9021b`
- página original preservada: `fabio-capiao.html`
- nova rota: `/fabio-capiao-piloto-v2/`
- backup: `/root/.hermes/backups/fabio-capiao-piloto-v2-20260827_175004/`

## Rollback

Antes do merge: fechar eventual PR e excluir o branch `feat/fabio-capiao-piloto-v2`.

Depois do merge, somente com autorização: reverter o commit do piloto e confirmar que a rota nova retorna 404. A página original deve permanecer intacta.
