# Research System

Arquitectura del sistema de investigación: cómo se relacionan sus componentes.

## Componentes

- **Prompts (`prompts/`)**: unidades de trabajo repetibles. Cada prompt tiene un objetivo,
  una entrada esperada y un formato de salida.
- **Research (`research/`)**: capa de captura. Notas en bruto, fechadas, sin depurar.
- **Knowledge (`knowledge/`)**: capa curada. Solo entra lo validado, escrito según
  `WRITING_STANDARD.md` y clasificado según `TAXONOMY.md`.
- **Docs/product**: capa de decisión. Traduce conocimiento en modelo de dominio y estrategia.
- **Templates**: contratos de formato para que toda entrada sea consistente.
- **Archive**: capa histórica. Nada se elimina, se reclasifica.

## Diagrama de flujo (texto)

```
prompts/ ──ejecuta──> research/ ──valida y destila──> knowledge/ ──informa──> docs/product/
                                                              │
                                                              └──obsoleto──> archive/
```

## Dominios de conocimiento
Coinciden con las subcarpetas de `knowledge/`: market, operations, customers, competitors,
automation, ai, architecture, product. Ver `docs/knowledge/TAXONOMY.md` para el detalle de
qué entra en cada una.
