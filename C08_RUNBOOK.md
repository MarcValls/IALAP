# C08 · Persistencia HTTP nativa

Rama de ejecución: `c08-persistencia-http`

## Entrada inmutable

Subir sin renombrar:

`input/PROT-002_InterfazMinima_IALP_v0.3-DRAFT.zip`

SHA-256 exigido:

`f4e2f464f864f5b152eaf7c214ff1e03934773a9660bfa252ab59e9696538956`

La subida activa automáticamente `.github/workflows/c08-persistencia-http.yml`.

## Comprobaciones

1. Integridad del ZIP.
2. Smoke test.
3. Regresión adversarial.
4. Manifiesto SHA-256.
5. Servidor HTTP real.
6. Chromium real.
7. Escritura en `localStorage`.
8. Recarga de la misma URL.
9. Recuperación exacta del estado.
10. HANDOFF y OFF tras recarga.
11. Migración y reset.
12. Ausencia de modificaciones en el árbol de PROT-002.

## Salida

El workflow publica el artefacto:

`IALP-C08-persistencia-http-<run_id>`

Incluye logs, JSON de resultado, diferencia no destructiva y resumen C08.

PROT-002 no se modifica. PROT-003 no se inicia.
