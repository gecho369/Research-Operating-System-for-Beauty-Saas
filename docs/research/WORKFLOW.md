# Workflow de investigación

Flujo paso a paso desde una pregunta de investigación hasta una entrada validada en la
base de conocimiento.

## 1. Definir la pregunta
Qué se quiere saber y por qué importa para el producto.

## 2. Elegir el prompt
Seleccionar el prompt correspondiente en `prompts/` (01 a 10) según el dominio.

## 3. Ejecutar y capturar
Correr el prompt contra la(s) fuente(s), y guardar el resultado sin editar en `research/`
usando `templates/research.md`.

## 4. Validar
Contrastar el hallazgo con al menos una fuente adicional cuando sea posible. Marcar
explícitamente el nivel de confianza (alto / medio / bajo).

## 5. Destilar a conocimiento
Convertir la nota validada en una entrada curada en `knowledge/<dominio>/` con
`templates/knowledge.md`, y actualizar `knowledge/index.md`.

## 6. Actualizar producto
Si el hallazgo afecta al dominio o la estrategia de producto, reflejarlo en
`docs/product/DOMAIN_MODEL.md` o `docs/product/PRODUCT_STRATEGY.md`, y registrar la
decisión con `templates/decision.md` si corresponde.

## 7. Archivar lo obsoleto
Cuando una entrada de conocimiento queda reemplazada, se mueve a `archive/` con una nota
de por qué y por qué la reemplaza.
