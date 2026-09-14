# Proyecto: Antecedentes de Tesis — Gestión de Procesos e Inventarios en MYPE Recicladora

Este archivo contiene las reglas **permanentes** del proyecto. Todo subagente y
toda sesión de Claude Code que trabaje en este directorio debe respetarlas.
No se contradicen entre sí; si una instrucción puntual del usuario pareciera
chocar con una regla de integridad académica (sección 5), esa regla de
integridad prevalece salvo que el usuario la modifique explícitamente aquí.

## 1. Contexto del caso de estudio

MYPE del sector reciclaje dedicada a compra, procesamiento, almacenamiento y
comercialización de **botellas de plástico PET** y **cartón**.

Flujo general:

```
Recepción/compra → pesaje → clasificación → procesamiento → almacenamiento → venta
```

- **PET:** selección → picado/triturado → almacenamiento → comercialización.
- **Cartón:** selección → prensado/compactado → formación de fardos →
  almacenamiento → comercialización.

La empresa maneja inventario tanto **antes** como **después** del procesamiento.

Problemas potenciales observados (sirven para juzgar similitud/relevancia de
antecedentes, no son un checklist a completar en cada paper):

- falta de control de materiales
- diferencias entre inventario físico y registrado
- errores de registro
- información desactualizada
- desorganización
- acumulación de PET/cartón
- dificultad para conocer entradas y salidas
- falta de procedimientos estandarizados
- tiempos elevados
- falta de indicadores
- dificultad para controlar material antes/después del procesamiento
- desconocimiento del stock realmente disponible para venta

## 2. Las dos líneas de investigación

### Línea 1 — Gestión de Procesos

Temas de interés: gestión por procesos, BPM, modelamiento y análisis de
procesos, estandarización, diagramas de procesos, mapeo y caracterización de
procesos, indicadores de procesos, rediseño de procesos, optimización de
procesos, mejora de métodos de trabajo, medición de tiempos, productividad,
simulación de procesos orientada a mejora, metodologías académicamente
aceptadas de gestión de procesos.

Prioridad de aplicación (de mayor a menor relevancia):

1. reciclaje de PET/cartón
2. empresas recicladoras
3. procesamiento de plástico
4. residuos sólidos / recuperación de materiales
5. empresas con operaciones físicamente comparables
6. MYPEs o empresas con problemas operacionales equivalentes

**EXCLUSIÓN ABSOLUTA para esta línea:** Lean Manufacturing, Lean Management,
5S, Kaizen, Lean Six Sigma. Un trabajo cuya intervención principal dependa de
estas metodologías **no puede** ser antecedente de Gestión de Procesos,
aunque reporte buenos resultados. Esto se aplica de forma automática y no es
negociable por un subagente individual.

### Línea 2 — Control / Gestión de Inventarios

Temas de interés: clasificación ABC, EOQ, punto de pedido, stock de
seguridad, inventario mínimo/máximo, revisión periódica, revisión continua,
pronóstico de demanda, control de entradas y salidas, exactitud de
inventarios, inventarios cíclicos, gestión de almacenes, Kardex,
trazabilidad, sistemas de registro, modelos de gestión de inventarios,
indicadores de inventario, optimización de inventarios.

Prioridad de aplicación (de mayor a menor relevancia):

1. reciclaje/PET/cartón
2. residuos sólidos
3. almacenes de materiales reciclables
4. empresas de transformación de materiales
5. MYPEs
6. empresas con flujos de inventario comparables

No tiene una exclusión metodológica equivalente a Lean, pero un antecedente
cuya única intervención sea un checklist genérico de orden y limpieza (tipo
5S) debe tratarse igual que en la Línea 1: no cuenta como antecedente de
control/gestión de inventarios.

## 3. Tipo de evidencia buscada

**No priorizar literatura exclusivamente teórica.** Los antecedentes
principales deben ser investigaciones aplicadas que sigan aproximadamente:

```
PROBLEMA → HERRAMIENTA/MODELO → IMPLEMENTACIÓN → INDICADORES → RESULTADO
```

Priorizar especialmente resultados cuantificables: reducción de costos,
reducción de tiempos, incremento de productividad, incremento de eficiencia,
reducción de errores, incremento de exactitud del inventario, reducción de
pérdidas, reducción de inventario innecesario, mejora del nivel de
cumplimiento, mejora de indicadores operacionales.

