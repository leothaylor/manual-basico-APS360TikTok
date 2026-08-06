# Preparação de domínio — Manual Básico APS 360

Estado-base: `ecdf8f5d5f2900e347e246c9d10317749f20e19f` (`main`).

- URL atual preservada: `https://leothaylor.github.io/manual-basico-APS360TikTok/`
- URL futura: `https://aps360.rotinaacs.com.br/`
- Arquivo inativo: `CNAME.pending`
- Branch local de preparação: `prep/domain-migration-20260806`

## Ativação autorizada

1. Registrar evidência da URL e do checkout atuais.
2. Criar `aps360 CNAME leothaylor.github.io` no DNS.
3. Renomear `CNAME.pending` para `CNAME` no commit de ativação.
4. Configurar o domínio no GitHub Pages e aguardar HTTPS.
5. Validar GA4 `G-926XGX9HB2`, Clarity `vxesptwfqj`, eventos e checkout Hotmart.

## Riscos antes do merge

- O repasse atual copia toda a query string para a Hotmart, sem lista permitida.
- Um parâmetro já existente no checkout pode ser repetido pela query de entrada.
- Não há Meta Pixel físico no código.

## Rollback

Remover somente o CNAME novo, restaurar canonical/OG para a URL do GitHub Pages e confirmar GA4, Clarity e checkout na URL histórica.
