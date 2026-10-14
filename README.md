# S7N Booking — deploy en Vercel

## Subir (5 min)
1. Entra a https://vercel.com/new → "Deploy" → arrastra esta carpeta (o súbela a GitHub como `Gerryram/s7n-booking` e impórtala).
2. Framework: **Other**. Sin build command. Output: raíz.
3. Queda en `https://s7n.info` (si el nombre está tomado, Vercel te da otro).

## Dominio s7n.info
1. Vercel → Project → Settings → Domains → agrega `s7n.info` y `www.s7n.info` (que www redirija a s7n.info).
2. En el DNS de tu registrador:
   - `s7n.info` → registro **A** → `76.76.21.21`
   - `www` → registro **CNAME** → `cname.vercel-dns.com`
   - No borres los registros **MX** del correo booking@s7n.info.
3. Vercel emite el SSL solo en unos minutos. Los meta tags, sitemap y canonical ya apuntan a https://s7n.info.
