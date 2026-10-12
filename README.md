# Funil — 100 Receitas que Marcaram o MasterChef

Página de vendas modelada da página de empratamento do `site.materialseguro.shop`, com a mesma
ordem de blocos e a mesma paleta: barra vermelha, hero cinza-escuro, seções creme, CTA verde,
faixa vermelha com cronômetro, bônus, dois planos e garantia.

    node servidor.cjs     # http://localhost:4210

## Oferta (decidida pelo Heitor em 12/10/2026)

- **Plano Básico: R$ 10,00** (o preço falado nos 15 criativos). O botão abre um **popup** que oferece
  o Completo por **R$ 16,90**. Quem recusa vai para o checkout do Básico.
- **Plano Completo: R$ 24,90**, com 4 bônus:
  1. 30 Sobremesas do MasterChef (**ainda não existe, precisa ser produzido**)
  2. Lista de Compras das 100 Receitas (sai do conteúdo das receitas)
  3. Guia de Temperos do Chef (precisa ser produzido)
  4. 10 Cardápios Prontos para Receber (sai do conteúdo das receitas)
- **Back redirect** para `/promo`: as 100 receitas por **R$ 8,90**, com cronômetro de 5 min.
- **Sem depoimentos:** a seção entra quando houver pelo menos 3 prints reais de clientes.

## Falta antes de subir

- **Links da Wiapy:** cadastrar o produto, colocar os 4 links em `LINKS` no fim do `index.html` e o de R$ 8,90 em
  `LINK_PROMO` no `promo.html`. As UTMs da página são repassadas para o checkout.
- **Pixel da UTMify:** colar o script nos dois arquivos, no comentário `PIXEL / UTMIFY`.
- **Capas dos bônus:** hoje são feitas em CSS (cor + foto de um prato). Dá para trocar por capas geradas.
- **Sobremesas e temperos:** produzir antes de vender o Completo, ou trocar por bônus que já existam.
- Rodapé com e-mail de suporte e CNPJ, se houver.
