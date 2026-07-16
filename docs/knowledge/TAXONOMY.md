# Taxonomía

Define qué entra en cada dominio de `knowledge/` y de `prompts/`.

| Dominio | Qué incluye | Qué NO incluye |
|---|---|---|
| `market/` | Tamaño de mercado, tendencias, regulación, segmentos | Competidores puntuales (va en `competitors/`) |
| `operations/` | Cómo operan hoy los negocios del sector (salones, clínicas, etc.) | Estrategia de producto propio |
| `customers/` | Perfiles, jobs-to-be-done, dolores, comportamiento de compra | Datos de mercado agregado |
| `competitors/` | Jugadores existentes, su propuesta de valor, precios, gaps | Tendencias de mercado generales |
| `automation/` | Procesos automatizables del sector, herramientas existentes | Arquitectura técnica propia |
| `ai/` | Casos de uso de IA aplicables al sector, límites y riesgos | Automatización no basada en IA |
| `architecture/` | Decisiones técnicas y de arquitectura del propio producto | Investigación de mercado |
| `product/` | Conocimiento que informa directamente features o el modelo de producto | Estrategia (va en `docs/product/`) |

Cada archivo en `knowledge/<dominio>/` debe poder clasificarse sin ambigüedad en una única
fila de esta tabla. Si un hallazgo cruza dos dominios, se documenta en el dominio principal
y se referencia cruzado desde el otro.
