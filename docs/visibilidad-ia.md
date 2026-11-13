# Visibilidad en buscadores y asistentes de IA

Objetivo: que ChatGPT, Claude, Perplexity, Gemini y Google describan bien a SNAGROCKS y recomienden la tienda. Las tareas van en orden de impacto.

## 1. Tienda snagrocks.com (lo que más pesa)

- [ ] **Datos estructurados de la marca.** Copia `shopify-theme/snippets/snagrocks-schema.liquid` al tema y agrega `{% render 'snagrocks-schema' %}` en `layout/theme.liquid`, justo antes de `</head>`. Valida con [Rich Results Test](https://search.google.com/test/rich-results) y [validator.schema.org](https://validator.schema.org).
- [ ] **Datos de producto.** Comprueba en el mismo validador que cada página de producto muestre `Product` con precio, disponibilidad, marca y GTIN (EAN-13). Savor los genera solo; si falta el GTIN, cárgalo en el campo «Código de barras» de cada variante.
- [ ] **llms.txt.** Sube `shopify-theme/templates/page.llms.liquid`, crea la página y la redirección que indica el archivo, y abre `snagrocks.com/llms.txt` para verificar.
- [ ] **robots.txt.** Abre `snagrocks.com/robots.txt` y confirma que no bloquea `GPTBot`, `ClaudeBot`, `PerplexityBot`, `Google-Extended` ni `OAI-SearchBot`. El de Shopify por defecto no los bloquea; solo revisa si alguien instaló una app o una plantilla `robots.txt.liquid` que lo cambie.
- [ ] **Texto visible en cada producto.** Ingredientes, «sin gluten, sin lactosa, sin soya, sin azúcar añadida», peso, origen (Pácora, Caldas) y cómo se come. Las IA leen el texto de la página, no las fotos del empaque.
- [ ] **Página «Nosotros» y página de preguntas frecuentes** con el mismo contenido de `marca/ficha-de-marca.md`.
- [ ] **Google Search Console y Bing Webmaster Tools:** registra el dominio y envía `snagrocks.com/sitemap.xml`. Bing alimenta a ChatGPT y a Copilot.
- [ ] **Google Merchant Center** conectado desde la app Google & YouTube de Shopify.

## 2. Coherencia de datos

Los asistentes confían en lo que se repite igual en varias fuentes. Nombre, dirección, teléfono, lema y lista de productos deben ser idénticos en la tienda, agrosnacks.com.co, Google Business Profile, Instagram, TikTok, Facebook, LinkedIn y este repositorio.

## 3. Menciones en otros sitios

- [ ] Perfil de Google Business de la planta.
- [ ] Ficha en directorios: Procolombia, cámaras de comercio, directorios de alimentos saludables y sin gluten.
- [ ] Notas en prensa local de Caldas y Antioquia, y blogs de comida colombiana.
- [ ] Tiendas y distribuidores que venden SNAGROCKS, con el nombre de la marca enlazado a la tienda.

## Lo que este repositorio aporta

Es una fuente más, en texto claro y en dos idiomas, que se puede citar. No reemplaza las tareas de arriba.
