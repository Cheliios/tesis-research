# Manufacturing Execution System Application within Manufacturing Small–Medium Enterprises towards Key Performance Indicators Development and Their Implementation in the Production Line

- Autores: Bianchini, Augusto; Savini, Ivan; Andreoni, Alessandro; Morolli, Matteo; Solfrini, Valentino (verificados vía metadatos oficiales de Crossref, no vía lectura directa del texto completo)
- Año: 2024
- Fuente/plataforma: MDPI — revista *Sustainability*, vol. 16, núm. 7, artículo 2974
- Tipo: artículo científico
- URL: https://www.mdpi.com/2071-1050/16/7/2974
- DOI: 10.3390/su16072974
- Idioma: inglés

## Por qué podría ser relevante (razonamiento preliminar, no verificado)

Según el abstract (reconstruido a partir de metadatos de Crossref y fragmentos consistentes de búsqueda web, no de lectura directa del PDF/HTML completo), el artículo presenta la implementación de un **Manufacturing Execution System (MES)** en una PYME manufacturera real para desarrollar e implementar un marco de **indicadores clave de desempeño (KPI)** en la línea de producción, con enfoque en monitoreo de datos y evaluación del desempeño industrial (transición de "big data" a "smart data"). Esto se alinea con los temas de Línea 1 de CLAUDE.md: indicadores de procesos y gestión por procesos apoyada en datos, en el contexto de una MYPE/PYME manufacturera con las mismas limitaciones de recursos que la empresa caso de estudio (obstáculos de presupuesto y adopción tecnológica típicos de SMEs, mencionados explícitamente en el abstract).

**Advertencia honesta:** no pude verificar en el texto completo qué indicadores concretos se implementaron ni si hay cifras de resultados antes/después — el abstract disponible describe el enfoque y el propósito del sistema, pero no reporta explícitamente resultados cuantitativos. No se debe asumir ni inventar que hubo mejora cuantificada; eso queda `NO VERIFICADO` hasta que alguien con acceso al texto completo lo confirme.

Sector: manufactura general (SME, aparentemente europea/italiana a juzgar por la afiliación institucional en el repositorio de la Universidad de Bolonia), no reciclaje/PET/cartón. Igual que el otro candidato de esta prueba, se incluye por ampliación de sector (categoría 6 de prioridad de CLAUDE.md: MYPEs con problemas operacionales equivalentes — falta de indicadores, necesidad de sistematizar el monitoreo de procesos), tras no encontrar un candidato de reciclaje/PET/cartón verificable con estas características. Ver nota de ampliación en el resumen final de la tarea.

## Texto completo disponible

No — topé con bloqueo repetido (HTTP 403) al intentar abrir la página del artículo. Intenté WebFetch sobre: la URL directa de MDPI (dos veces), la variante `/htm`, el PDF alojado en el repositorio institucional de la Universidad de Bolonia (cris.unibo.it), la ficha del mismo repositorio, y la página de ResearchGate del artículo — todas devolvieron 403. También probé `curl` con user-agent de navegador de escritorio, con el mismo resultado. La identidad bibliográfica (título, autores, año, revista, volumen, número, página, DOI) se confirmó de forma independiente vía la API oficial de Crossref (api.crossref.org), que sí fue accesible. El resumen del contenido proviene de fragmentos de búsqueda agregados (WebSearch), no de una lectura directa del abstract completo en la fuente — esto se marca explícitamente como limitación, no como texto completo ni como abstract verificado de primera mano. *Sustainability* es una revista de acceso abierto (MDPI), por lo que el bloqueo observado parece ser una restricción anti-bot del sitio hacia herramientas automatizadas, no un paywall real.

## Nota de exclusión Lean (obligatoria)

No parece depender de Lean/5S/Kaizen/Lean Six Sigma como intervención principal — la intervención descrita en las fuentes disponibles es la implementación de un MES y un marco de KPIs, sin mención de metodologías Lean en ningún fragmento consultado. Esta conclusión se basa en información parcial (no se leyó el texto completo), así que si el cuerpo del artículo menciona Lean en algún punto no visible en el abstract, `paper-screener`/`reference-verifier` deberían confirmarlo al acceder al texto completo.

## Screening

No aplica exclusión Lean (Línea 1): ni el título ni los fragmentos
disponibles mencionan Lean/5S/Kaizen/Lean Six Sigma como intervención; la
intervención descrita es MES + marco de KPIs. No hay ambigüedad de mezcla de
metodologías que resolver aquí (a diferencia de L1-001).

