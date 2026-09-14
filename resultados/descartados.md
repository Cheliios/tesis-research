# Candidatos descartados

Registro de todo candidato que entró al pipeline (`papers/candidatos/` o
notas en `research/`) y fue descartado en cualquier etapa
(screening, verificación o análisis). Se mantiene por trazabilidad y para
evitar reprocesar el mismo candidato dos veces.

Formato por entrada:

```markdown
## [ID] — [Título]

- Línea: [Procesos | Inventarios]
- Etapa donde se descartó: [Screening | Verificación | Análisis]
- Motivo: [cita la regla exacta de CLAUDE.md o el hallazgo que lo descarta]
- Score al momento de descarte (si aplica): X/100
- Fecha: 
```

Motivos frecuentes esperados (no exhaustivo):

- Exclusión metodológica Lean/5S/Kaizen/Lean Six Sigma (Línea 1).
- Checklist genérico de orden/limpieza sin modelo de inventario real
  (Línea 2).
- Fuera de rango temporal (no 2021-2026) o idioma (no es/en).
- Score preliminar o final por debajo del umbral (60/100).
- Identidad bibliográfica no verificable (`NO VERIFICADO` en verificación
  central: título/autores/año/revista o universidad).
- Sector sin analogía operativa real con la MYPE del caso de estudio.

---

## L1-002 — Manufacturing Execution System Application within Manufacturing Small–Medium Enterprises towards Key Performance Indicators Development and Their Implementation in the Production Line

- Línea: Procesos
- Etapa donde se descartó: Screening
- Motivo: Score preliminar por debajo del umbral mínimo (39/100 < 40). Regla
  aplicada: CLAUDE.md sección 6 (sistema de scoring) según el criterio de
  decisión de `paper-screener.md` — "Score preliminar < 40 → DESCARTADO
  salvo justificación explícita muy fuerte (documentar por qué se mantiene
  pese al score bajo)". No se identificó justificación excepcionalmente
  fuerte: la correspondencia temática con Línea 1 (indicadores de procesos)
  es real, pero la base de evidencia es prácticamente nula — todas las
  fuentes probadas (MDPI directo x2, variante /htm, PDF y ficha del
  repositorio institucional cris.unibo.it, ResearchGate, con WebFetch y con
  curl con user-agent de navegador) devolvieron HTTP 403; el researcher no
  llegó a confirmar haber leído siquiera el abstract real (el resumen se
  reconstruyó de fragmentos agregados de WebSearch), y no hay ningún
  resultado cuantificable reportado ni verificable (0/20 en ese
  componente). Componentes del desglose: sector 10/20, problema-herramienta
  12/20, carácter aplicado 10/15, resultados cuantificables 0/20, calidad
  académica (preliminar) 2/10, actualidad 5/5, evidencia disponible 0/10.
  Ver detalle completo en `research/procesos/2024-mes-kpi-pyme-manufactura-italia.md`,
  sección `## Screening`.
- Score al momento de descarte (si aplica): 39/100
- Fecha: 2026-09-13

---

*(L2-001 y L1-001 fueron evaluados en la misma prueba controlada de
screening y quedaron SCREENED-IN — ver `resultados/matriz-articulos.csv` y
la sección `## Screening` en sus respectivos archivos de `research/`; no se
registran aquí por no haber sido descartados.)*
