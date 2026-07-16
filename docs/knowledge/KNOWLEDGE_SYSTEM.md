# Knowledge Base

Reglas de estructura y mantenimiento de `knowledge/`.

## Estructura
Cada dominio (`market/`, `operations/`, `customers/`, `competitors/`, `automation/`, `ai/`,
`architecture/`, `product/`) contiene archivos `.md` independientes, uno por hallazgo o
tema cohesivo. Nada de archivos "cajón de sastre".

## Ciclo de vida de una entrada
1. Se crea a partir de una nota validada en `research/` (ver `WORKFLOW.md`).
2. Se referencia en `knowledge/index.md`.
3. Se revisa periódicamente; si queda desactualizada, se actualiza o se mueve a `archive/`.

## Convención de nombres
`kebab-case`, descriptivo, sin fechas en el nombre del archivo (la fecha va en el
front-matter, no en el nombre).

## Front-matter mínimo por entrada
```yaml
title:
domain:
status: draft | validated | archived
confidence: alto | medio | bajo
sources:
last_updated:
```
