# Estrategias para optimizar el control de inventarios y fortalecer los procesos administrativos en una empresa recicladora de Quevedo, Ecuador

- Autores: Darwin Antonio Montoya Torres; Rosa Jamileth Cedeño Andrade; Jefferson Alberto Agurto Soria; Byron Fabricio Loor Párraga (los cuatro afiliados a la Universidad Técnica Estatal de Quevedo, Ecuador — afiliación institucional, no es publicación de repositorio universitario, es artículo de revista)
- Año: 2026 (recibido 10-jun-2026, aceptado 21-jun-2026, publicado 11-jul-2026)
- Fuente/plataforma: Revista *Polo del Conocimiento* (revista científico-académica multidisciplinaria, Casa Editora del Polo, Manta, Ecuador), Vol. 11, No. 7 (2026), pp. 906-923
- Tipo: Artículo científico (Artículo de Investigación, revista con OJS/Open Journal Systems, acceso abierto CC BY-NC-SA 4.0). No es tesis ni repositorio universitario, aunque los autores son de una universidad.
- URL: https://polodelconocimiento.com/ojs/index.php/es/article/view/12063
- URL texto completo (HTML): https://polodelconocimiento.com/ojs/index.php/es/article/view/12063/html
- URL PDF: https://polodelconocimiento.com/ojs/index.php/es/article/download/12063/30739
- DOI: 10.23857/pc.v11i7.12063 (verificado directamente en metadatos `DC.Identifier.DOI` de la página fuente, no inferido)
- ISSN: 2550-682X (verificado en metadatos de la página)
- Idioma: Español (con resúmenes también en inglés y portugués)

## Cómo se accedió a la fuente

WebFetch fue bloqueado por la plataforma (HTTP 403), por lo que se accedió al HTML real de la página vía `curl` con user-agent de navegador, y se confirmaron directamente en el HTML fuente: título, autores, fechas, DOI, ISSN, volumen/número, páginas, y el texto completo del artículo (resumen, introducción, marco teórico, metodología, resultados, discusión, conclusiones, referencias). Ningún dato bibliográfico de este archivo fue tomado solo del snippet de un buscador.

## Por qué podría ser relevante (mi razonamiento, no un hecho verificado)

Coincidencia directa de sector: es un estudio de caso en una **empresa recicladora** (materiales reciclables, economía circular) en Quevedo, Ecuador — la prioridad más alta de la Línea 2 según `CLAUDE.md`. El problema diagnosticado es prácticamente un espejo del caso de la MYPE de la tesis: ausencia de procedimientos estandarizados de registro, registros manuales, desorganización del almacenamiento, dificultad para conocer existencias reales, escasa capacitación del personal y bajo uso de herramientas tecnológicas para el control de inventarios. El estudio también cita explícitamente antecedentes sobre Kardex y control de inventarios en PYMEs (Parrales et al., 2021; Malca, 2023) dentro de su marco teórico.

**Duda genuina que dejo explícita para `paper-screener`:** la intervención central de este estudio **no es un modelo cuantitativo clásico de inventarios** (no hay ABC, EOQ, punto de pedido, pronóstico de demanda, ni una implementación real de Kardex por parte de los autores). La herramienta usada es un diagnóstico mixto (entrevistas + encuestas + observación directa) seguido de un análisis **FODA / FODA cruzado** que desemboca en un **plan estratégico con KPIs propuestos** para el sistema de inventarios (exactitud de inventario, rotación de inventario, tiempo promedio de registro, % de material correctamente clasificado, % de pérdidas por errores, etc.). Estos indicadores son **metas propuestas, no resultados medidos**: el estudio no reporta datos antes/después ni implementación real de la propuesta. Esto lo acerca al patrón "propuesta no implementada" de la sección 6 de `CLAUDE.md` (carácter aplicado = 5, no 15), y no al patrón completo problema→modelo→implementación→indicadores→resultado.

