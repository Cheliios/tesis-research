# Bitácora de verificación bibliográfica

Registro de cada verificación realizada por `reference-verifier`. Un
candidato puede tener más de una entrada si se re-verifica tras una
corrección o un nuevo intento de encontrar el cuartil.

Formato por entrada (ver detalle completo en `.claude/agents/reference-verifier.md`):

```markdown
## [ID] — [Título corto]

- Fecha de verificación: 
- Título verificado: [Sí/No + discrepancia si aplica]
- Autores verificados: [Sí/No/Parcial]
- Año verificado: [Sí/No]
- Revista/universidad verificada: [Sí/No]
- DOI verificado: [DOI confirmado / no tiene DOI / NO VERIFICADO]
- URL verificada: [Sí/No]
- Indexación: [Scopus / Web of Science / ambas / ninguna detectada / NO VERIFICADO]
- Cuartil: [Q1/Q2/Q3/Q4 / No aplica (tesis) / NO VERIFICADO]
- Fuente de verificación del cuartil: [nombre + año de edición consultado / No aplica]
- Estado final: VERIFICADO | PARCIALMENTE VERIFICADO | NO VERIFICADO
- Detalle de lo no verificado (si aplica): 
```

---

## L1-001 — BPR + simulación + VSM en confecciones (Vietnam, Emerald)

- Fecha de verificación: 2026-09-13
- Título verificado: Sí — "Improving processing efficiency through workflow
  process reengineering, simulation and value stream mapping: a case study
  of business process reengineering", coincide exactamente entre Crossref
  (API oficial `api.crossref.org/works/10.1108/BPMJ-11-2023-0869`, categoría
  A: metadata bibliográfica) y la página real de Emerald recuperada por
  WebFetch (categoría B: verificado por abstract — solo el resumen
  estructurado es visible).
- Autores verificados: Sí — Crossref y Emerald (dos fuentes independientes)
  coinciden en: Chia-Nan Wang, Tran Thi Bich Chau Vo, Hsien-Pin Hsu, Yu-Chi
  Chung, Nhut Tien Nguyen, Nhat-Luong Nhieu. Los nombres abreviados que trae
  el archivo del researcher ("Wang, C."; "Vo, T.T.B.C."; etc.) son
  consistentes con estos nombres completos, sin discrepancia.
- Año verificado: Sí — Crossref registra `published-print` 2024-11-29, Vol.
  30, No. 7 (categoría A).
- Revista/universidad verificada: Sí — *Business Process Management
  Journal*, Emerald, ISSN 1463-7154 (impreso) / 1758-4116 (electrónico), vía
  Crossref (categoría A). Se distinguió explícitamente de la
  *International Journal of Business Process Integration and Management*
  (SJR id 4700152810), un journal distinto con nombre parecido que apareció
  en las mismas búsquedas — no se confundieron.
- DOI verificado: DOI confirmado — 10.1108/BPMJ-11-2023-0869 resuelve
  correctamente en la API de Crossref (`status: ok`) y coincide con el DOI
  mostrado en la página de Emerald (categoría A, dos fuentes independientes:
  Crossref API + página del editor).
- URL verificada (resuelve y corresponde): Sí — la URL de Emerald resuelve
  (HTTP 200 vía WebFetch) y su contenido (título, autores, volumen, DOI,
  abstract) corresponde exactamente al candidato.
- Indexación: Scopus — evidencia INDIRECTA únicamente: el ID de Scimago
  (145291) para esta revista exacta aparece replicado de forma consistente
  en tres agregadores independientes entre sí (Resurchify, Researcher.life,
  Editage), y existe además una ficha específica en wos-journal.info
  (agregador especializado en el listado de Web of Science/JCR), lo que
  sugiere adicionalmente cobertura en Web of Science. **No se pudo
  confirmar accediendo directamente a Scopus.com, Scimago ni Clarivate/JCR**
  — los tres bloquearon el acceso automatizado (ver detalle). Por tanto esto
  se registra como indicio fuerte pero NO VERIFICADO de forma directa/primaria.
