# Scorpions Kids

Projetos técnicos **exclusivos da Scorpions Kids** (loja virtual Yampi — scorpionskids.com.br).
Não colocar aqui nada da Scorpions Marketing e Eventos.

| Projeto | O que faz | Onde roda |
| --- | --- | --- |
| `yampi-mcp/` | Conector que liga a loja Yampi da Scorpions Kids ao Claude: consulta pedidos, produtos, clientes, carrinhos abandonados e cupons; cria e edita produtos, preço, estoque, cupons e ofertas. **Não cancela pedidos, não estorna e não troca gateway de pagamento.** | Cloudflare Workers (`yampi-mcp`), credenciais criptografadas no KV `yampi-mcp-OAUTH_KV` |

Origem do `yampi-mcp`: cópia revisada do projeto aberto https://github.com/Eduardo-Orsi/yampi-mcp (licença MIT).

## site-scripts/
Scripts para colar no painel da loja Yampi da Scorpions Kids (não usar em sites da Scorpions Mkt e Eventos).
- `barra-instagram.html` — barra flutuante "Siga-nos no Instagram @scorpionskidss". Aparece após rolar a página, some por 7 dias ao fechar, não aparece no carrinho/checkout e envia o evento `instagram_bar` ao dataLayer (GTM/GA4).
