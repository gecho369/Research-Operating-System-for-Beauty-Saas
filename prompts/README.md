# Prompts

Librería de prompts numerados que ejecutan cada fase del sistema de investigación.
Se usan en orden (01 → 10), aunque no es obligatorio completarlos linealmente.

| # | Archivo | Dominio |
|---|---|---|
| 01 | `01-market.md` | Mercado |
| 02 | `02-operations.md` | Operación del sector |
| 03 | `03-customers.md` | Clientes |
| 04 | `04-competitors.md` | Competidores |
| 05 | `05-automation.md` | Automatización |
| 06 | `06-ai.md` | IA aplicada |
| 07 | `07-architecture.md` | Arquitectura técnica |
| 08 | `08-product.md` | Producto |
| 09 | `09-synthesis.md` | Síntesis cross-dominio |
| 10 | `10-mvp.md` | Definición de MVP |

> Nota: la numeración 02-09 es una propuesta inicial alineada con las subcarpetas de
> `knowledge/`; ajustar libremente el nombre/orden según convenga.

## Formato de cada prompt
Cada archivo sigue esta estructura: Objetivo, Contexto necesario, Prompt, Formato de
salida esperado, Dónde guardar el resultado.
