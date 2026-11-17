# Peça 1 · Pistache CREME MATTE · tampa com âncoras no claim — PROVA, 17/11/2026

**APROVADA pelo Rafael em 17/11/2026. PDF de impressão da tampa gerado.** Nada foi publicado nem enviado. A arte aprovada anterior (`saida/pistache-creme-matte-2026-11-17/`) **não foi alterada**.

## PDFs para a gráfica
- **Tampa (nova, com âncoras):** `impressao-tampa-pistache-creme-matte-ancora.pdf` (12,3 MB). Folha 95 x 95 mm, corte Ø 89,1, imagem a 684 dpi, CMYK FOGRA39. 87 peças em vetor (textos e as 2 âncoras de traço).
- **Tarja: use a que JÁ EXISTE**, `saida/pistache-creme-matte-2026-11-17/impressao-tarja-pistache-creme-matte.pdf` (26,1 MB). A tarja não mudou e não foi gerada outra.
- **Não use** a `impressao-tampa-pistache-creme-matte.pdf` da pasta antiga: é a versão com losangos.

**Pendências:** dados legais e gramatura continuam **PROVISÓRIOS**. Falta a **prova impressa 1:1** antes da gráfica.

Refazer o PDF: `node pedidos/elegance-premium/gerar-pdfs-elegance.js pistache`. O script não sobrescreve; para refazer de propósito, use `REFAZER_PDF=1`.

---
Histórico da prova:

## O que mudou
- **Tampa:** "VITAMINA D ⚓ B7 ⚓ QUERATINA". As duas âncoras entram no lugar dos losangos.
  - É o desenho da âncora de "FIXAÇÃO QUE NÃO SOLTA", em traço vetorial arredondado, dourado #F3CB62 (a cor do losango).
  - A altura é 1,2 vez a das maiúsculas, centrada nelas, com espaço igual dos dois lados.
  - O contorno escuro tem a metade da espessura do texto, para a argola não fechar, e a sombra é curta e centralizada.
  - Todo o resto da tampa é igual à aprovada.
- **Tarja:** não muda (usa "·"). O painel mostra a tarja aprovada.

## Arquivos
`tampa-pistache-creme-matte.png` (2400 px, 684 dpi, com texto) · `tampa-pistache-creme-matte-pdf.png` e `-base.png` (sem texto, para o PDF quando for aprovado) · `tampa-textos.json` · `prova-tampa.jpg` · `prova-lado-a-lado.jpg` (nova ao lado da aprovada, com a tarja aprovada embaixo).

## Como refazer (Git Bash, na pasta `rotulo-vetorizador`)
```
ANCORA=1 node pedidos/pistache/creme-matte/gerar-tampa-arco.js
node pedidos/pistache/creme-matte/montar-prova-ancora.js
```
Sem `ANCORA=1`, o script refaz a tampa aprovada (losangos) na pasta original, como antes.

Dados legais e gramatura continuam PROVISÓRIOS (ver o LEIA-ME da pasta aprovada).
