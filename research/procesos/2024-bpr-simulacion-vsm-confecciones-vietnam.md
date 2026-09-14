# Improving processing efficiency through workflow process reengineering, simulation and value stream mapping: a case study of business process reengineering

- Autores: Wang, C.; Vo, T.T.B.C.; Hsu, H.; Chung, Y.; Nguyen, N.T.; Nhieu, N. (nombres tal como aparecen en la ficha de Emerald recuperada; no se pudo verificar nombres completos/afiliaciones por estar el texto completo detrás de paywall)
- Año: 2024
- Fuente/plataforma: Emerald Publishing — revista *Business Process Management Journal*
- Tipo: artículo científico
- URL: https://www.emerald.com/insight/content/doi/10.1108/bpmj-11-2023-0869/full/html
- DOI: 10.1108/BPMJ-11-2023-0869
- Idioma: inglés

## Por qué podría ser relevante (razonamiento preliminar, no verificado)

Es un caso aplicado de **Business Process Reengineering (BPR)** combinado con **simulación** y **Value Stream Mapping (VSM)** en una empresa real de confecciones/vestuario en Vietnam. Sigue el patrón problema → herramienta → implementación → indicadores → resultado que pide CLAUDE.md: identifica actividades sin valor agregado (NVA) y esenciales-sin-valor-agregado (ENVA) en la línea de costura, rediseña el flujo de trabajo y valida con simulación. Resultados reportados en el abstract/resumen estructurado de Emerald: de 186 operaciones combinadas ENVA/NVA se eliminaron 25 (15 ENVA + 10 NVA), con una reducción del 8.5% en la proporción de operaciones ENVA y eliminación del 100% de las operaciones NVA identificadas.

Sector: manufactura de confecciones (no reciclaje/PET/cartón). Se prioriza igual porque, tras múltiples búsquedas dirigidas a reciclaje de PET/cartón, residuos sólidos y plantas recicladoras con gestión por procesos/BPM no-Lean, no se encontró un candidato verificable de mejor ajuste sectorial (ver nota de ampliación de sector en el resumen de la tarea). Es una MYPE/empresa manufacturera con problema operacional comparable (ineficiencias de flujo, actividades sin valor agregado, necesidad de rediseño de proceso) — categoría 6 de la prioridad de CLAUDE.md.

## Texto completo disponible

Solo abstract — la página de Emerald muestra un resumen estructurado (objetivo, metodología, hallazgos) pero el texto completo requiere pago (~US$41) o suscripción institucional. Intenté abrir la página real con WebFetch (no solo el snippet de búsqueda) y confirmé el muro de pago directamente en la fuente.

## Nota de exclusión Lean (obligatoria)

Duda genuina explícita: el marco metodológico principal declarado en el título es **Business Process Reengineering (BPR)**, no "Lean Manufacturing" con ese nombre, y no se menciona 5S, Kaizen ni Lean Six Sigma. Sin embargo, una de las tres herramientas centrales usadas es **Value Stream Mapping (VSM)**, que es una herramienta históricamente asociada a Lean, y el marco de análisis (actividades NVA/ENVA/VA) también proviene de la tradición Lean de eliminación de desperdicio. No lo descarté yo mismo porque la intervención nombrada como principal es BPR + simulación (no "Lean Manufacturing" ni 5S/Kaizen/Lean Six Sigma tal como los define la exclusión de CLAUDE.md), pero dejo constancia explícita de esta ambigüedad para que `paper-screener` decida con el criterio de exclusión de CLAUDE.md si el uso de VSM cuenta como "intervención principal Lean" en este caso.

## Screening

