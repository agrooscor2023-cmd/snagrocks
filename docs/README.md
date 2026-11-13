# Guía de revisión

## Alcance

Estos archivos se exportaron del borrador de packs, sin modificar su código ni publicarlos en la tienda. No se realizaron pruebas funcionales como parte de esta exportación.

## Instalación y pruebas

1. Trabaja sobre una copia de respaldo del tema, nunca directamente en producción.
2. Conserva los archivos originales y compara los cambios con tu versión de Savor.
3. Copia primero `snippets/pack-picker.liquid`, después `blocks/variant-picker.liquid` y finalmente `sections/snagrocks-crunch.liquid`.
4. Prueba selección de variantes, disponibilidad, precio y producto añadido al carrito en móvil y escritorio.
5. Configura la sección Elige tu crunch con sus imágenes y enlaces; comprueba cada tarjeta.
6. Publica únicamente después de validar el resultado.

## Puntos pendientes del selector

- Se activa cuando existe la opción `Presentación`, pero recorre todas las opciones del producto. Prueba cuidadosamente productos con opciones adicionales.
- Toma como referencia el precio de la primera opción. Revisa que corresponda realmente a la unidad suelta.
- La etiqueta Mejor valor depende de que la última opción tenga ahorro, no de comparar todos los precios unitarios.
- El cálculo interpreta números en el nombre como cantidades: nombres como `Tarro 425 g` requieren revisión antes de utilizar los ahorros o precios unitarios.
- No utiliza el precio de comparación para calcular ahorro, pero eso no garantiza que otros componentes del tema no muestren ofertas.

## Convenciones de catálogo proporcionadas por la marca

- Imágenes: 1500 × 1200 px; frente principal y posterior secundaria.
- Títulos: `[Producto] [sabor] [peso] | SNAGROCKS`, conforme al empaque.
- SKU: `MARCA-PRODUCTO-CORTE-SABOR-EMPAQUE+PESO-ACEITE-MERCADO`.
- Ejemplo: `SNG-PLV-C-NAT-BT70-GP-N`.
- Cada variante lleva su EAN-13 junto al SKU.

## Publicación segura

Incluye únicamente estas personalizaciones y documentación. No añadas configuraciones privadas, credenciales, datos de clientes, pedidos, costos ni el tema completo.