**Nunca inventar porcentajes, resultados, muestras, DOI, autores, cuartiles,
indexaciones ni conclusiones.** Si un dato no está en la fuente, no existe
para efectos de este proyecto.

## 4. Criterios bibliográficos

- **Rango temporal:** 2021–2026 inclusive.
- **Idiomas:** inglés y español.
- **Objetivo:** al menos 15 antecedentes finales de alta calidad (calidad
  por encima de cantidad; nunca se rellena la cuota con fuentes débiles o
  inventadas).
- **Prioridad de indexación:** artículos indexados en Scopus o Web of
  Science.
- **Editoriales/plataformas de interés:** ScienceDirect, Springer, Emerald,
  Taylor & Francis, Wiley, MDPI, SciELO.
- **Para artículos científicos:** priorizar revistas Q1 o Q2.

  > **Importante:** aparecer en ScienceDirect, Springer, Emerald, Taylor &
  > Francis, Wiley, MDPI o SciELO **no implica** que la revista sea Q1/Q2.
  > El cuartil debe verificarse de forma independiente (p. ej. Scimago
  > Journal Rank, JCR) y debe registrarse explícitamente cuál fue la fuente
  > usada para verificarlo. Ver `reference-verifier.md`.

- **Tesis y repositorios universitarios:** se pueden usar, pero se
  clasifican explícitamente como **evidencia complementaria**, nunca como
  artículo Q1/Q2. Una tesis no recibe un cuartil ficticio.

## 5. Reglas de integridad académica (CRÍTICO)

Ningún candidato se convierte automáticamente en antecedente final. El flujo
obligatorio es:

```
DESCUBRIMIENTO → SCREENING → VERIFICACIÓN → ANÁLISIS → SELECCIÓN FINAL
```

- **Descubrimiento:** `process-researcher` / `inventory-researcher` buscan y
  proponen candidatos. Solo proponen, no aceptan ni rechazan definitivamente.
- **Screening:** `paper-screener` evalúa inclusión/exclusión y relevancia
  preliminar. Puede descartar candidatos claramente fuera de alcance
  (incluyendo cualquier caso Lean/5S/Kaizen/Lean Six Sigma en Línea 1), pero
  no puede *aprobar* un antecedente final por sí mismo.
- **Verificación:** `reference-verifier` confirma identidad bibliográfica
  (título, autores, año, revista/universidad, DOI, URL, indexación, cuartil
  y fuente de verificación del cuartil) antes de invertir esfuerzo en
  análisis profundo de contenido.
- **Análisis:** `paper-analyst` extrae metodología, contexto, indicadores y
  resultados **solo de fuentes ya verificadas o en proceso de verificación**,
  marcando explícitamente cualquier dato que no pueda confirmar.
- **Selección final:** es una decisión que toma el orquestador (la sesión
  principal de Claude Code) junto con el usuario, a partir del score de
  relevancia y el estado de verificación. **Ningún subagente individual
  tiene autoridad para declarar un artículo como antecedente final.**

Reglas adicionales, sin excepción:

- Si un dato no puede verificarse: marcarlo como `NO VERIFICADO` en la
  matriz y en cualquier nota, nunca omitirlo silenciosamente ni inventarlo.
- Si el texto completo no está disponible, no se afirman detalles
  metodológicos ni resultados que solo podrían conocerse leyendo el texto
  completo. Se documenta explícitamente qué partes provienen de abstract
  únicamente.
- Los resultados cuantitativos deben proceder del paper o de evidencia
  primaria consultable. Nunca se infieren ni se estiman.
- Nunca se fabrica una referencia para completar la cuota de 15 antecedentes.

## 6. Sistema de scoring de relevancia (0–100)

Sistema reproducible, aplicado por `paper-screener` (score preliminar) y
refinado por el orquestador tras el análisis y la verificación. Cualquier
subagente que asigne un score debe dejar por escrito el desglose, no solo el
número final.