- Cuartil: Q1 como mejor cuartil reportado, con matiz importante — la
  categoría Scimago "Business, Management and Accounting (miscellaneous)"
  aparece como Q1 de forma consistente en las fuentes secundarias
  consultadas; la categoría "Business and International Management" aparece
  como Q2 en una página de Resurchify y como Q1 en otra página del mismo
  agregador (posiblemente años de edición distintos, no se pudo determinar
  cuál año corresponde a cada dato porque el acceso directo a Scimago quedó
  bloqueado). Siguiendo el criterio de no elegir el cuartil más favorable
  ante ambigüedad, este dato se registra como **Q1/parcial — variabilidad
  por categoría y posible año, ver detalle**, no como Q1 limpio.
- Fuente de verificación del cuartil: Intento primario — Scimago Journal
  Rank (scimagojr.com), intentado por tres vías independientes: WebFetch
  directo, `curl` con user-agent de navegador, y proxy de lectura
  (r.jina.ai) — las tres bloqueadas con HTTP 403 / pantalla de verificación
  anti-bot, sin poder leer la tabla de cuartil por año. Fuente secundaria
  usada en su lugar: agregadores que replican datos de Scimago/SJR
  (Resurchify id 145291, Researcher.life, Editage) — ninguno es la fuente
  primaria exigida por `reference-verifier.md`, por lo que el cuartil queda
  como verificación indirecta, no confirmada en la fuente primaria misma.
- Estado final: PARCIALMENTE VERIFICADO
- Detalle de lo no verificado (si aplica): (1) Texto completo NO
  disponible — confirmé directamente en la página real de Emerald (WebFetch)
  que el artículo está detrás de paywall (pay-per-view ~US$41), coincidiendo
  con lo que había reportado el researcher; solo el abstract estructurado es
  legible, por lo que los datos cuantitativos del abstract (186 operaciones
  ENVA/NVA, 25 eliminadas, reducción 8.5%, eliminación 100% de NVA) están
  verificados únicamente por abstract (categoría B), no por texto completo
  (categoría C) — no se afirma nada del cuerpo del artículo. (2) Afiliaciones
  institucionales de los autores: no verificadas (no visibles sin acceso al
  texto completo). (3) Indexación en Scopus/Web of Science: solo evidencia
  indirecta vía agregadores, no confirmada en la fuente primaria (Scopus,
  Scimago o Clarivate bloquearon el acceso automatizado). (4) Cuartil exacto:
  variabilidad entre categorías Scimago y posible variabilidad por año no
  resuelta por el mismo bloqueo de acceso — ver nota arriba.

---

## L2-001 — Control de inventarios en empresa recicladora de Quevedo (Polo del Conocimiento)

- Fecha de verificación: 2026-09-13
- Título verificado: Sí — "Estrategias para optimizar el control de
  inventarios y fortalecer los procesos administrativos en una empresa
  recicladora de Quevedo, Ecuador" coincide exactamente entre (a) el HTML
  real de la página del artículo obtenido de forma independiente vía `curl`
  con user-agent de navegador (metaetiquetas `citation_title`/`DC.Title`,
  categoría A) y (b) resultados de una búsqueda web independiente por el
  título que devolvió la misma ficha de Polo del Conocimiento con resumen de
  contenido coincidente (categoría B, no solo la palabra del researcher).
- Autores verificados: Sí — Darwin Antonio Montoya Torres; Rosa Jamileth
  Cedeño Andrade; Jefferson Alberto Agurto Soria; Byron Fabricio Loor
  Párraga, confirmados en las metaetiquetas `citation_author` del HTML de la
  fuente (categoría A), leídas de forma independiente (no copiadas del
  archivo del researcher).
- Año verificado: Sí — metaetiqueta `citation_date` = 2026/07/12 en el HTML
  fuente (categoría A), consistente con el volumen 11, número 7 (2026).
