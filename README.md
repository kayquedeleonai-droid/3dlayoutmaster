# 3D Layout Master · blocking playblast (flamingos)

O app inteiro é `public/index.html` (Three.js e mp4-muxer vêm de CDN; não há build).

## Publicação na Cloudflare (Workers com Git)

- `wrangler.jsonc` diz para a Cloudflare servir a pasta `public/` como site estático.
- Em **Workers & Pages → 3dlayoutmaster → Settings → Build**: comando de build **vazio**,
  comando de deploy `npx wrangler deploy`, diretório raiz `/`.
- O `name` no `wrangler.jsonc` precisa ser igual ao nome do Worker no painel.
- Cada push na branch `main` publica de novo.

## Rodar no computador

`npx wrangler dev` (ou `python3 -m http.server` dentro de `public/`).
