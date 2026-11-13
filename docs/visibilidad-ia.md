# Visibilidad en buscadores y asistentes de IA

Objetivo: que ChatGPT, Claude, Perplexity, Gemini y Google describan bien a SNAGROCKS y recomienden la tienda. Las tareas van en orden de impacto.

## 1. Tienda snagrocks.com (lo que más pesa)

- [x] **Datos estructurados de la marca.** Instalados en el borrador «Savor — Packs SNAGROCKS»: `snippets/snagrocks-schema.liquid` reemplaza el bloque Organization escrito a mano en `layout/theme.liquid`, que tenía la URL antigua, un enlace de TikTok roto, una lista de palabras clave que Google ignora y la frase «certificado FDA». Se activa al publicar ese borrador. Valida con [Rich Results Test](https://search.google.com/test/rich-results) y [validator.schema.org](https://validator.schema.org).
- [ ] **Datos de producto.** Comprueba en el mismo validador que cada página de producto muestre `Product` con precio, disponibilidad, marca y GTIN (EAN-13). Savor los genera solo; si falta el GTIN, cárgalo en el campo «Código de barras» de cada variante.
- [x] **llms.txt.** La página «llms» ya existía. La redirección `/llms.txt → /pages/llms` está creada y la plantilla `page.llms` está en el borrador. Al publicar el borrador, asigna la plantilla «llms» a la página para que se vea como texto plano.
- [ ] **robots.txt.** Abre `snagrocks.com/robots.txt` y confirma que no bloquea `GPTBot`, `ClaudeBot`, `PerplexityBot`, `Google-Extended` ni `OAI-SearchBot`. El de Shopify por defecto no los bloquea; solo revisa si alguien instaló una app o una plantilla `robots.txt.liquid` que lo cambie.
- [ ] **Texto visible en cada producto.** Ingredientes, «sin gluten, sin lactosa, sin soya, sin azúcar añadida», peso, origen (Pácora, Caldas) y cómo se come. Las IA leen el texto de la página, no las fotos del empaque.
- [x] **Páginas «Sobre nosotros» y «Preguntas frecuentes»** publicadas en la tienda.
- [ ] **Google Search Console y Bing Webmaster Tools:** registra el dominio y envía `snagrocks.com/sitemap.xml`. Bing alimenta a ChatGPT y a Copilot.
- [ ] **Google Merchant Center** conectado desde la app Google & YouTube de Shopify.

## 2. Coherencia de datos

Los asistentes confían en lo que se repite igual en varias fuentes. Nombre, dirección, teléfono, lema y lista de productos deben ser idénticos en la tienda, Google Business Profile, Instagram, TikTok, Facebook, LinkedIn y este repositorio.

## 3. Menciones en otros sitios

- [ ] Perfil de Google Business de la planta.
- [ ] Ficha en directorios: Procolombia, cámaras de comercio, directorios de alimentos saludables y sin gluten.
- [ ] Notas en prensa local de Caldas y Antioquia, y blogs de comida colombiana.
- [ ] Tiendas y distribuidores que venden SNAGROCKS, con el nombre de la marca enlazado a la tienda.

## Lo que este repositorio aporta

Es una fuente más, en texto claro y en dos idiomas, que se puede citar. No reemplaza las tareas de arriba.