- Revista/universidad verificada: Sí — *Polo del Conocimiento*
  (`citation_journal_title`), ISSN 2550-682X (`citation_issn` /
  `DC.Source.ISSN`), confirmado en el HTML fuente (categoría A) y de forma
  cruzada en el registro de la revista en la API de Crossref
  (`api.crossref.org/journals/2550-682X`, que confirma título "Polo del
  Conocimiento", editorial "Polo de Capacitacion, Investigacion y
  Publicacion" y 2061-2062 DOIs registrados bajo ese ISSN) — dos fuentes
  independientes.
- DOI verificado: **NO VERIFICADO — hallazgo relevante.** El DOI
  10.23857/pc.v11i7.12063 aparece en las metaetiquetas de la propia página
  del artículo (`DC.Identifier.DOI`, `citation_doi`), pero **no resuelve**:
  `https://doi.org/10.23857/pc.v11i7.12063` devuelve HTTP 404, y la API
  oficial de Crossref (`api.crossref.org/works/10.23857/pc.v11i7.12063`)
  responde "Resource not found" (HTTP 404) — confirmado por dos vías
  independientes (WebFetch y `curl` directo). Se descartó que fuera un
  bloqueo anti-bot: el prefijo 10.23857 SÍ está activo en Crossref (revista
  con 2061+ DOIs registrados, incluyendo artículos del mismo volumen 11,
  número 7, como 10.23857/pc.v11i7.12065, 12001, 12043, 12138-12151, etc.),
  y se comprobó uno por uno el rango 12060-12066: solo 12065 resuelve
  (HTTP 200), el resto —incluido 12063— da 404. Es decir, la revista sí
  deposita DOIs en Crossref de forma rutinaria, pero este artículo
  específico no tiene su DOI registrado/depositado ahí (o el registro está
  pendiente), pese a que la propia plataforma OJS de la revista ya lo
  muestra como si existiera.
- URL verificada (resuelve y corresponde): Sí — la URL
  `https://polodelconocimiento.com/ojs/index.php/es/article/view/12063`
  resuelve (HTTP 200 vía `curl`; WebFetch directo dio 403, bloqueo anti-bot
  de la plataforma, no indicación de que la URL no exista) y su contenido
  (título, autores, fecha, ISSN, DOI declarado) corresponde exactamente al
  candidato. Es una URL institucional estable de la propia revista.
- Indexación: Ninguna en Scopus ni Web of Science detectada. Se buscó
  explícitamente evidencia de indexación en Scopus (no solo se aceptó la
  ausencia por defecto): múltiples búsquedas dirigidas no encontraron a
  "Polo del Conocimiento" en Scopus ni en Scimago. Sí se encontró en
  Latindex (Catálogo 2.0, ficha 23260), Dialnet (registro de revista) y
  REDIB — ninguna de estas tres es equivalente a Scopus/Web of Science ni
  asigna cuartil SJR/JCR (son directorios/repositorios de metadatos, no
  bases de indexación con cuartil). No se aceptó ninguna autodeclaración de
  la propia revista como prueba.
- Cuartil: NO VERIFICADO — la revista no aparece en Scimago Journal Rank
  (intentos de búsqueda directa por ISSN/nombre en scimagojr.com bloqueados
  por verificación anti-bot en WebFetch, `curl` y proxy r.jina.ai; búsquedas
  web dirigidas tampoco arrojaron ninguna ficha de Scimago para esta
  revista, a diferencia de lo que sí ocurrió para L1-001). Consistente con
  la hipótesis de partida del encargo: revista ecuatoriana multidisciplinaria
  de este tipo, sin cuartil real detectado. No se le asigna cuartil por
  default ni "No aplica" (eso es solo para tesis) — se registra
  explícitamente como no encontrado.
- Fuente de verificación del cuartil: Scimago Journal Rank — búsqueda
  directa por ISSN (2550-682X) y por nombre de revista, sin resultados
  encontrados en dos intentos independientes de acceso (bloqueo 403 en
  ambos); contraste adicional en MIAR (ficha de la revista existe pero no
  se pudo leer su contenido por error del servidor) y en Latindex/Dialnet/
  REDIB (ninguna asigna cuartil). No se encontró evidencia de cuartil en
  ninguna fuente confiable.
- Estado final: PARCIALMENTE VERIFICADO
- Detalle de lo no verificado (si aplica): El DOI específico
  10.23857/pc.v11i7.12063 no resuelve en doi.org ni en Crossref (ver
  detalle arriba) — se registra como identidad central confirmada por otra
  vía (URL institucional estable + metadatos de la propia página,
  corroborados por búsqueda web independiente) pero el DOI puntual queda sin
  confirmar, que es exactamente el escenario que `reference-verifier.md`
  define como PARCIALMENTE VERIFICADO (no NO VERIFICADO) cuando el
  documento es claramente localizable por otra vía. Adicionalmente,
  indexación Scopus/WoS y cuartil: no se encontraron en ninguna fuente
  confiable tras búsqueda activa (no es una omisión por falta de intento).
  Nota: la calidad/consistencia metodológica del contenido (si el
  diagnóstico + FODA + KPIs propuestos constituye o no un antecedente sólido)
  queda fuera del alcance de esta verificación bibliográfica — corresponde a
  `paper-analyst`.
