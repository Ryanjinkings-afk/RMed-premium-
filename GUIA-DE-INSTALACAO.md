# RMed — Base funcional restaurada

Esta versão retoma a arquitetura monolítica aprovada: CSS e JavaScript permanecem incorporados no `index.html`.

## Publicação no GitHub Pages

1. Extraia o ZIP.
2. Entre na pasta `RMed_BASE_FUNCIONAL`.
3. Envie o conteúdo dessa pasta diretamente para a raiz da branch `main`.
4. Substitua os arquivos existentes quando o GitHub solicitar.
5. Faça o commit.
6. Aguarde a publicação do GitHub Pages.

Arquivos esperados na raiz:
- `index.html`
- `manifest.webmanifest`
- `sw.js`
- `logo.svg`
- `icon-192.png`
- `icon-512.webp`

Não há pastas `src/`, nem dependências externas de CSS ou JavaScript para a interface principal.

Após publicar, feche a aba antiga do aplicativo, abra novamente o endereço e recarregue para atualizar o cache.