**Resolución de la duda sobre exclusión Lean (punto 1 del encargo):** CLAUDE.md
sección 2 declara la exclusión absoluta para "Lean Manufacturing, Lean
Management, 5S, Kaizen, Lean Six Sigma" cuando la **intervención principal**
del trabajo depende de esas metodologías nombradas explícitamente así. Este
paper declara su marco principal como **Business Process Reengineering
(BPR)** — un marco de gestión de procesos distinto de Lean, no listado en la
exclusión — y usa **VSM como una de tres herramientas** dentro de ese marco
(junto con simulación), no como el programa de intervención central. Por lo
tanto, la exclusión automática de la sección 2 **no aplica literalmente**:
no es un caso de "intervención principal Lean/5S/Kaizen/Lean Six Sigma".
Sin embargo, esto encaja exactamente en el escenario que `paper-screener.md`
anticipa como "metodología reportada combina Lean con otra herramienta de
gestión de procesos no Lean": VSM y el marco de análisis NVA/ENVA/VA son de
tradición Lean, aunque el paraguas declarado sea BPR. Siguiendo la
instrucción explícita de `paper-screener.md` ("no aplicar la exclusión Lean
de forma dudosa... marca el candidato como 'revisar manualmente — mezcla de
metodologías' en observaciones y baja el score de carácter aplicado en vez
de descartarlo automáticamente, dejando la decisión final al orquestador"),
**no se aplica la exclusión directa (score 0)**; en su lugar se penaliza el
componente "Carácter aplicado" (ver desglose) y se marca explícitamente
"revisar manualmente — mezcla de metodologías" para que el orquestador
confirme esta lectura antes de avanzar a verificación/análisis.

- Sector/contexto: 10/20 — manufactura de confecciones/vestuario (Vietnam),
  no reciclaje/PET/cartón. Es una empresa real con un problema operacional
  de flujo comparable (ineficiencias de proceso, actividades sin valor
  agregado), categoría 6 de prioridad de CLAUDE.md ("MYPEs o empresas con
  problemas operacionales equivalentes"), pero no es físicamente comparable
  a pesaje/clasificación/procesamiento de materiales reciclables/almacenamiento
  de la MYPE del caso de estudio. Corresponde al tramo "MYPE/manufactura
  físicamente comparable" (10/20), no al tramo superior de reciclaje directo.
- Problema-herramienta: 16/20 — correspondencia fuerte: el problema
  (ineficiencias de flujo de trabajo, alta proporción de actividades NVA/ENVA)
  y la herramienta (rediseño de proceso validado con simulación y mapeo del
  flujo de valor) encajan directamente con los temas explícitos de Línea 1:
  "rediseño de procesos", "optimización de procesos", "simulación de procesos
  orientada a mejora", "mapeo y caracterización de procesos".
- Carácter aplicado: 10/15 (bajado desde el tramo máximo de 15 —
  "implementado en empresa real", que aplicaría de otro modo a un caso real
  con simulación de validación — específicamente por la mezcla de
  metodologías Lean/no-Lean señalada arriba, siguiendo la instrucción de
  `paper-screener.md` de penalizar este componente en vez de aplicar la
  exclusión directa). **Marcar: revisar manualmente — mezcla de
  metodologías (BPR declarado + VSM/marco NVA-ENVA de tradición Lean).**
- Resultados cuantificables: 10/20 — el abstract estructurado de Emerald
  reporta cifras antes/después (186 operaciones ENVA/NVA identificadas, 25
  eliminadas, reducción del 8.5% en proporción ENVA, eliminación del 100% de
  NVA), pero no se pudo verificar en el cuerpo del texto por estar detrás de
  paywall — se puntúa como "parcialmente cuantificados" (tramo 10), no como
  "antes/después con datos verificables en el texto" (tramo 20), porque el
  texto completo no fue accesible para confirmar los datos del abstract.
- Calidad académica (preliminar, sin verificar cuartil aún): 2/10 — Emerald
  / *Business Process Management Journal* es una editorial de interés listada
  en CLAUDE.md sección 4, pero el cuartil no está verificado en esta etapa
  (tarea exclusiva de `reference-verifier`); se usa el tramo "cuartil no
  verificable".
- Actualidad: 5/5 — publicado en 2024.
- Evidencia disponible: 3/10 — solo abstract estructurado disponible; el
  researcher confirmó el muro de pago directamente en la página real de
  Emerald (no solo snippet de buscador), por lo que corresponde al tramo
  "solo abstract/resumen" (3), no a "texto completo disponible" (10) ni a
  "no disponible" (0), dado que sí hay un abstract confiablemente visto.
- Penalizaciones aplicadas: ninguna adicional sobre la tabla anterior (la
  incertidumbre por paywall y la mezcla de metodologías ya están reflejadas
  en los componentes "Resultados cuantificables", "Evidencia disponible" y
  "Carácter aplicado" respectivamente; aplicar penalizaciones adicionales
  duplicaría el mismo descuento).
- Score preliminar: 56/100
- Decisión: SCREENED-IN — "revisar con cautela" (score en tramo 40-59):
  aspectos que la verificación/análisis podrían mejorar son la calidad
  académica (cuartil aún no verificado) y la disponibilidad de evidencia
  (posible acceso a texto completo institucional). Adicionalmente, queda
  pendiente para el orquestador la confirmación de la lectura "revisar
  manualmente — mezcla de metodologías" antes de invertir esfuerzo pleno de
  verificación/análisis.
- Motivo (si DESCARTADO): No aplica (SCREENED-IN).

## Análisis

- Fuente del análisis: **Solo abstract** (estructurado, Purpose/Design-Methodology-Approach/Findings/Originality). Verifiqué yo mismo, directamente vía WebFetch a la URL real de Emerald
  (https://www.emerald.com/insight/content/doi/10.1108/bpmj-11-2023-0869/full/html),
  que el abstract estructurado es visible públicamente y que el texto completo
  está bloqueado por paywall a **US$41.00** (mensaje de pago por artículo
  confirmado directamente en la página, no en un snippet de buscador). No
  pagué ni intenté eludir el muro de pago; no tuve acceso al cuerpo del texto,
  tablas, metodología detallada, muestra ni discusión.
- Problema investigado: ineficiencias de flujo de trabajo en la línea de
  costura de una empresa de confecciones (apparel) vietnamita — alta
  proporción de actividades sin valor agregado (NVA) y esenciales-sin-valor-
  agregado (ENVA), según el propio abstract ("Business Process Reengineering
  (BPR) aims to eliminate non-value-added (NVA) and essential non-value-added
  (ENVA) waste through radical process redesign").
- Metodología/herramienta: **Business Process Reengineering (BPR) multietapa**
  con **Workflow Process Reengineering**, **Value Stream Mapping (VSM)** y
  **simulación** de validación, según el abstract: "(1) identifying
  improvement processes and analyzing workflows via Workflow Process
  Reengineering and Value Stream Mapping; (2) improving efficiency by
  redefining roles and integrating automation; (3) validating changes through
  simulation and assessing key performance metrics." Nota de anomalía de
  pipeline (no la resuelvo yo, la traslado): `paper-screener` ya documentó y
  dejó pendiente para el orquestador la ambigüedad de que VSM y el marco
  NVA/ENVA/VA son de tradición Lean aunque el paraguas declarado sea BPR;
  no me corresponde recalcular esa decisión de inclusión/exclusión, solo
  reportar que sigue abierta.
- Contexto/empresa/sector: empresa real de confecciones/vestuario (apparel)
  en Vietnam ("Empirically tested through a case study of a Vietnamese
  apparel company"), sector manufactura textil — no reciclaje/PET/cartón.
- Indicadores usados: número de operaciones NVA, número de operaciones ENVA,
  proporción de operaciones ENVA sobre el total de operaciones de la línea de
  costura.
- Resultado antes: **186 operaciones combinadas ENVA+NVA identificadas** en
  la instalación de costura antes del rediseño — verificado por **ABSTRACT
  (categoría B)**, cita casi textual del abstract: "reducing 25 out of 186
  combined ENVA and NVA operations in the sewing facility". No verificado en
  el cuerpo del texto (paywall).
- Resultado después: **25 operaciones eliminadas** (15 ENVA + 10 NVA), con
  **eliminación del 100% de las operaciones NVA identificadas** — verificado
  por **ABSTRACT (categoría B)**, citas: "a decrease of 15 ENVA operations
  and the removal of 10 NVA operations" y "complete 100% elimination of NVA
  activities". No verificado en el cuerpo del texto (paywall).
- Mejora cuantitativa: **reducción del 8.5% en la proporción de operaciones
  ENVA** sobre el total — verificado por **ABSTRACT (categoría B)**, cita:
  "an 8.5% reduction in the proportion of ENVA operations". Además,
  eliminación del 100% de las NVA (ver arriba). No hay significancia
  estadística ni método de medición detallado visible en el abstract; eso
  queda **NO VERIFICADO** por estar en el cuerpo del texto (paywall).
- Similitud con la MYPE (razonada): **media**. El problema de fondo
  (ineficiencias operativas, actividades sin valor agregado, necesidad de
  rediseño y estandarización de un flujo con muchas operaciones manuales) es
  análogo al de la MYPE recicladora (falta de procedimientos estandarizados,
  tiempos elevados, falta de indicadores — sección 1 de CLAUDE.md). Sin
  embargo, el sector (confección textil) y el tipo de operación física
  (costura en línea de producción) no son comparables al flujo de
  pesaje/clasificación/procesamiento/almacenamiento de PET y cartón. Es una
  similitud metodológica y de tipo de problema, no de sector físico.
- Score final (desglose):
  - Similitud de sector/contexto: 10/20 — manufactura/confecciones, tramo
    "MYPE/manufactura físicamente comparable" (no reciclaje directo).
  - Correspondencia problema-herramienta: 16/20 — correspondencia fuerte
    entre el problema (ineficiencias de flujo, alta proporción NVA/ENVA) y la
    herramienta (rediseño validado con simulación y VSM), alineado con temas
    explícitos de Línea 1 (rediseño, optimización, simulación, mapeo de
    procesos).
  - Carácter aplicado: 10/15 — caso real empíricamente probado en una empresa
    de confecciones vietnamita, validado con simulación; se mantiene el
    ajuste de `paper-screener` (bajado desde 15) por la mezcla de
    metodologías BPR/VSM de tradición Lean, cuestión aún abierta para el
    orquestador. No recalculo ni resuelvo yo esta ambigüedad.
  - Resultados cuantificables y verificables: 10/20 — el abstract sí reporta
    antes/después con cifras explícitas (verificado por mí directamente vía
    WebFetch), pero al no poder confirmarse en el cuerpo del texto completo
    (paywall) no llega al tramo máximo de "datos verificables en el texto";
    corresponde a "resultados parcialmente cuantificados".
  - Calidad académica: 10/10 — cuartil **Q1** (mejor cuartil reportado,
    consistente entre fuentes para la categoría "Business/Management and
    Accounting (miscellaneous)"; varía Q1/Q2 según fuente/año para "Business
    and International Management") verificado por `reference-verifier` vía
    Scimago Journal Rank a través de agregadores secundarios (Resurchify,
    Researcher.life, Editage), con indicio adicional de cobertura Web of
    Science (wos-journal.info). **Advertencia que dejo explícita:** esta
    verificación es indirecta (acceso directo a scimagojr.com y a Scopus.com
    bloqueado por verificación anti-bot) y la indexación Scopus es solo
    indicio indirecto (réplica de un mismo ID Scimago en varios agregadores),
    no una confirmación primaria en Scopus.com/Clarivate. Puntúo en el tramo
    "Q1 verificado" siguiendo el registro de `reference-verifier`
    (autoridad de verificación bibliográfica, que no me corresponde
    cuestionar), pero el orquestador debe conocer que la robustez de esta
    verificación es menor que una confirmación primaria directa.
  - Actualidad: 5/5 — publicado en 2024.
  - Disponibilidad de evidencia verificable: 3/10 — solo abstract/resumen
    disponible (confirmado directamente por mí vía WebFetch a la página real
    de Emerald, no solo snippet de buscador).
  - Penalizaciones aplicadas: ninguna adicional. No aplica "contexto poco
    comparable" (hay analogía operativa real de problema, aunque no de
    sector físico — ya reflejado en el componente de sector). No aplica
    "ausencia de implementación real" (caso real implementado y validado por
    simulación). No aplica "resultados no verificables" (los resultados
    citados son trazables a una frase específica del abstract, no afirmados
    sin sustento — la incertidumbre por paywall ya está reflejada en
    "Resultados cuantificables" y "Evidencia disponible", penalizar de nuevo
    duplicaría el descuento). No aplica "información bibliográfica dudosa"
    (autores, año, revista y DOI están identificados y consistentes).
  - Subtotal: 10+16+10+10+10+5+3 = 64
- Score final: **64/100**
- Recomendación: **LISTO PARA DECISIÓN FINAL** (score ≥ 60 y estado de
  verificación PARCIALMENTE VERIFICADO). Esto es una recomendación técnica,
  no una aprobación de antecedente final — la decisión final la toman el
  usuario y el orquestador, considerando además la ambigüedad Lean/BPR aún
  abierta y la naturaleza indirecta de la verificación de cuartil/indexación
  Scopus señaladas arriba.