| Componente | Puntos máx. | Criterio |
|---|---|---|
| Similitud de sector/contexto | 20 | 20 = PET/cartón/reciclaje directo · 15 = residuos sólidos/materiales reciclables · 10 = MYPE/manufactura físicamente comparable · 5 = industria genérica · 0 = sector irrelevante |
| Correspondencia problema–herramienta | 20 | Qué tan bien la herramienta/modelo usado responde a un problema análogo a los listados en la sección 1 |
| Carácter aplicado | 15 | 15 = implementado en empresa real · 10 = piloto/simulación con datos reales · 5 = propuesta no implementada · 0 = puramente teórico |
| Resultados cuantificables y verificables | 20 | 20 = antes/después con datos verificables en el texto · 10 = resultados parcialmente cuantificados · 5 = solo cualitativos · 0 = sin resultados |
| Calidad académica | 10 | 10 = Q1 verificado · 7 = Q2 verificado · 4 = Q3/Q4 verificado · 2 = tesis/repositorio o cuartil no verificable |
| Actualidad | 5 | 5 = 2024–2026 · 3 = 2022–2023 · 1 = 2021 |
| Disponibilidad de evidencia verificable | 10 | 10 = texto completo disponible · 3 = solo abstract/resumen · 0 = no disponible |

**Penalizaciones** (se restan sobre el subtotal anterior, pueden llevar el
score a 0; se aplican además de, no en lugar de, la tabla anterior):

- Contexto poco comparable (sector sin analogía operativa real): **-15**
- Ausencia de implementación real detrás de resultados reportados: **-10**
- Resultados no verificables (afirmados sin sustento localizable en el
  texto): **-15**
- Información bibliográfica dudosa (no se pudo verificar autor, año,
  revista o DOI): **-20**

**Exclusión directa (score = 0, descartado automáticamente, sin excepción):**
cualquier candidato de Línea 1 cuya intervención principal sea Lean
Manufacturing, Lean Management, 5S, Kaizen o Lean Six Sigma.

**Umbral orientativo de preselección:** score ≥ 60 **y** estado de
verificación `VERIFICADO` o `PARCIALMENTE VERIFICADO` (solo detalles
menores pendientes). Cruzar el umbral hace a un candidato elegible para
selección final; no lo convierte automáticamente en antecedente (ver
sección 5).

## 7. Estructura de archivos del proyecto

```
CLAUDE.md
.claude/agents/
  process-researcher.md
  inventory-researcher.md
  paper-screener.md
  paper-analyst.md
  reference-verifier.md
research/
  procesos/       ← notas de búsqueda y hallazgos crudos de Línea 1
  inventarios/    ← notas de búsqueda y hallazgos crudos de Línea 2
papers/
  candidatos/     ← candidatos aún no verificados/analizados (uno por archivo)
  seleccionados/  ← candidatos que pasaron verificación + análisis y están
                    listos para la decisión de selección final
resultados/
  matriz-articulos.csv   ← matriz maestra (ver plantilla, columnas fijas)
  antecedentes.md         ← antecedentes finales aprobados por el usuario
  descartados.md          ← candidatos descartados, con motivo
  verification-log.md     ← bitácora de verificación bibliográfica
```

Cada candidato en `papers/candidatos/` y `papers/seleccionados/` debe tener
un ID único y consistente con la columna `ID` de `matriz-articulos.csv`
(sugerido: `L1-001`, `L1-002`... para Línea 1 y `L2-001`, `L2-002`... para
Línea 2).

## 8. Flujo de orquestación esperado (referencia, no ejecutar todavía)

1. El orquestador lanza `process-researcher` y/o `inventory-researcher` para
   proponer candidatos → se guardan en `papers/candidatos/` + fila en
   `matriz-articulos.csv` con estado `DESCUBIERTO`.
2. `paper-screener` evalúa cada candidato, aplica inclusión/exclusión y
   score preliminar → actualiza estado a `SCREENED-IN` o mueve el motivo a
   `descartados.md` con estado `DESCARTADO`.
3. `reference-verifier` verifica identidad bibliográfica e indexación de los
   `SCREENED-IN` → actualiza estado a `VERIFICADO`,
   `PARCIALMENTE VERIFICADO` o `NO VERIFICADO`, registra la verificación en
   `verification-log.md`.
4. `paper-analyst` extrae metodología, indicadores y resultados de los
   candidatos verificados/parcialmente verificados → mueve el archivo a
   `papers/seleccionados/` si cumple el umbral de la sección 6, actualiza la
   matriz.
5. El orquestador presenta al usuario los candidatos que cruzan el umbral
   junto con su desglose de score y estado de verificación. **Solo el
   usuario, junto con el orquestador, decide qué entra a `antecedentes.md`
   como antecedente final.**

## 9. Regla operativa actual

**No se ejecuta ninguna búsqueda, verificación ni análisis hasta que el
usuario lo apruebe explícitamente.** Esta fase solo cubre arquitectura,
subagentes y plantillas.
