# Peça 2 · ELEGANCE PREMIUM · TARJA v5 (sangria preta) — 17/11/2026

Nada foi publicado nem enviado. A **tampa não mudou**: continua a da v4 (`../base-tipo-x-v4/`, PNG e PDF aprovados).

## O que mudou em relação à v4 (só a tarja)
- A **sangria** (a faixa de 3 mm fora do corte 190 x 17 mm) agora é **PRETA #000**, porque o pote é preto. Na v4 era pergaminho esticado.
- É uma camada vetorial por cima do pergaminho: a folha 196 x 23 menos o retângulo do corte (x 3, y 3, 190 x 17).
- **Dentro do corte nada muda.** Pergaminho (inclusive os 0,5 mm entre a moldura e o corte), moldura, rosas-dos-ventos, placa, logo e textos estão exatamente como aprovados.
- O PNG do corte (7600 x 680) foi comparado com o da v4: **idêntico, pixel a pixel**.

## Arquivos
| Arquivo | O que é |
|---|---|
| `impressao-tarja-elegance-tipo-x.pdf` | **PDF de impressão (12,5 MB)**: folha 196 x 23 mm com sangria preta, corte 190 x 17, CMYK FOGRA39, texto e âncora em curvas, traços de corte. Imagens: pergaminho 600 dpi, moldura 1500, rosas 2400-2800, placa 555, logo 2400 |
| `tarja-elegance-tipo-x.svg` | Folha inteira com a sangria preta (vetor + imagens embutidas) |
| `tarja-elegance-tipo-x.png` | Corte 190 x 17 a 40 px/mm (igual à v4) |
| `tarja-elegance-tipo-x-textos.json` | Textos e posições (com `sangria_preta: true`) |
| `prova-sangria.jpg` | Folha inteira do PDF renderizado (sangria preta) acima da v4 |

## Conferência
O PDF foi renderizado com PyMuPDF (`ferramentas/leitor-pdf`). Os cantos do corte, ampliados a 2400 dpi, mostram o preto limpo e contínuo, sem fresta nem franja: o pergaminho termina exatamente na linha de corte. A preta passa 0,1 mm da folha por fora, para nenhum fio de pergaminho aparecer na borda.

## Para a gráfica (Elegance Premium)
- **Tampa:** `../base-tipo-x-v4/impressao-tampa-elegance-tipo-x.pdf`
- **Tarja:** `impressao-tarja-elegance-tipo-x.pdf` (esta pasta, v5)

**Pendências:** dados legais e gramatura "150 g" continuam **PROVISÓRIOS**. Falta a **prova impressa 1:1**.

## Como refazer (Git Bash, na pasta `rotulo-vetorizador`)
```
BASE=tipo-x-v5 node pedidos/elegance-premium/gerar-tarja-elegance-tipo-x.js
REFAZER_PDF=1 node pedidos/elegance-premium/gerar-pdfs-elegance.js tarja-v5
```
