# gbp-assets — percha pública de tarjetas de GBP

Hosting de las tarjetas de marca que acompañan las publicaciones de Google
Business Profile de los clientes de Rigol&Co. La API de GBP solo acepta
imágenes por URL pública y **las copia a su CDN al publicar**: este repo es
la percha temporal de la que Google copia, para no tener que hacer PR +
deploy en la web de cada cliente por cada tarjeta (decisión del operador,
2026-08-26).

- Un directorio por cliente (`cervel/`, `congenius/`, `rigolco/`).
- URL pública: `https://tonrigol-dot.github.io/gbp-assets/<cliente>/<archivo>.png`
- Los PNG se generan con `gbp-agent/scripts/gbp-cards/` y se versionan
  también en `gbp-agent/clients/<slug>/gbp-media/` (esa sigue siendo la
  copia de registro).
- Las tarjetas publicadas ANTES del 2026-08-26 se sirven desde las webs de
  los clientes y ahí se quedan: Google ya tiene su copia.
