# IALAP

Repositorio operativo de **IA, LA PREGUNTA, PRÁCTICA**.

## Estado del proyecto

- PROT-001 · Diagrama lógico: construido, pendiente de consolidación canónica.
- PROT-002 · Interfaz mínima v0.3-DRAFT: construido y corregido tras CRIT C03 y C05.
- Persistencia HTTP nativa: pendiente de ejecución C08 en GitHub Actions.
- PROT-003: no iniciado.
- Nomenclatura IALP / IALAP / SRG: provisional hasta decisión canónica.

## Ejecución C08

La infraestructura de prueba está disponible en:

- Workflow: `.github/workflows/c08-persistencia-http.yml`
- Instrucciones: `C08_RUNBOOK.md`
- SHA-256 esperado: `C08_EXPECTED_SHA256.txt`
- Rama de ejecución: `c08-persistencia-http`

El paquete de entrada debe situarse sin renombrar en:

`input/PROT-002_InterfazMinima_IALP_v0.3-DRAFT.zip`

El workflow verifica la integridad del ZIP, ejecuta Chromium bajo HTTP, comprueba la persistencia de `localStorage` después de recargar la misma URL, valida HANDOFF, OFF, migración y reset, y publica logs y resultados JSON.

## Restricción de continuidad

PROT-003 permanece bloqueado hasta que C08 termine con resultado verificable y se emita el siguiente dictamen CRIT.