El problema central de este candidato (punto 3 del encargo) es la
**disponibilidad de evidencia**: no hay texto completo ni siquiera certeza
de haber visto el abstract real — el propio researcher aclara que el
resumen de contenido "proviene de fragmentos de búsqueda agregados
(WebSearch), no de una lectura directa del abstract completo en la fuente".
Esto se refleja tanto en el componente de evidencia disponible (0/10, no
3/10) como, de forma conservadora, en los componentes de correspondencia
problema-herramienta y carácter aplicado, siguiendo la regla de "manejo de
información incierta" de `paper-screener.md` (nunca asumir el máximo por
beneficio de la duda).

- Sector/contexto: 10/20 — manufactura general / PYME (Italia, afiliación
  inferida de repositorio institucional, no reciclaje/PET/cartón). Encaja en
  el tramo "MYPE/manufactura físicamente comparable" por tratarse de una
  PYME manufacturera con limitaciones de recursos análogas (categoría 6 de
  prioridad de CLAUDE.md), no en un tramo superior de reciclaje directo.
- Problema-herramienta: 12/20 — el título (dato bibliográfico confirmado vía
  Crossref, no solo fragmentos) indica una correspondencia temática clara
  con "indicadores de procesos" de Línea 1 (MES + desarrollo e implementación
  de KPIs en una PYME manufacturera). Se puntúa de forma conservadora
  (12/20, no un tramo alto tipo 16-18) porque no hay confirmación directa
  del contenido real más allá del título/metadatos — el resumen de enfoque
  proviene de fragmentos agregados de búsqueda, no de lectura directa de la
  fuente, y no se puede confirmar el grado real de correspondencia
  metodológica.
- Carácter aplicado: 10/15 — el título mismo ("...and Their Implementation
  in the Production Line") indica implementación real en línea de
  producción, y este dato de título está confirmado vía Crossref, no
  inventado. Se puntúa por debajo del máximo (15) porque no hay verificación
  directa de los detalles de esa implementación en el cuerpo del texto.
- Resultados cuantificables: 0/20 — el propio researcher indica
  explícitamente que "no reporta explícitamente resultados cuantitativos" y
  que "no se debe asumir ni inventar que hubo mejora cuantificada". Sin
  información suficiente para acreditar ningún resultado, se asume el
  mínimo (0/20), no un valor intermedio.
- Calidad académica (preliminar, sin verificar cuartil aún): 2/10 — MDPI
  *Sustainability* es una editorial de interés listada en CLAUDE.md sección
  4, pero el cuartil no está verificado en esta etapa; tramo "cuartil no
  verificable".
- Actualidad: 5/5 — publicado en 2024.
- Evidencia disponible: 0/10 — a diferencia de un caso de "solo abstract"
  (que ameritaría 3/10), aquí ni siquiera hay certeza de haber visto el
  abstract real: todas las fuentes probadas devolvieron HTTP 403 y el
  resumen de contenido se reconstruyó de fragmentos agregados de WebSearch,
  no de una lectura directa. Sin información suficiente, se asume el
  mínimo (0/10), no el tramo de "solo abstract".
- Penalizaciones aplicadas: ninguna adicional sobre la tabla anterior (la
  falta de evidencia y de resultados verificables ya se refleja en los
  componentes "Resultados cuantificables" y "Evidencia disponible"; una
  penalización adicional duplicaría el mismo descuento).
- Score preliminar: 39/100
- Decisión: DESCARTADO
- Motivo (si DESCARTADO): Score preliminar por debajo del umbral mínimo
  (39/100 < 40). CLAUDE.md sección 6, criterio de `paper-screener.md`
  "Criterios de decisión": "Score preliminar < 40 → DESCARTADO salvo
  justificación explícita muy fuerte (documentar por qué se mantiene pese
  al score bajo)". No se identifica una justificación excepcionalmente
  fuerte que sostenga mantenerlo pese al score bajo: la correspondencia
  temática con Línea 1 es real, pero la base de evidencia es prácticamente
  nula (ni siquiera se confirmó la lectura directa del abstract, 403 en
  todas las fuentes probadas incluyendo el repositorio institucional y
  ResearchGate) y no hay ningún resultado cuantificable reportado ni
  verificable. Se descarta en screening; no pasa a `reference-verifier`.
