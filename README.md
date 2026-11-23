# Plano 100 dias TJ-SP

Plano de estudos para Escrevente Técnico Judiciário do TJ-SP (Vunesp, prova em 14/03/2027). São 2 h por dia, de 22/11/2026 a 13/03/2027.

O app funciona no navegador e pode ser instalado no celular ou no tablet. Depois de aberto uma vez, funciona sem internet. O progresso fica salvo no aparelho. Para levar para outro aparelho, use "App, backup e outros aparelhos" e exporte o backup ou o código de progresso.

## Arquivos

- `index.html`: o plano (progresso, revisões de 7 e 30 dias, edital item por item)
- `questoes.html`: as questões Vunesp do Gran de um bloco, por artigo. Abre pelo botão "Abrir página de questões deste bloco" no plano, ou sem parâmetro para ver todos os blocos
- `questoes-data.js`: a lista de questões por bloco, usada pelas duas páginas
- `manifest.webmanifest` e `sw.js`: instalação e uso offline
- `icon-*.png` e `apple-touch-icon.png`: ícones

## Publicar no GitHub Pages

1. Em Settings > Pages, escolha "Deploy from a branch".
2. Branch `main`, pasta `/ (root)`. Salve.
3. Em um ou dois minutos o app abre em `https://SEU-USUARIO.github.io/tjsptudyplan/`.

O service worker só roda em https. No GitHub Pages isso já vem pronto.

Ao publicar uma versão nova do `index.html`, troque o nome do cache em `sw.js` (`plano-tjsp-100d-v1` para `v2`) para os aparelhos baixarem a atualização.