No obstante, no lo considero un caso equivalente al "checklist genérico de orden y limpieza (tipo 5S)" que `CLAUDE.md` excluye explícitamente para esta línea: la intervención trata específicamente de **control de inventarios, indicadores de inventario y sistemas de registro** (temas centrales de la Línea 2), no de orden/limpieza física. Por eso lo reporto como candidato, pero con esta salvedad explícita para que `paper-screener` decida si el carácter no implementado / basado en FODA-KPI (en vez de un modelo de inventario cuantitativo) es suficiente para la línea.

No amplié a otro sector: este es un match directo de prioridad (a) — reciclaje — por lo que no fue necesario ampliar a MYPEs/transformación de materiales genéricas.

## Texto completo disponible

**Sí.** Se accedió y leyó el texto completo del artículo (resumen, introducción, marco teórico, metodología, resultados, análisis FODA, plan estratégico, tabla de indicadores, discusión, conclusiones y referencias), no solo el abstract.

## Otros datos NO VERIFICADOS

- Indexación en Scopus/Web of Science: NO VERIFICADO (pendiente de `reference-verifier`).
- Cuartil de la revista: NO VERIFICADO — no se debe afirmar cuartil en esta etapa; corresponde a `reference-verifier`.
- No se observó ninguna cifra de resultado cuantitativo antes/después en el texto (solo metas/fórmulas de KPIs propuestos); esto se deja anotado explícitamente, no se infiere ni se estima ningún porcentaje de mejora.

## Screening

**Resolución de la duda del researcher (punto 2 del encargo):** el propio
researcher documentó correctamente que la intervención central no es un
modelo cuantitativo clásico de inventarios (no hay ABC, EOQ, punto de
pedido, pronóstico de demanda ni una implementación real de Kardex), sino un
diagnóstico mixto + análisis FODA/FODA cruzado que desemboca en un plan
estratégico con **KPIs propuestos** (metas, no medidos). Esto se trata
explícitamente como "carácter aplicado" en el tramo de **propuesta no
implementada = 5/15** de la tabla de CLAUDE.md sección 6, no como
"implementado en empresa real" (15) ni como "piloto/simulación con datos
reales" (10). Consecuentemente, "resultados cuantificables" se puntúa en
**0/20**: no hay ningún dato antes/después medido en el texto, solo metas
propuestas de KPIs — el tramo 0 ("sin resultados") es el que corresponde,
no el tramo 5 ("solo cualitativos"), porque ni siquiera hay una evaluación
cualitativa de resultados de una intervención ya ejecutada, sino objetivos a
futuro.

