# Peça 2 · ELEGANCE PREMIUM · base Tipo X · v4 — PROVA, 17/11/2026

**APROVADA pelo Rafael em 17/11/2026. PDFs de impressão gerados** (CMYK FOGRA39, texto e âncoras em curvas, traços de corte). Nada foi publicado nem enviado.

## PDFs de impressão
| Arquivo | Tamanho | O que é |
|---|---|---|
| `impressao-tampa-elegance-tipo-x.pdf` | 12,3 MB | Folha 95 x 95 mm, corte Ø 89,1. Imagem a 684 dpi. A borda e a folga pretas continuam pretas até a sangria. 84 peças em vetor (textos, filetes, estrela e a âncora do claim) |
| `impressao-tarja-elegance-tipo-x.pdf` | 12,5 MB | Folha 196 x 23 mm, corte 190 x 17. Pergaminho 600 dpi, moldura 1500, rosas 2400-2800, placa 555, logo 2400. 931 peças em vetor (a âncora do claim incluída) |

**Pendências:** dados legais e gramatura "150 g" continuam **PROVISÓRIOS**. Falta a **prova impressa 1:1** antes da gráfica.

Refazer os PDFs: `node pedidos/elegance-premium/gerar-pdfs-elegance.js elegance`. O script não sobrescreve um PDF que já existe; para refazer de propósito, use `REFAZER_PDF=1`. A imagem sem texto do PDF (`tampa-elegance-tipo-x-pdf.png`) vem de `SO_PDF_PNG=1 BASE=tipo-x-v4 node pedidos/elegance-premium/gerar-tampa-elegance.js`, que não regrava a prova aprovada. A conferência mostrou que a tampa com texto refeita difere da aprovada no máximo em 1/255, só arredondamento.

---
Histórico da prova (antes da aprovação):

## O que mudou em relação à v3
1. **Âncora no lugar do losango** nos claims: na tampa, "VITAMINA B5 ⚓ B7"; na tarja, "B5 ⚓ B7".
   - É o mesmo desenho da âncora de "FIXAÇÃO QUE NÃO SOLTA" (`gerar-tampa.js`), feito em traço vetorial arredondado. Não usa fonte de símbolos.
   - A altura é 1,2 vez a das maiúsculas, centrada nelas, com espaço igual dos dois lados.
   - Tampa: âncora dourada, com o contorno escuro fino dos textos reduzido à metade, para a argola não fechar, e a mesma sombra curta centralizada.
   - Tarja: âncora verde-escura #0B3B2E com o contorno marrom #8A6A2A dos claims.
2. **"PASTA MODELADORA" voltou.**
   - Tampa: entra no lugar de "MODELADOR", entre os filetes ondulados, com a mesma cor e o mesmo contorno, espaçamento menor e filetes menores e simétricos. Fica longe das âncoras.
   - Tarja: sob o logo, na placa verde (como no Tipo X original), e depois, em letra menor, "ELEGANCE PREMIUM · ROTA EVOLUÇÃO" e o "150 g". Tudo dentro da placa.
   - **Menor letra visível da tarja: 0,88 mm**, em "ELEGANCE PREMIUM · ROTA EVOLUÇÃO". O texto legal tem 1,21 mm.

Continua igual: arco redondo sem deformar, borda preta, miolo preto do Tipo X, contorno marrom nos claims verdes, texto legal e rosas-dos-ventos livres.

## Precisa de confirmação do cliente
- **Gramatura "150 g"**: provisória.
- **Dados legais: PROVISÓRIOS**, copiados do Pistache antigo (Anvisa, EAN, composição, fabricante, SAC).
- Sem aroma.

## Como refazer (Git Bash, na pasta `rotulo-vetorizador`)
```
BASE=tipo-x-v4 node pedidos/elegance-premium/gerar-tampa-elegance.js
BASE=tipo-x-v4 node pedidos/elegance-premium/gerar-tarja-elegance-tipo-x.js
BASE=tipo-x-v4 node pedidos/elegance-premium/montar-painel-tipo-x-v2.js
```
`painel-prova.jpg`: a v4 ao lado da v3, com a tarja v4 embaixo.
