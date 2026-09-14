# Proyecto: Antecedentes de Tesis — Gestión de Procesos de Control de
# Inventarios en MYPE Recicladora (PET y Cartón)

Este archivo contiene las reglas **permanentes** del proyecto. Todo subagente
y toda sesión de Claude Code que trabaje en este directorio debe respetarlas.
Si una instrucción puntual del usuario pareciera chocar con una regla de
integridad académica (sección 14) o con una regla dura de consumo (sección
16), esas reglas prevalecen salvo que el usuario las modifique explícitamente
aquí.

> **Reconfiguración 2026-09-14:** este archivo reemplaza la versión anterior
> del proyecto (dos líneas independientes "Gestión de Procesos" / "Control de
> Inventarios"). El tema se unificó y la arquitectura se rediseñó para reducir
> drásticamente el consumo de Claude Pro tras el smoke test inicial. Los
> resultados de ese smoke test (`L1-001`, `L1-002`, `L2-001`) se conservan
> íntegros como evidencia histórica — ver sección 21.
>
> **Ajuste V3 (misma fecha, aprobado por el usuario):** se afinó el rol de
> `process-researcher` (sección 5), se recalibraron los umbrales de
> clasificación y se añadieron gates obligatorios de verificación para
> `ANTECEDENTE FUERTE` (sección 17). No se modificaron los datos del smoke
> test salvo un campo estructural de consistencia (sección 21).

## 1. Tema central de la tesis

Ingeniería Industrial. Eje principal:

**GESTIÓN DE PROCESOS DE CONTROL DE INVENTARIOS**

Caso de estudio: MYPE del sector reciclaje dedicada a compra, procesamiento,
almacenamiento y comercialización de **botellas de plástico PET** y
**cartón**.

Objetivo de la búsqueda bibliográfica: encontrar antecedentes que ayuden a
determinar qué herramientas, modelos, metodologías, sistemas e indicadores
son científicamente adecuados para mejorar el **proceso de control de
inventarios** de esta empresa. **No se asume todavía cuál será la solución
final de la tesis** — los antecedentes deben ayudar a justificar esa
decisión, no anticiparla.

## 2. Proceso real de la empresa

```
RECEPCIÓN/COMPRA → REGISTRO → CLASIFICACIÓN → PROCESAMIENTO → ALMACENAMIENTO → VENTA/SALIDA
```

- **PET:** recepción → clasificación → picado/triturado → almacenamiento →
  venta.
- **Cartón:** recepción → clasificación → prensado/compactado →
  almacenamiento → venta.

Existe **transformación física** del material. El control de inventarios no
se limita a compras y ventas: debe poder distinguir conceptualmente entre

- material recibido,
- material en procesamiento,
- material procesado,
- material almacenado,
- material vendido/despachado,
- inventario disponible.

Un antecedente es más valioso cuanto mejor ayude a modelar esta distinción,
no solo un balance simple de entradas menos salidas.

## 3. Problema real de la empresa

Actualmente **no existe un sistema formal y sistemático de control de
inventarios**. Problemas observados:

- entradas registradas manualmente;
- ausencia de registro sistemático de cuánto material ingresa;
- información de stock desactualizada o inexistente;
- desconocimiento preciso del cartón y del PET almacenados;
- ausencia de control sistemático de cuánto material se procesa;
- registros inadecuados de salidas/ventas;
- inventario no actualizado;
- dificultad para conocer el stock disponible en un momento determinado;
- poca trazabilidad entre recepción, procesamiento, almacenamiento y venta;
- información distribuida principalmente en registros manuales;
- decisiones de venta asociadas a necesidades de liquidez, no a
  planificación basada en inventario.

Preguntas que la empresa hoy no puede responder con precisión: ¿cuánto PET
tenemos?, ¿cuánto cartón tenemos?, ¿cuánto ingresó?, ¿cuánto se procesó?,
¿cuánto se vendió?, ¿cuánto queda disponible?, ¿cuánto tiempo permanece
almacenado?

**Este problema real (sección "A. Similitud del problema" del scoring, ver
sección 17) tiene el mayor peso individual al evaluar un candidato.**

## 4. Ecuación conceptual de referencia (no asumir que es la final)

La tesista considera, solo como punto de partida conceptual:

```
inventario inicial + entradas − salidas/procesamiento = inventario disponible
```

Pero por la transformación física de PET y cartón, la literatura puede
mostrar modelos mejores para distinguir:

```
materia prima/material recibido → material en proceso → producto/material
procesado → almacenamiento → salida/venta
```

La función de los antecedentes es ayudar a determinar el modelo correcto —
no confirmar la ecuación de arriba a priori.

## 5. Enfoque unificado: proceso de control de inventarios

**No tratar "gestión de procesos" e "inventarios" como dos investigaciones
independientes.** El eje de búsqueda es el **proceso de control de
inventarios** en sí mismo: inventory control process, inventory management
process, inventory process improvement/redesign/standardization, inventory
workflow, material flow control, inventory tracking/traceability, digital
inventory control, inventory information systems, stock control systems.

Un antecedente puede ser muy valioso aunque no sea exactamente de PET/cartón
si reproduce con gran similitud:

```
PROBLEMA → PROCESO → HERRAMIENTA/MODELO → IMPLEMENTACIÓN → INDICADORES → RESULTADOS
```

### Redefinición de responsabilidades de los researchers

Para evitar redundancia entre los dos agentes de descubrimiento existentes:

- **`inventory-researcher` es el researcher PRINCIPAL.** Cubre todo el
  espacio unificado de "gestión de procesos de control de inventarios"
  (secciones 5, 6 y 7 de este archivo). Es el que se lanza por defecto.
- **`process-researcher` es SECUNDARIO y de uso restringido.** Solo se
  lanza cuando el orquestador necesita **profundizar específicamente en el
  ángulo BPM/modelamiento/estandarización/rediseño del propio proceso de
  control de inventarios** (p. ej. mapeo detallado del flujo de
  registro/entradas/salidas, rediseño o estandarización del proceso de
  control, caracterización de procedimientos de inventario) — no para temas
  de gestión de procesos genéricos ajenos al control de inventarios. No se
  ejecuta en paralelo con `inventory-researcher` por defecto (regla dura,
  sección 16).

Los prefijos de ID existentes se conservan por continuidad con la matriz:
`L2-` para candidatos de `inventory-researcher` (ahora el flujo principal),
`L1-` para candidatos de `process-researcher` (uso puntual).

## 6. Prioridad temática de búsqueda

**Prioridad 1 — máxima**
`PET recycling + inventory`, `PET recycling + inventory management`,
`PET recycling + inventory control`, `plastic recycling + inventory
management`, `plastic waste + inventory control`, `recycled plastic +
inventory management`.

**Prioridad 2**
`cardboard recycling + inventory`, `cardboard recycling + inventory
management`, `paper recycling + inventory control`, `recycled cardboard +
inventory`.

**Prioridad 3**
`recycling company + inventory management`, `recycling plant + inventory
control`, `recycling industry + inventory`, `waste recycling + inventory
management`, `material recovery facility + inventory`, `recycled materials
inventory control`.

**Prioridad 4 — solo si es necesario ampliar**
`MYPE + inventory management`, `SME + inventory control`, `small
manufacturing company + inventory management`. Para esta prioridad, exigir
analogía operacional clara: recepción de materiales → almacenamiento →
transformación/procesamiento → almacenamiento/control → venta/despacho. Ser
PYME/MYPE por sí solo **no** constituye similitud suficiente.

No agotar automáticamente una prioridad antes de pasar a la siguiente: el
researcher puede combinar tiers en un mismo lote si es más eficiente, pero
debe reportar de qué prioridad proviene cada candidato.

## 7. Herramientas / modelos de interés

Sin limitar artificialmente la búsqueda a esta lista: clasificación ABC,
Kardex, inventario permanente, inventario periódico, inventarios cíclicos,
control de entradas y salidas, stock mínimo/máximo, punto de pedido, stock de
seguridad, EOQ, pronósticos de demanda, indicadores de inventario, exactitud
de inventario, sistemas de registro, trazabilidad, digitalización del
control de inventarios, sistemas de información para inventarios,
gestión/control de almacenes, modelos de gestión de inventarios, modelos de
revisión continua/periódica, modelos (Q,R), (s,S) u otros pertinentes,
modelamiento/estandarización/rediseño del proceso de control de inventarios.

Si aparece otra herramienta académicamente válida directamente relacionada
con el problema, no descartarla por no estar en esta lista — el researcher
debe explicar cómo podría relacionarse con el caso.

## 8. Profundidad metodológica obligatoria

Para un **antecedente fuerte**, priorizar:

```
PROBLEMA REAL → HERRAMIENTA/MODELO → IMPLEMENTACIÓN → INDICADORES → RESULTADOS MEDIBLES
```

Preferentemente con secuencia **ANTES → INTERVENCIÓN → DESPUÉS**.

No confundir nunca:

- **RESULTADO MEDIDO** (dato real antes/después)
- **META PROPUESTA** (cifra objetivo futura, verbo en futuro/condicional)
- **RESULTADO SIMULADO** (válido si está explícitamente etiquetado como
  simulación)
- **RECOMENDACIÓN** (sugerencia sin dato asociado)

Cada candidato debe declarar explícitamente cuál de estos cuatro tipos es su
"resultado" — ver campo `result_type` en la matriz (sección 19).

## 9. Exclusiones y penalizaciones

**No** seleccionar como antecedente metodológico principal trabajos basados
principalmente en: FODA/DAFO, diagnóstico descriptivo básico, encuestas o
entrevistas sin intervención, recomendaciones generales, KPIs solamente
propuestos, planes no implementados. Pueden conservarse como **evidencia
complementaria** si tienen gran similitud sectorial (ver umbrales, sección
17).

**Excluir como metodología principal** (aplica sobre todo a candidatos de
`process-researcher`, Línea Procesos): Lean Manufacturing, Lean Management,
5S, Kaizen, Lean Six Sigma. Un trabajo cuya intervención principal dependa de
estas metodologías **no puede** ser antecedente, aunque reporte buenos
resultados. Automático, no negociable por un subagente individual.

**Caso híbrido** (p. ej. una metodología permitida — BPR, rediseño de
procesos — que use una herramienta de raíz Lean como Value Stream Mapping):
**no decidir automáticamente**. Marcar `REVISIÓN MANUAL — POSIBLE CONFLICTO
METODOLÓGICO`, aplicar la penalización de componente B del scoring (sección
17) y dejar la decisión al orquestador junto con el usuario. Este es
exactamente el caso ya registrado de `L1-001` (ver sección 21).

También excluir o penalizar fuertemente: artículos únicamente ambientales,
contaminación sin gestión de inventarios, estudios químicos del PET,
reciclaje exclusivamente ambiental, revisiones bibliográficas sin aplicación
(cuando se buscan antecedentes principales), trabajos sin organización/caso
real, artículos sin relación real con inventarios/control de materiales.

## 10. Criterios bibliográficos

- **Rango temporal principal:** 2015–2026 inclusive, pero **trabajos
  anteriores a 2021 solo se consideran excepcionalmente si son
  fundamentales**, y debe justificarse explícitamente por qué se incluyen
  pese a no estar en el rango preferente 2021–2026.
- **Idiomas:** inglés y español.
- **Objetivo:** 15 antecedentes finales de alta calidad. **Nunca** se rellena
  la cuota con fuentes débiles, dudosas o inventadas. No hay obligación de
  llegar exactamente a 15 si la evidencia de calidad no alcanza ese número.
- **Artículos científicos principales:** preferentemente estudio de caso,
  organización/planta/empresa real, problema relacionado con
  inventarios/materiales, herramienta/modelo aplicado, resultados medibles,
  indexación Scopus, Q1 o Q2, preferentemente también Web of Science. Q3/Q4
  no se priorizan si existen suficientes Q1/Q2.
- **Tesis y repositorios universitarios:** permitidos, clasificados
  explícitamente como **evidencia complementaria**, nunca como artículo
  Q1/Q2. No se les inventa cuartil; se evalúa calidad de universidad,
  metodología y similitud.

  > Aparecer en ScienceDirect, Springer, Emerald, Taylor & Francis, Wiley,
  > MDPI o SciELO **no implica** Q1/Q2. El cuartil se verifica de forma
  > independiente (ver sección 12) y se registra la fuente usada.

## 11. Fuentes de descubrimiento

**Cinco plataformas priorizadas por la tesista** (herramientas de
descubrimiento, no fuentes de verificación — ver sección 12):

1. Elicit — https://elicit.com/
2. SciSpace — https://scispace.com/es
3. Perplexity — https://www.perplexity.ai/
4. Consensus — https://consensus.app/
5. SciELO — https://www.scielo.org/es/

No son exclusivas: si `WebSearch`/`WebFetch` encuentran mejores artículos o
tesis por otras vías académicas fiables, deben considerarse igual. SciELO
además puede actuar como **fuente primaria** cuando el artículo original
esté efectivamente alojado allí (no solo como buscador).

**Nota operativa (regla dura, ver sección 16):** Elicit, SciSpace, Consensus
y Perplexity son mayormente interfaces conversacionales/interactivas que
pueden requerir login o no ser accesibles vía `WebFetch` estándar. Un
researcher debe intentarlas de forma razonable (pocos intentos); si no son
automatizables, **no forzar el acceso** — registrar la búsqueda como
"pendiente de intento manual por la tesista" en el lote correspondiente
(sección 20) y continuar con las demás fuentes (SciELO, Google Scholar,
Scopus/ScienceDirect/WoS vía `WebSearch`, editoriales listadas abajo). Nunca
gastar múltiples tool calls intentando variantes de acceso a una misma
plataforma bloqueada.

Ninguna afirmación generada por Elicit/SciSpace/Consensus/Perplexity/Google
Scholar demuestra por sí sola Q1/Q2, Scopus, Web of Science, DOI correcto o
resultados del artículo — eso siempre se confirma después en la publicación
original (sección 12, `reference-verifier`).

**Bases/fuentes académicas a priorizar además:** Scopus, ScienceDirect, Web
of Science, SpringerLink, Wiley Online Library, Taylor & Francis, Emerald
Insight, MDPI, SciELO, DOAJ, Google Scholar, Crossref, repositorios
institucionales/universitarios, otras fuentes académicas fiables.

## 12. Verificación de cuartil

Priorizar, en este orden: SCImago Journal Rank (SJR) → Scopus Sources
(cuando sea accesible) → JCR/Web of Science (cuando sea pertinente/accesible)
→ otra fuente académica fiable si las anteriores no son accesibles.

Registrar siempre: cuartil, fuente, año del ranking consultado (cuando esté
disponible), categoría (si es relevante), estado de verificación. Nunca
inventar cuartil. Si solo hay evidencia secundaria (agregadores que replican
SJR, por ejemplo), marcar explícitamente `CUARTIL PENDIENTE DE VERIFICACIÓN
PRIMARIA` — exactamente el caso ya documentado para `L1-001` en
`verification-log.md`.

## 13. Acceso al full text

Estados posibles: `OPEN_ACCESS`, `REPOSITORY_COPY`, `AUTHOR_MANUSCRIPT`,
`ABSTRACT_ONLY`, `PAYWALL`, `AUTOMATION_BLOCKED`, `UNAVAILABLE`.

**Diferenciar siempre `PAYWALL` de `AUTOMATION_BLOCKED`.** Un HTTP 403 a
Claude **no** significa automáticamente que el artículo sea inaccesible para
una persona mediante navegador (caso ya documentado: `L1-002`, sección 21).

Antes de abandonar un paper muy relevante por paywall, se puede buscar de
forma **eficiente** una copia legal: repositorio institucional, accepted
manuscript, author manuscript, preprint, repositorio universitario, página
académica del autor, fuente Open Access. Nunca evadir paywalls ni intentar
saltarse controles de acceso.

**Regla de pocos intentos:** no gastar muchos tool calls probando variantes
equivalentes de una URL bloqueada. Después de 2-3 intentos razonables
(WebFetch directo, una variante de URL, quizás un proxy de lectura):
`REQUIERE VERIFICACIÓN MANUAL` y continuar con el siguiente candidato.

## 14. Reglas de integridad académica (crítico)

Ningún candidato se convierte automáticamente en antecedente final:

```
DESCUBRIMIENTO → PREFILTRO → VERIFICACIÓN → ABSTRACT SCREENING → FULL TEXT/ANÁLISIS → DECISIÓN
```

- **Descubrimiento** (`inventory-researcher` / `process-researcher`): busca y
  propone candidatos en lotes. Solo propone, no aprueba ni rechaza
  definitivamente.
- **Prefiltro** (`paper-screener`): aplica inclusión/exclusión y score
  preliminar por lotes. Puede descartar candidatos claramente fuera de
  alcance, pero no puede aprobar un antecedente final.
- **Verificación** (`reference-verifier`): confirma identidad bibliográfica
  e indexación **solo de los sobrevivientes del prefiltro, después de
  aprobación humana** (sección 15, Fase 3).
- **Abstract screening / Full text / Análisis** (`paper-analyst`): extrae
  metodología, contexto, indicadores y resultados **solo de candidatos ya
  verificados**, y el análisis profundo de texto completo se reserva para
  finalistas (Fase 5). Marca explícitamente cualquier dato no confirmable.
- **Decisión final:** la toma el orquestador junto con el usuario, a partir
  del score y el estado de verificación. **Ningún subagente tiene autoridad
  para declarar un artículo antecedente final.**

Reglas adicionales sin excepción:

- Dato no verificable → `NO VERIFICADO` en la matriz y en cualquier nota,
  nunca omitido silenciosamente ni inventado.
- Sin texto completo → no se afirman detalles metodológicos ni resultados
  que solo se conocerían leyéndolo. Se documenta explícitamente qué proviene
  solo del abstract.
- Resultados cuantitativos siempre del paper o evidencia primaria
  consultable, nunca inferidos ni estimados.
- Nunca se fabrica una referencia para completar la cuota de 15.

## 15. Arquitectura low-cost por fases

**Principio central:** este proyecto se ejecuta con Claude Pro y la cuota es
limitada. Máxima calidad útil con mínimo consumo razonable (ver reglas duras,
sección 16).

**Fase 1 — Discovery por lotes.** Un researcher (por defecto
`inventory-researcher`) busca candidatos en **lotes de 20-25** por ronda.
Recolecta solo lo barato: título, año, revista/fuente, DOI si aparece
fácilmente, URL, abstract/snippet disponible, sector aproximado, problema
aparente, herramienta aparente. Nada de full text ni verificación exhaustiva.
Ningún agente por artículo individual.

**Fase 2 — Prefiltro barato por lotes.** `paper-screener` aplica año, idioma,
relación con inventarios, similitud del problema, similitud operacional,
sector, herramienta aparente, indicio de caso aplicado, exclusiones —
sobre el lote completo. Objetivo orientativo: reducir 20-25 candidatos a
8-12 fuertes (no es cuota rígida; calidad > cantidad).

> **En la primera ronda futura, y en cada ronda por defecto, el flujo se
> DETIENE al final de esta fase** y se pide revisión humana antes de
> continuar a verificación (Fase 3).

**Fase 3 — Verificación bibliográfica.** Solo después de aprobación humana
explícita. Para los sobrevivientes del prefiltro: DOI, autores, año,
revista, Scopus, Q1/Q2, WoS cuando corresponda, acceso a full text. Usar
metadata y verificaciones deterministas primero (Crossref, etc.); no usar
análisis profundo para comprobar metadata.

**Fase 4 — Abstract screening.** Solo candidatos bibliográficamente fuertes.
Evaluar problema → herramienta → implementación aparente → indicadores →
resultados aparentes. Eliminar antes del full text: teóricos, revisiones sin
aplicación, diagnósticos simples, propuestas sin implementación,
sector/problema demasiado lejano, metodología prohibida (sección 9).

**Fase 5 — Full text / análisis profundo.** Solo finalistas que superaron
todas las fases anteriores. Aquí sí se usa `paper-analyst` en profundidad:
problema, contexto, metodología, herramienta, implementación, muestra,
proceso, indicadores, resultados, antes/después, limitaciones, utilidad para
la tesis, indicadores potencialmente transferibles. Esta es la fase cara.

**Fase 6 — Decisión.** Clasificar cada candidato: `ANTECEDENTE FUERTE`,
`RESERVA`, `EVIDENCIA COMPLEMENTARIA`, `DESCARTADO`, `REVISIÓN MANUAL`
(sección 17). La decisión final requiere siempre revisión humana.

## 16. Reglas duras de consumo

1. Discovery trabaja por **lotes** (20-25 candidatos/ronda), no artículo por
   artículo.
2. Screening trabaja por **lotes**, sobre el lote completo de una ronda.
3. **Máximo 1 researcher activo por defecto.**
4. **No** lanzar researchers en paralelo salvo autorización explícita del
   usuario.
5. **No** lanzar varios agentes para la misma consulta.
6. **No** crear subagentes dinámicos por artículo.
7. **No** hacer full text automáticamente — solo en Fase 5, solo finalistas.
8. **No** ejecutar `paper-analyst` antes de Fase 5.
9. **No** ejecutar `reference-verifier` sobre candidatos ya `DESCARTADO`.
10. Reutilizar metadata ya obtenida — no releer/reverificar lo ya
    almacenado y confirmado sin razón nueva.
11. Mantener el registro de URLs/consultas ya intentadas
    (`resultados/control-eficiencia.md`) para evitar repeticiones.
12. Ante 403/anti-bot: pocos intentos razonables (2-3) →
    `AUTOMATION_BLOCKED` → revisión manual. No perseguir.
13. **No** perseguir exhaustivamente un único candidato durante discovery.
14. Si una fuente prioritaria (sección 11) requiere login o no es
    automatizable: no forzar. Registrar como búsqueda manual pendiente y
    continuar.
15. Al alcanzar el objetivo de una fase: **DETENERSE**.
16. Antes de comenzar una fase cara (verificación, full text): **solicitar
    aprobación humana**.
17. No verificar dos veces el mismo DOI con dos agentes distintos salvo
    conflicto real entre fuentes.
18. No enviar candidatos débiles (score preliminar bajo, ver sección 17) a
    verificación o análisis profundo.

## 17. Sistema de scoring de relevancia (0–100)

Rediseñado para el tema unificado. Aplicado por `paper-screener` (score
preliminar, con lo disponible en discovery) y refinado por
`reference-verifier`/`paper-analyst` a medida que hay más evidencia. Todo
subagente que asigne un score debe dejar el desglose por escrito.

| Componente | Peso | Puntos máx. | Criterio |
|---|---|---|---|
| A. Similitud del problema | Alto | 20 | 20 = coincide de forma directa y explícita con varios problemas de la sección 3 (registros manuales, stock desconocido, entradas/salidas sin control, trazabilidad insuficiente, inventario desactualizado, dificultad de distinguir material recibido/en proceso/procesado/almacenado/vendido) · 14 = coincide claramente con 2-3 de esos problemas · 8 = coincidencia parcial o genérica ("mejorar gestión de inventarios" sin detalle) · 0 = problema no relacionado con control de inventarios |
| B. Calidad de la herramienta/metodología | Alto | 20 | 20 = modelo/herramienta robusto y reconocido en Ingeniería Industrial (ABC, EOQ, (s,S)/(Q,R), Kardex + sistema de registro, revisión continua/periódica, pronóstico de demanda validado, sistema de información/digitalización con lógica de control, rediseño/estandarización del proceso de inventario, etc.) aplicado con rigor · 12 = herramienta válida aplicada de forma parcial/simplificada · 5 = herramienta débil (checklist genérico, diagnóstico sin modelo) · 0 = sin herramienta/metodología identificable |
| C. Implementación real | Alto | 20 | 20 = implementado en empresa real con datos reales antes/después · 12 = piloto/simulación con datos reales, claramente etiquetado como simulación · 5 = propuesta diseñada pero no implementada · 0 = puramente teórico |
| D. Resultados cuantificables | Alto | 15 | 15 = antes/después medido, cifras verificables en el texto · 8 = resultado parcialmente cuantificado o resultado simulado etiquetado · 3 = solo cualitativos · 0 = sin resultados, o solo meta/recomendación propuesta (nunca confundir meta con resultado, sección 8) |
| E. Similitud sectorial/operacional | Medio | 10 | 10 = PET/cartón/reciclaje directo · 7 = residuos sólidos/materiales reciclables/MRF · 5 = empresa de transformación de materiales con flujo recepción→procesamiento→almacenamiento→venta comparable · 3 = MYPE/PYME con analogía operacional clara y justificada (no solo por ser MYPE) · 0 = sector sin analogía operativa |
| F. Calidad académica | Relevante | 10 | 10 = Q1 verificado · 7 = Q2 verificado · 4 = Q3/Q4 verificado · 2 = tesis/repositorio o cuartil no verificable |
| G. Acceso/evidencia verificable | Relevante, no dominante | 5 | 5 = texto completo disponible (`OPEN_ACCESS`/`REPOSITORY_COPY`/`AUTHOR_MANUSCRIPT`) · 2 = solo abstract · 0 = no disponible sin alternativa encontrada |

**Suma máxima: 100.**

### Regla anti-sesgo sectorial (obligatoria)

Un artículo de reciclaje con FODA + KPIs propuestos + ninguna implementación
**no puede** obtener score alto solo por coincidencia sectorial: sus
componentes C y D ya lo limitan estructuralmente, y además aplica el tope
duro de abajo. Un artículo de otro sector con problema prácticamente
idéntico, metodología robusta, implementación real y resultados medidos
**sí** puede ser antecedente fuerte si existe analogía operacional
justificable (componente E ≥ 3, justificado por escrito).

### Tope duro (cap)

Si `implementation_status = NO_IMPLEMENTADO` **y**
`result_type = META_PROPUESTA` (sección 19): el score total **no puede
superar 35/100**, sin importar cuánto sumen los demás componentes. Este tope
ya es consistente con el resultado real obtenido para `L2-001` en el smoke
test (34/100).

### Penalizaciones (se restan sobre el subtotal, pueden llevar el score a 0)

- Sector sin analogía operativa real: **-10**
- Resultados no verificables (afirmados sin sustento localizable en el
  texto): **-15**
- Información bibliográfica dudosa (DOI no resuelve, autor/año/revista no
  verificable): **-20**
- Caso híbrido con conflicto metodológico no resuelto (p. ej. herramienta de
  raíz Lean dentro de una metodología permitida): **-5** en el componente B,
  además de marcar `REVISIÓN MANUAL — POSIBLE CONFLICTO METODOLÓGICO`.

**Exclusión directa (score = 0):** cualquier candidato de la línea de
procesos cuya intervención principal sea Lean Manufacturing, Lean
Management, 5S, Kaizen o Lean Six Sigma (sección 9).

### Umbrales de clasificación (Fase 6, orientativos — nunca sustituyen la revisión humana)

- **ANTECEDENTE FUERTE:** score ≥ 70 **y** cumple todos los gates
  obligatorios que le correspondan (ver subsección "Gates obligatorios"
  abajo) — un score alto por sí solo **no** basta. Además: sin conflicto
  metodológico sin resolver, implementación real o piloto/simulación con
  datos reales, estado de verificación `VERIFICADO` o `PARCIALMENTE
  VERIFICADO`.
- **RESERVA:** score 55-69.
- **RESERVA / PENDIENTE DE VERIFICACIÓN:** score ≥ 70 pero falta verificar
  al menos un gate crítico (p. ej. Scopus o Q1/Q2 sin confirmar de forma
  primaria). Nunca se clasifica como `ANTECEDENTE FUERTE` mientras el gate
  siga pendiente.
- **EVIDENCIA COMPLEMENTARIA:** score 30-54, **y solo si** se cumple al
  menos una de estas condiciones: alta similitud del problema (A ≥ 14),
  alta similitud sectorial/operacional (E ≥ 7), o valor contextual
  excepcional claramente justificado por escrito. Útil solo como contexto,
  nunca como antecedente metodológico principal.
- **DESCARTADO:** score < 30; o score 30-54 sin ninguna de las condiciones
  de arriba; o fallo crítico de pertinencia/calidad (identidad
  bibliográfica no verificable, sector sin ninguna analogía operativa,
  metodología prohibida) independientemente del score.
- **REVISIÓN MANUAL:** conflictos metodológicos sin resolver o información
  crítica ambigua, independientemente del score — el orquestador decide con
  el usuario en cuál de las otras categorías termina.

### Gates obligatorios para ANTECEDENTE FUERTE (solo artículos científicos)

Un score ≥ 70 **no** es suficiente por sí solo. Para que un **artículo
científico** se clasifique como `ANTECEDENTE FUERTE` debe cumplir **todos**
estos gates:

1. Rango temporal 2021-2026, salvo excepción explícitamente justificada
   (sección 10).
2. Indexación **Scopus VERIFICADA** (verificación primaria o razonablemente
   confiable registrada como tal por `reference-verifier` — no solo
   evidencia indirecta vía agregadores).
3. **Cuartil Q1 o Q2 VERIFICADO** (misma exigencia de verificación primaria
   que el gate anterior).
4. Caso/organización real documentado (no puramente teórico/hipotético).
5. Herramienta/modelo efectivamente **implementado** (no solo propuesto).
6. **Resultados medidos y verificables** (no solo simulados sin etiquetar
   como tal, ni metas/recomendaciones propuestas).

Si el score ≥ 70 pero falta verificar Scopus, Q1/Q2, u otro gate crítico de
esta lista: clasificar como `RESERVA / PENDIENTE DE VERIFICACIÓN`, **nunca**
como `ANTECEDENTE FUERTE`.

**Tesis y repositorios universitarios siguen una vía separada:** no están
sujetos a los gates 2 y 3 (Scopus/Q1/Q2 no aplican a tesis, sección 10; una
tesis nunca recibe cuartil ficticio para "pasar" el gate), pero sí deben
cumplir los gates 1, 4, 5 y 6 para alcanzar `ANTECEDENTE FUERTE` dentro de su
propia categoría de evidencia.

## 18. Indicadores

**No se fijan todavía los indicadores finales de la tesis.** Durante el
análisis, registrar los indicadores usados científicamente en los
antecedentes cuando aparezcan, por ejemplo: inventory accuracy, stockout
rate, inventory turnover, days inventory, record accuracy,
processing/registration time, material loss, shrinkage, service level,
storage utilization, traceability accuracy, diferencias físico vs
registrado, u otros relevantes.

Diferenciar siempre **indicador utilizado en el paper** de **indicador
recomendado para la tesis**. La recomendación final se hará más adelante,
con evidencia suficiente acumulada.

## 19. Estructura de archivos del proyecto

```
CLAUDE.md
.claude/agents/
  inventory-researcher.md   ← researcher PRINCIPAL (tema unificado)
  process-researcher.md     ← researcher SECUNDARIO (uso restringido)
  paper-screener.md
  paper-analyst.md
  reference-verifier.md
research/
  inventarios/    ← notas de búsqueda y hallazgos crudos (flujo principal)
  procesos/       ← notas de búsqueda de process-researcher (uso puntual)
papers/
  candidatos/     ← candidatos aún no verificados/analizados
  seleccionados/  ← candidatos que pasaron verificación + análisis y están
                    listos para la decisión de selección final
resultados/
  matriz-articulos.csv     ← matriz maestra (ver columnas abajo)
  antecedentes.md           ← antecedentes finales aprobados por el usuario
  descartados.md            ← candidatos descartados, con motivo
  verification-log.md       ← bitácora de verificación bibliográfica
  control-eficiencia.md     ← registro de rondas + consultas/URLs intentadas
```

Cada candidato en `papers/candidatos/` y `papers/seleccionados/` debe tener
un ID único y consistente con la columna `ID` de `matriz-articulos.csv`:
`L2-` para candidatos del researcher principal (inventarios/proceso
unificado), `L1-` para candidatos puntuales de `process-researcher`.

### Columnas de `matriz-articulos.csv`

Columnas heredadas (sin cambios): `ID, linea, titulo, autores, anio, pais,
tipo_publicacion, revista_universidad, doi, url, indexacion, cuartil,
fuente_verificacion_cuartil, sector, problema, herramienta_modelo,
metodologia, indicadores, resultado_antes, resultado_despues,
mejora_cuantitativa, similitud_con_mype, score_relevancia, estado,
estado_verificacion, motivo_inclusion, observaciones`.

Columnas nuevas (añadidas al final, sin romper filas existentes):

- `full_text_access` — uno de `OPEN_ACCESS`, `REPOSITORY_COPY`,
  `AUTHOR_MANUSCRIPT`, `ABSTRACT_ONLY`, `PAYWALL`, `AUTOMATION_BLOCKED`,
  `UNAVAILABLE`.
- `evidence_level` — `FULL_TEXT` | `ABSTRACT_ONLY` | `METADATA_ONLY`.
- `problem_similarity` — `ALTA` | `MEDIA` | `BAJA`, ligado al componente A
  del scoring.
- `operational_similarity` — `ALTA` | `MEDIA` | `BAJA`, ligado al
  componente E.
- `methodological_depth` — `ALTA` | `MEDIA` | `BAJA`, ligado al componente
  B.
- `implementation_status` — `IMPLEMENTADO` | `PILOTO_SIMULACION` |
  `NO_IMPLEMENTADO` | `TEORICO`.
- `result_type` — `RESULTADO_MEDIDO` | `RESULTADO_SIMULADO` |
  `META_PROPUESTA` | `RECOMENDACION` | `SIN_RESULTADO` (sección 8).
- `manual_review_required` — `SÍ` | `NO`.
- `methodological_conflict` — `SÍ` | `NO` (caso híbrido Lean/otra
  metodología, sección 9).
- `source_quartile` — `Q1` | `Q2` | `Q3` | `Q4` | `NO_ENCONTRADO` |
  `NO_APLICA_TESIS`.
- `quartile_year` — año de edición del ranking consultado, o
  `NO_VERIFICADO`/`NO_APLICA`.
- `quartile_verification_status` — `VERIFICADO_PRIMARIO` |
  `VERIFICACION_INDIRECTA` | `NO_VERIFICADO` | `NO_APLICA`.
- `candidate_stage` — `DISCOVERY` | `PREFILTER_SURVIVOR` |
  `PREFILTER_DESCARTADO` | `VERIFICATION_PENDING` | `VERIFIED` |
  `ABSTRACT_SCREENING` | `FULL_TEXT_ANALYSIS` | `FINALISTA` | `DECIDIDO` |
  `PRE-ARQUITECTURA (smoke test)` para las 3 filas históricas.

## 20. Control de eficiencia por ronda

`resultados/control-eficiencia.md` registra, por ronda: candidatos
descubiertos, eliminados en prefiltro, supervivientes, enviados a
verificación, enviados a abstract screening, enviados a full text,
finalistas, fuentes bloqueadas, verificaciones manuales pendientes. También
mantiene un log de URLs/consultas ya intentadas para evitar repetirlas. No
se estiman tokens ficticios — el objetivo es detectar si se está
profundizando demasiado pronto en una ronda dada.

## 21. Historial del smoke test (preservado, no reescribir)

Los siguientes candidatos son evidencia histórica de la prueba inicial del
pipeline y **no forman parte** de la búsqueda de los 15 antecedentes. Sus
datos en `matriz-articulos.csv`, `verification-log.md`, `descartados.md` y
`research/` se conservan intactos. Reglas aprendidas de ellos, ya
incorporadas en la arquitectura de arriba:

- **`L1-001`** (BPR + simulación + VSM, confecciones, Vietnam): caso híbrido
  metodológico (VSM de raíz Lean dentro de un marco declarado BPR). Bajo la
  nueva arquitectura corresponde a **RESERVA / REVISIÓN MANUAL** por ese
  conflicto, no a una aprobación directa pese a su score de 64/100 — ver
  regla de caso híbrido, sección 9, y penalización de componente B, sección
  17.
- **`L1-002`** (MES/KPI, PYME manufacturera, Italia): descartado en
  screening. Regla aprendida: no asumir "inaccesible" únicamente por un 403
  automatizado — puede ser `AUTOMATION_BLOCKED` (bloqueo anti-bot hacia
  herramientas automatizadas, no necesariamente hacia una persona con
  navegador), aunque su similitud sectorial también sea baja. Ver sección
  13.
- **`L2-001`** (diagnóstico + FODA + KPIs propuestos, empresa recicladora,
  Quevedo, Ecuador): gran similitud sectorial (componente E alto) pero
  metodología/implementación insuficiente (FODA + KPIs solo propuestos, sin
  medición real). Bajo la nueva arquitectura corresponde a **EVIDENCIA
  COMPLEMENTARIA/CONTEXTUAL**, consistente con el tope duro de la sección 17
  (`implementation_status = NO_IMPLEMENTADO` + `result_type =
  META_PROPUESTA` → score ≤ 35; su score real fue 34/100).

## 22. Regla operativa actual

**No se ejecuta ninguna búsqueda, verificación ni análisis hasta que el
usuario lo apruebe explícitamente.** Cuando el usuario apruebe iniciar la
investigación, esta comienza en Fase 1 (Discovery, sección 15) con un único
researcher activo por defecto, y **se detiene automáticamente al final de la
Fase 2 (prefiltro) de la primera ronda** para revisión humana antes de
continuar a verificación — sin excepción, salvo instrucción explícita en
contrario del usuario.
