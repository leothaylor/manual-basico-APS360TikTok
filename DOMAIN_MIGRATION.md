# Preparação de domínio — Manual Básico APS 360

Estado-base: `ecdf8f5d5f2900e347e246c9d10317749f20e19f` (`main`).

- URL atual preservada: `https://leothaylor.github.io/manual-basico-APS360TikTok/`
- URL futura: `https://aps360.rotinaacs.com.br/`
- Arquivo de ativação: `CNAME`
- Branch local de preparação: `prep/domain-migration-20260806`
- Ativação autorizada em: `2026-08-06`

## Ativação autorizada

1. Registrar evidência da URL e do checkout atuais.
2. Criar `aps360 CNAME leothaylor.github.io` no DNS.
3. Publicar o arquivo `CNAME` no commit de ativação.
4. Configurar o domínio no GitHub Pages e aguardar HTTPS.
5. Validar GA4 `G-926XGX9HB2`, Clarity `vxesptwfqj`, eventos e checkout Hotmart.

## Correções incluídas na ativação

- O repasse para a Hotmart usa lista permitida de parâmetros de atribuição.
- `checkoutMode=10` permanece fixo e não pode ser sobrescrito pela URL de entrada.
- O valor do evento `begin_checkout` foi alinhado ao preço exibido de R$ 24,90.
- Não há Meta Pixel físico no código.

## Rollback

Remover somente o CNAME novo, restaurar canonical/OG para a URL do GitHub Pages e confirmar GA4, Clarity e checkout na URL histórica.
