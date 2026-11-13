# SNAGROCKS · AGRO SNACKS del campo colombiano

**Ingredientes reales — Un crunch diferente.**

**SNAGROCKS** es una marca de snacks artesanales hechos con lo mejor del campo colombiano: plátano verde y maduro, yuca, batata, arracacha, taro y papa. Hace parte de la familia **AGRO SNACKS**, snacks del agro colombiano de **AGRO OSCOR S.A.S.**, con planta en Castilla, Pácora (Caldas).

🌐 Tienda en línea: [snagrocks.com](https://snagrocks.com)

---

## ¿Qué hay en este repositorio?

Documentación y recursos públicos de SNAGROCKS. Cada carpeta explica su propio alcance en su archivo `README.md`.

| Carpeta | Contenido |
|---|---|
| `shopify-theme/` | Personalizaciones del tema de la tienda (Savor): selector de packs por volumen y sección interactiva "Elige tu crunch". |
| `docs/` | Guías de uso: cómo instalar las personalizaciones y convenciones de catálogo. |

> El repositorio **no** contiene el tema completo de Shopify, solo los archivos que creamos o modificamos.

## Personalizaciones del tema

### Selector de packs (`snippets/pack-picker.liquid` + `blocks/variant-picker.liquid`)
- Se activa solo en productos que tienen la opción **"Presentación"** (por ejemplo: `1 bolsa`, `Pack x6`, `Pack x12`, `Pack x24`, o tamaños como `Tarro 425 g`).
- Muestra cada opción como tarjeta con precio, precio por unidad y ahorro, y marca el pack más grande como **"Mejor valor"**.
- El ahorro se calcula comparando con el precio de la unidad suelta. **No usa precio de oferta**, así que ningún producto aparece "en oferta" en la tienda.
- Detecta si el producto es bolsa o tarro para escribir "por bolsa" o "por tarro".

### Sección "Elige tu crunch" (`sections/snagrocks-crunch.liquid`)
- Tarjetas con foto de producto: en computador se expanden al pasar el mouse; en celular se deslizan con el dedo.
- Cada tarjeta se edita desde el editor de temas: foto, nombre, descripción corta, producto y texto del botón (máximo 6).

### Instalación
1. En Shopify: **Tienda online → Temas → … → Editar código** de una **copia** del tema (nunca del tema publicado).
2. Crea o reemplaza los archivos con el mismo nombre y ruta que tienen en `shopify-theme/`.
3. En el editor de temas, agrega la sección **"Elige tu crunch"** donde la quieras.
4. Revisa la vista previa en computador y celular antes de publicar.

## Convenciones del catálogo

- **Imágenes de producto:** 1500 × 1200 px. Principal = frente del empaque; secundaria = vista posterior.
- **Títulos:** `[Producto] [sabor] [peso] | SNAGROCKS`, igual a lo que dice el empaque.
- **SKU:** `MARCA-PRODUCTO-CORTE-SABOR-EMPAQUE+PESO-ACEITE-MERCADO`
  Ejemplo: `SNG-PLV-C-NAT-BT70-GP-N` → SNAGROCKS · plátano verde · chips · natural · bolsa transparente 70 g · girasol y palma · nacional.
- **Código de barras:** cada variante lleva su EAN-13 junto al SKU.

## Seguridad y privacidad

Nunca publiques en este repositorio:
- Contraseñas, tokens de acceso, llaves de API ni archivos `.env`.
- Datos de clientes, pedidos o facturas.
- Listas de precios por canal, costos, márgenes ni información comercial confidencial.

Revisa el contenido de cada archivo **y el historial de Git** antes de subirlo. Si una credencial quedó expuesta, revócala o cámbiala en el servicio que la emitió: borrar el archivo no la invalida.

## Marca y uso del contenido

Que este repositorio sea público **no** concede licencia para reutilizar su código, imágenes, textos, logotipos ni marcas. Revisa el archivo de licencia o aviso de cada recurso. SNAGROCKS y AGRO SNACKS son marcas de AGRO OSCOR S.A.S.

## Contacto

SNAGROCKS · AGRO SNACKS del campo colombiano · AGRO OSCOR S.A.S. · [snagrocks.com](https://snagrocks.com) · Instagram [@homemadesnackscol](https://instagram.com/homemadesnackscol)