No se trata del caso de exclusión de Línea 2 ("checklist genérico de orden y
limpieza tipo 5S"): la intervención trata específicamente temas centrales de
Línea 2 (control de inventarios, indicadores de inventario, sistemas de
registro), por lo que no se aplica esa exclusión. Sin embargo, la
correspondencia problema-herramienta se puntúa de forma moderada porque el
lado de la "herramienta" (diagnóstico + FODA + KPIs propuestos) es débil
frente a los temas de interés explícitos de Línea 2 (clasificación ABC, EOQ,
Kardex, control de entradas/salidas, modelos de gestión de inventarios) —
aunque el lado del "problema" es un espejo casi exacto de los problemas de
la MYPE del caso de estudio.

- Sector/contexto: 20/20 — coincidencia directa de sector: empresa
  recicladora de materiales reciclables (economía circular) en Quevedo,
  Ecuador — la prioridad más alta de Línea 2 en CLAUDE.md
  ("reciclaje/PET/cartón" en sentido amplio de empresa recicladora).
- Problema-herramienta: 12/20 — el problema diagnosticado (ausencia de
  procedimientos estandarizados, registros manuales, desorganización de
  almacenamiento, dificultad para conocer existencias reales, bajo uso de
  tecnología) es prácticamente un espejo de los problemas listados en
  CLAUDE.md sección 1. Pero la "herramienta" usada (diagnóstico + FODA +
  KPIs propuestos) no es un modelo cuantitativo de inventarios de los temas
  de interés explícitos de Línea 2 (ABC, EOQ, Kardex, control de entradas y
  salidas, etc.), por lo que se puntúa por debajo del tramo alto pese a la
  excelente correspondencia del lado del problema.
- Carácter aplicado: 5/15 — propuesta no implementada (diagnóstico + FODA +
  plan estratégico con KPIs propuestos, sin implementación real de la
  propuesta por parte de los autores), según lo documentado explícitamente
  por el researcher y confirmado en la lectura del texto completo.
- Resultados cuantificables: 0/20 — sin información de resultados
  antes/después; solo se formulan metas/fórmulas de KPIs propuestos, no
  resultados medidos. Sin información suficiente para acreditar ningún
  resultado real, se asume el mínimo.
- Calidad académica (preliminar, sin verificar cuartil aún): 2/10 — *Polo
  del Conocimiento* no está entre las editoriales/plataformas de interés
  listadas en CLAUDE.md sección 4 (ScienceDirect, Springer, Emerald, Taylor
  & Francis, Wiley, MDPI, SciELO); es artículo de revista con OJS (no tesis
  ni repositorio), pero el cuartil no está verificado en esta etapa —
  corresponde al tramo "cuartil no verificable".
- Actualidad: 5/5 — publicado en 2026.
- Evidencia disponible: 10/10 — texto completo leído y verificado
  directamente en la fuente (HTML real vía curl con user-agent de
  navegador), incluyendo resultados, discusión y conclusiones, no solo el
  abstract.
- Penalizaciones aplicadas: ninguna (el sector es un match directo, la
  identidad bibliográfica está verificada en metadatos de la propia página
  fuente, y la ausencia de resultados/implementación ya está reflejada de
  forma explícita y transparente en los componentes "Carácter aplicado" y
  "Resultados cuantificables" — no es un caso de resultados afirmados sin
  sustento, sino de metas declaradas abiertamente como no implementadas).
- Score preliminar: 54/100
- Decisión: SCREENED-IN — "revisar con cautela" (score en tramo 40-59): el
  ajuste de sector y la disponibilidad de evidencia son excelentes, pero el
  carácter aplicado y los resultados cuantificables son bajos porque es una
  propuesta no implementada. Útil principalmente como evidencia de
  contexto/espejo del problema de la MYPE (mismo sector, mismos síntomas de
  falta de control), no como antecedente de un modelo cuantitativo de
  inventarios ya validado. El orquestador debe evaluar si complementa mejor
  como antecedente de diagnóstico/contexto que como antecedente metodológico
  central de Línea 2.
- Motivo (si DESCARTADO): No aplica (SCREENED-IN).

## Análisis

- Fuente del análisis: **Texto completo**. WebFetch directo a
  https://polodelconocimiento.com/ojs/index.php/es/article/view/12063,
  a la variante `/html` y al PDF de descarga devolvió HTTP 403 en los tres
  casos (mismo bloqueo anti-bot que ya había reportado `reference-verifier`).
  Accedí al contenido completo a través del proxy de lectura
  `https://r.jina.ai/<URL>` sobre la URL de vista del artículo y sobre la
  variante `/html`, que sí devolvió el resumen, metodología, la Tabla 4 de
  indicadores/KPIs (nombres y metas) y las conclusiones. Esto es una lectura
  directa mía del contenido real del artículo (categoría C), independiente
  del archivo de research/ ya existente, y coincide con lo que el researcher
  había reportado.
- Problema investigado (según el propio paper): "deficiencias asociadas con
  la ausencia de registros sistemáticos, limitada capacitación del personal,
  desorganización en el almacenamiento" y bajo uso de herramientas
  tecnológicas para el control de inventarios en una empresa recicladora de
  Quevedo, Ecuador.
- Metodología/herramienta: **diagnóstico mixto** (entrevistas gerenciales +
  encuestas al personal + observación directa, enfoque descriptivo-
  exploratorio, diseño no experimental transversal) seguido de **análisis
  FODA / FODA cruzado** y culminando en un **plan estratégico con KPIs
  propuestos** para el sistema de inventarios (Tabla 4 del artículo). No es
  un modelo cuantitativo clásico de inventarios (no hay ABC, EOQ, punto de
  pedido, pronóstico de demanda ni Kardex implementado por los autores) —
  confirmado por mí en la lectura de la sección de metodología y resultados.
- Contexto/empresa/sector: empresa recicladora de materiales reciclables
  (economía circular) en Quevedo, Ecuador — coincidencia directa de sector
  con la Línea 2 (prioridad más alta de CLAUDE.md sección 2).
- Indicadores usados: Tabla 4 del artículo — exactitud del inventario (meta
  ≥98%), rotación del inventario (meta ≥8 veces/año), tiempo promedio de
  registro (meta ≤5 minutos), % material correctamente clasificado (meta
  ≥95%), % cumplimiento de procedimientos (meta ≥95%), % pérdidas por
  errores (meta ≤2%), % cumplimiento de capacitaciones (meta 100%). **Todos
  estos valores son metas propuestas para monitoreo futuro, no mediciones
  reales.** Cita textual confirmada en mi lectura: los KPIs "permitirán
  monitorear variables relacionadas con la exactitud del inventario, la
  rotación de existencias, el tiempo de registro y el cumplimiento de
  procedimientos administrativos" (verbo en futuro "permitirán", no
  reportando un hecho ya medido).
