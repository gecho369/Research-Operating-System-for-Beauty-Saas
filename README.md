# Research Operating System for Beauty SaaS

Sistema operativo de investigación para construir un SaaS en el sector belleza/wellness
basado en evidencia: un proceso repetible para investigar mercado, operación, clientes,
competencia y tecnología, y convertir esos hallazgos en una base de conocimiento
estructurada que alimenta decisiones de producto.

## Cómo está organizado

| Carpeta | Qué contiene | Naturaleza |
|---|---|---|
| `docs/foundation/` | Visión, misión, alcance y principios del sistema | Estable, cambia poco |
| `docs/research/` | Cómo se investiga: workflow, metodología, criterios de fuentes | Metodología |
| `docs/knowledge/` | Reglas de la base de conocimiento: estructura, estilo, taxonomía | Metodología |
| `docs/product/` | Modelo de dominio y estrategia de producto | Producto |
| `prompts/` | Librería de prompts numerados para ejecutar cada fase de investigación | Herramientas |
| `research/` | Notas de investigación en bruto / borradores, sin curar | Trabajo en progreso |
| `knowledge/` | Base de conocimiento curada, organizada por dominio | Output final |
| `templates/` | Plantillas para notas de investigación, entradas de conocimiento y decisiones | Herramientas |
| `archive/` | Documentos deprecados o reemplazados, conservados por trazabilidad | Histórico |

## Flujo de trabajo (resumen)

1. Se ejecuta un prompt de `prompts/` (en orden, 01 a 10) contra la fuente correspondiente.
2. El resultado bruto se guarda como nota en `research/` usando `templates/research.md`.
3. Cuando la nota está validada, se destila en una entrada curada dentro de `knowledge/<dominio>/`
   usando `templates/knowledge.md`, y se referencia en `knowledge/index.md`.
4. Las decisiones de producto que se derivan del conocimiento acumulado se documentan con
   `templates/decision.md`.
5. Lo que queda obsoleto se mueve a `archive/` en lugar de borrarse.

Ver `docs/research/WORKFLOW.md` para el detalle paso a paso y `docs/research/RESEARCH_SYSTEM.md`
para la arquitectura completa del sistema.

## Punto de partida recomendado

1. `docs/foundation/FOUNDATION.md`
2. `docs/foundation/PRINCIPLES.md`
3. `docs/research/RESEARCH_SYSTEM.md`
4. `prompts/README.md`