- Resultado antes: **NO DISPONIBLE**. El artículo describe deficiencias de
  forma cualitativa (ausencia de registros, desorganización, escasa
  capacitación) pero no reporta ninguna cifra de línea base medida (por
  ejemplo, no hay un % de exactitud de inventario actual, ni tiempo de
  registro actual medido). Confirmado directamente por mí leyendo el texto
  completo, no es una inferencia por falta de acceso.
- Resultado después: **NO DISPONIBLE**. No hay implementación real de la
  propuesta ni medición posterior por parte de los autores; solo se
  formulan las metas de la Tabla 4 citadas arriba, sin datos de seguimiento.
  Confirmado directamente por mí en la sección de resultados/discusión/
  conclusiones: el artículo es explícitamente "propositivo, no evaluativo"
  ("Presenta un modelo estratégico recomendado sin validación empírica
  posterior").
- Mejora cuantitativa: **NO DISPONIBLE / NO VERIFICADO**. No existe ningún
  cálculo de mejora porcentual real en el texto — solo umbrales meta (p. ej.
  "≥98%", "≤2%") que el plan aspira a alcanzar en el futuro, no una
  comparación antes/después medida. Reportar estas metas como "mejora
  cuantitativa" sería atribuir al artículo un resultado que no midió; me
  abstengo de hacerlo, siguiendo la regla explícita de `paper-analyst.md` y
  de CLAUDE.md sección 3/5.
- Similitud con la MYPE (razonada): **alta**. El problema diagnosticado es
  prácticamente un espejo del caso de estudio: empresa recicladora PYME,
  materiales heterogéneos, mismos síntomas (falta de control, registros
  manuales, desorganización de almacenamiento, desconocimiento del stock
  real). La similitud es de contexto/problema, no de solución validada — es
  más útil como evidencia de diagnóstico/contexto que como antecedente
  metodológico de un modelo de inventarios ya probado.
- Score final (desglose):
  - Similitud de sector/contexto: 20/20 — empresa recicladora (economía
    circular) en Ecuador, coincidencia directa de sector con Línea 2.
  - Correspondencia problema-herramienta: 12/20 — el problema es un espejo
    casi exacto de los problemas de la MYPE, pero la herramienta (diagnóstico
    + FODA + KPIs propuestos) no es un modelo cuantitativo de inventarios de
    los temas centrales de Línea 2 (ABC, EOQ, Kardex, control de
    entradas/salidas).
  - Carácter aplicado: 5/15 — propuesta no implementada; confirmado
    directamente por mí en la lectura completa (plan estratégico sin
    validación empírica posterior por parte de los autores).
  - Resultados cuantificables y verificables: 0/20 — sin ningún dato
    antes/después medido; solo metas de KPIs propuestas para monitoreo
    futuro. Confirmado directamente por mí, no por falta de acceso al texto.
  - Calidad académica: 2/10 — cuartil **NO VERIFICADO** (revista no
    encontrada en Scimago Journal Rank ni en JCR, según `reference-verifier`)
    y **sin indexación en Scopus ni Web of Science** (solo Latindex 2.0,
    Dialnet, REDIB, que no equivalen a Scopus/WoS). Tramo "cuartil no
    verificable".
  - Actualidad: 5/5 — publicado en 2026.
  - Disponibilidad de evidencia verificable: 10/10 — texto completo leído y
    confirmado de forma independiente por mí (vía proxy de lectura, dado que
    WebFetch directo devuelve 403), incluyendo la tabla de indicadores,
    discusión y conclusiones.
  - Subtotal antes de penalizaciones: 20+12+5+0+2+5+10 = 54
  - Penalizaciones aplicadas:
    - Contexto poco comparable: no aplica (el sector es un match directo,
      ya reflejado con el máximo puntaje en ese componente).
    - Ausencia de implementación real detrás de resultados reportados: no
      aplica — no hay resultados reportados que aparenten sustento real sin
      tenerlo; el artículo declara abiertamente que es una propuesta no
      implementada (ya reflejado, sin duplicar, en "carácter aplicado" y
      "resultados cuantificables" = 0/20).
    - Resultados no verificables (afirmados sin sustento localizable en el
      texto): no aplica por la misma razón — no hay afirmaciones de
      resultado sin sustento, sino ausencia transparente de resultados.
    - **Información bibliográfica dudosa: -20.** Verifiqué yo mismo que el
      DOI declarado en la página del artículo, `10.23857/pc.v11i7.12063`,
      **no resuelve**: al consultar directamente `https://doi.org/10.23857/pc.v11i7.12063`
      obtuve HTTP 404 (probado por mí vía WebFetch el 2026-09-13). Autores,
      año, revista, volumen/número y páginas sí están razonablemente
      identificados a partir de los metadatos de la propia página fuente
      (confirmado antes por el researcher y no cuestionado por mí), pero el
      identificador DOI —un elemento central de identidad bibliográfica
      según CLAUDE.md sección 4— no resuelve a través del sistema oficial de
      DOI. Esto cumple literalmente el criterio de penalización de CLAUDE.md
      sección 6 ("no se pudo verificar... DOI"). Dejo esto explícito para que
      el orquestador lo pondere: no cuestiono el estado de verificación
      bibliográfica general asignado por `reference-verifier`
      (PARCIALMENTE VERIFICADO), solo aplico la tabla de penalizaciones de
      CLAUDE.md con este hallazgo adicional que verifiqué de forma
      independiente.
  - Score final: 54 - 20 = **34/100**
- Score final: **34/100**
- Recomendación: **NO ALCANZA UMBRAL** (34/100 < 60). El candidato no cruza
  el umbral orientativo de la sección 6 de CLAUDE.md. Es más útil como
  evidencia de contexto/diagnóstico (mismo sector, mismos síntomas que la
  MYPE) que como antecedente metodológico central de Línea 2, y además carga
  un hallazgo de integridad bibliográfica (DOI que no resuelve) que el
  orquestador debe considerar independientemente del score.
