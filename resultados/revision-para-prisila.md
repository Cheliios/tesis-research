# Revisión para Prisila — Prueba controlada del pipeline (3 candidatos)

Este documento resume, únicamente a partir de la información ya generada por
el pipeline (`resultados/matriz-articulos.csv`, `resultados/verification-log.md`,
`resultados/descartados.md` y los archivos en `research/`), los 3 candidatos
de la prueba controlada. No se realizó ninguna búsqueda nueva ni se completó
ningún dato faltante para redactar este archivo. Todo lo que no fue
verificado por el pipeline aparece aquí como `NO VERIFICADO`.

Recordatorio de alcance: ninguno de estos 3 candidatos ha sido aprobado como
antecedente final de la tesis. `resultados/antecedentes.md` sigue vacío.

---

## L1-001 — BPR + simulación + VSM en confecciones (Vietnam)

1. **Título completo:** "Improving processing efficiency through workflow process reengineering, simulation and value stream mapping: a case study of business process reengineering"
2. **Autores:** Chia-Nan Wang; Tran Thi Bich Chau Vo; Hsien-Pin Hsu; Yu-Chi Chung; Nhut Tien Nguyen; Nhat-Luong Nhieu (verificados vía Crossref)
3. **Año:** 2024 (Crossref: `published-print` 2024-11-29, Vol. 30, No. 7)
4. **Revista:** *Business Process Management Journal* (Emerald Publishing), ISSN 1463-7154 (impreso) / 1758-4116 (electrónico)
5. **DOI:** 10.1108/BPMJ-11-2023-0869 — **resuelve correctamente** (confirmado vía API de Crossref y página de Emerald)
6. **URL disponible:** https://www.emerald.com/insight/content/doi/10.1108/bpmj-11-2023-0869/full/html
7. **Línea de investigación:** Línea 1 — Gestión de Procesos
8. **Herramienta/metodología:** Business Process Reengineering (BPR) multietapa, con Workflow Process Reengineering, Value Stream Mapping (VSM) y simulación de validación
9. **Contexto o sector estudiado:** empresa real de confecciones/vestuario (apparel) en Vietnam — manufactura textil, no reciclaje/PET/cartón
10. **Problema abordado:** ineficiencias de flujo de trabajo en la línea de costura; alta proporción de actividades sin valor agregado (NVA) y esenciales-sin-valor-agregado (ENVA)
11. **Resultados cuantitativos encontrados** (verificados por **ABSTRACT**, categoría B, citas casi textuales del resumen estructurado de Emerald):
    - 186 operaciones combinadas ENVA+NVA identificadas antes del rediseño
    - 25 operaciones eliminadas (15 ENVA + 10 NVA)
    - reducción del 8.5% en la proporción de operaciones ENVA
    - eliminación del 100% de las operaciones NVA identificadas
    - **No verificado en el cuerpo del texto** (paywall) — no hay confirmación en texto completo de estas cifras, solo en el abstract.
12. **Cuartil e indexación:**
    - Indexación Scopus: evidencia **indirecta únicamente** (mismo ID Scimago replicado en 3 agregadores independientes: Resurchify, Researcher.life, Editage; indicio adicional de Web of Science vía wos-journal.info). **No confirmado en fuente primaria** — Scopus.com, Scimago y Clarivate/JCR bloquearon el acceso automatizado en todos los intentos.
    - Cuartil: **Q1 como mejor cuartil reportado**, con variabilidad documentada entre categorías Scimago (una categoría consistentemente Q1; otra oscila Q1/Q2 según fuente/año, sin poder determinar cuál año corresponde a cada dato). Verificación **indirecta**, no primaria.
13. **Acceso disponible:** Metadata (categoría A) + Abstract (categoría B). **Sin acceso a texto completo** — confirmado directamente en la página real de Emerald: paywall pay-per-view de ~US$41.
14. **Score obtenido:** 64/100 (desglose: sector 10/20, problema-herramienta 16/20, carácter aplicado 10/15, resultados cuantificables 10/20, calidad académica 10/10, actualidad 5/5, evidencia disponible 3/10; sin penalizaciones adicionales)
15. **Estado:** **Candidato** (recomendación técnica del pipeline: "LISTO PARA DECISIÓN FINAL" — score ≥ 60 y estado de verificación PARCIALMENTE VERIFICADO). Esto no es una aprobación de antecedente final.
16. **Motivo del estado:** cumple el umbral de score con un caso real, implementado y validado por simulación, con resultados cuantitativos citables del abstract y calidad académica alta (Q1 indirecto). Se mantiene como "candidato" y no como "antecedente aprobado" porque queda una duda metodológica sin resolver (ver punto 17) y porque el texto completo no ha sido leído por nadie en el pipeline.
17. **Qué debería verificar manualmente Prisila antes de utilizarlo:**
    - **Ambigüedad Lean/BPR sin resolver:** el artículo usa Value Stream Mapping (herramienta de raíz Lean) y un marco de análisis NVA/ENVA propio de la tradición Lean, dentro de un paraguas declarado como BPR (no Lean Manufacturing/5S/Kaizen/Lean Six Sigma con ese nombre). El pipeline decidió no aplicar la exclusión automática de CLAUDE.md, pero dejó el caso marcado explícitamente como "revisar manualmente — mezcla de metodologías". **Esta es la decisión más importante que falta por confirmar.**
    - Conseguir acceso al texto completo (pago ~US$41 o vía biblioteca/institución) para confirmar que las cifras del abstract (186/25/8.5%/100%) efectivamente aparecen así en el cuerpo del artículo, y para poder describir la metodología con detalle (muestra, período, significancia).
    - Confirmar el cuartil y la indexación Scopus/WoS directamente en scimagojr.com o Scopus (el pipeline no pudo acceder a la fuente primaria por bloqueo anti-bot; todo lo que hay es indirecto vía agregadores).
    - Evaluar si la similitud sectorial (confección textil, no reciclaje) es suficiente para el estándar de la tesis, dado que la similitud es de tipo de problema (ineficiencias de flujo), no de sector físico.

---

## L1-002 — MES + KPIs en PYME manufacturera (Italia)

1. **Título completo:** "Manufacturing Execution System Application within Manufacturing Small–Medium Enterprises towards Key Performance Indicators Development and Their Implementation in the Production Line"
2. **Autores:** Augusto Bianchini; Ivan Savini; Alessandro Andreoni; Matteo Morolli; Valentino Solfrini (verificados vía Crossref)
3. **Año:** 2024
4. **Revista:** *Sustainability* (MDPI), vol. 16, núm. 7, artículo 2974
5. **DOI:** 10.3390/su16072974 — resuelve en Crossref (identidad bibliográfica confirmada por esta vía)
6. **URL disponible:** https://www.mdpi.com/2071-1050/16/7/2974 (bloqueada por HTTP 403 en todos los intentos automatizados)
7. **Línea de investigación:** Línea 1 — Gestión de Procesos
8. **Herramienta/metodología:** Manufacturing Execution System (MES) + marco de indicadores clave de desempeño (KPI) — **NO VERIFICADO** en detalle, solo a nivel de título
9. **Contexto o sector estudiado:** manufactura general / PYME, presuntamente Italia (afiliación inferida de un repositorio institucional de la Universidad de Bolonia, **NO VERIFICADO** de forma directa); no reciclaje/PET/cartón
10. **Problema abordado:** PYMEs manufactureras con obstáculos de presupuesto y adopción tecnológica para monitorear el desempeño de procesos — dato tomado de fragmentos agregados de búsqueda, **no de lectura directa de la fuente**
11. **Resultados cuantitativos encontrados:** **NO VERIFICADO**. Ninguna cifra de resultados fue reportada ni verificada; el propio pipeline documentó explícitamente que no debía asumirse ni inventarse ninguna mejora cuantificada.
12. **Cuartil e indexación:** **NO VERIFICADO** — el candidato fue descartado en la etapa de screening (score 39/100 < 40) y por protocolo no pasó a `reference-verifier`, por lo que nunca se intentó verificar cuartil ni indexación.
13. **Acceso disponible:** Solo metadata (categoría A, vía Crossref). **Ni siquiera hay certeza de haber visto el abstract real** — el resumen de contenido se reconstruyó de fragmentos agregados de WebSearch, no de lectura directa. Todos los intentos de acceso a la fuente (MDPI directo x2, variante /htm, PDF del repositorio institucional cris.unibo.it, ficha del mismo repositorio, ResearchGate, con WebFetch y con curl) devolvieron HTTP 403.
14. **Score obtenido:** 39/100 (desglose: sector 10/20, problema-herramienta 12/20, carácter aplicado 10/15, resultados cuantificables 0/20, calidad académica 2/10, actualidad 5/5, evidencia disponible 0/10)
15. **Estado:** **Descartado** (en la etapa de Screening, antes de verificación bibliográfica y antes de análisis de contenido)
16. **Motivo del estado:** score preliminar por debajo del umbral mínimo de 40/100, sin justificación excepcionalmente fuerte para mantenerlo. La base de evidencia es prácticamente nula: no se confirmó ni siquiera la lectura del abstract real, y no hay ningún resultado cuantificable reportado ni verificable.
17. **Qué debería verificar manualmente Prisila antes de utilizarlo:**
    - Este candidato **no debería usarse como antecedente en su estado actual**. Si Prisila quiere reconsiderarlo, el primer paso sería conseguir acceso real al artículo (es de acceso abierto en MDPI; el bloqueo detectado por el pipeline parece ser una restricción anti-bot del sitio hacia herramientas automatizadas, no un paywall real — es decir, una persona accediendo desde un navegador normal probablemente sí pueda leerlo).
    - Si se recupera el texto completo, habría que rehacer el screening desde cero con esa información (metodología real, resultados reales), ya que la evaluación actual se basó en información fragmentaria e insuficiente, no en una lectura real del artículo.

---

## L2-001 — Diagnóstico + FODA + KPIs propuestos en empresa recicladora (Quevedo, Ecuador)

1. **Título completo:** "Estrategias para optimizar el control de inventarios y fortalecer los procesos administrativos en una empresa recicladora de Quevedo, Ecuador"
2. **Autores:** Darwin Antonio Montoya Torres; Rosa Jamileth Cedeño Andrade; Jefferson Alberto Agurto Soria; Byron Fabricio Loor Párraga (Universidad Técnica Estatal de Quevedo, Ecuador)
3. **Año:** 2026 (recibido 10-jun-2026, aceptado 21-jun-2026, publicado 11-jul-2026)
4. **Revista:** *Polo del Conocimiento* (Casa Editora del Polo, Manta, Ecuador), Vol. 11, No. 7, pp. 906-923, ISSN 2550-682X
5. **DOI:** 10.23857/pc.v11i7.12063 — **declarado en la propia página del artículo, pero NO RESUELVE** (https://doi.org/10.23857/pc.v11i7.12063 → HTTP 404; Crossref → "Resource not found"). Se confirmó que el prefijo 10.23857 sí está activo en Crossref (2061+ DOIs de la misma revista) y que este DOI específico no está depositado, no es un bloqueo técnico.
6. **URL disponible:**
   - Vista del artículo: https://polodelconocimiento.com/ojs/index.php/es/article/view/12063
   - Texto completo (HTML): https://polodelconocimiento.com/ojs/index.php/es/article/view/12063/html
   - PDF: https://polodelconocimiento.com/ojs/index.php/es/article/download/12063/30739
7. **Línea de investigación:** Línea 2 — Control/Gestión de Inventarios
8. **Herramienta/metodología:** diagnóstico mixto (entrevistas + encuestas + observación directa, enfoque descriptivo-exploratorio, no experimental transversal) + análisis FODA/FODA cruzado + plan estratégico con KPIs propuestos. **No es un modelo cuantitativo clásico de inventarios** (no hay ABC, EOQ, punto de pedido, pronóstico de demanda ni Kardex implementado por los autores).
9. **Contexto o sector estudiado:** empresa recicladora de materiales reciclables (economía circular) en Quevedo, Ecuador — coincidencia directa de sector con la MYPE de la tesis.
10. **Problema abordado:** ausencia de registros sistemáticos de inventario, registros manuales, desorganización del almacenamiento, escasa capacitación del personal, bajo uso de herramientas tecnológicas para el control de inventarios — prácticamente un espejo de los problemas de la MYPE de la tesis.
11. **Resultados cuantitativos encontrados:** **NO DISPONIBLE / NO VERIFICADO.** Confirmado por lectura de **texto completo**: el artículo solo propone metas de KPIs a futuro (Tabla 4: exactitud de inventario ≥98%, rotación ≥8 veces/año, tiempo de registro ≤5 min, % material correctamente clasificado ≥95%, % cumplimiento de procedimientos ≥95%, % pérdidas por errores ≤2%, % cumplimiento de capacitaciones 100%), redactadas en futuro ("permitirán monitorear..."). **No hay ninguna medición real antes/después** — ni línea base ni resultado posterior. No se reporta ninguna mejora cuantitativa porque el artículo es propositivo, no evaluativo.
12. **Cuartil e indexación:**
    - Indexación: **ninguna en Scopus ni Web of Science detectada**, tras búsqueda activa. Solo aparece en Latindex (Catálogo 2.0), Dialnet y REDIB — ninguna equivale a Scopus/WoS ni asigna cuartil.
    - Cuartil: **NO VERIFICADO** — la revista no aparece en Scimago Journal Rank ni en JCR (búsqueda directa y búsqueda web dirigida, sin resultados).
13. **Acceso disponible:** **Texto completo** — leído de forma independiente por dos agentes distintos del pipeline (acceso directo bloqueado por HTTP 403; logrado vía `curl` con user-agent de navegador y vía proxy de lectura).
14. **Score obtenido:** 34/100 (desglose antes de penalización: sector 20/20, problema-herramienta 12/20, carácter aplicado 5/15, resultados cuantificables 0/20, calidad académica 2/10, actualidad 5/5, evidencia disponible 10/10 = 54; menos 20 de penalización por "información bibliográfica dudosa" — el DOI declarado no resuelve — = 34/100)
15. **Estado:** **Descartado** (no alcanza el umbral orientativo de 60/100 tras el análisis de contenido)
16. **Motivo del estado:** aunque el sector es un match directo (20/20) y el texto completo fue leído en su totalidad, la intervención central no es un modelo de inventarios implementado con resultados medibles, sino un diagnóstico con metas propuestas a futuro (carácter aplicado 5/15, resultados cuantificables 0/20). A esto se suma una penalización de -20 por un DOI declarado que no resuelve en el sistema oficial de DOI.
17. **Qué debería verificar manualmente Prisila antes de utilizarlo:**
    - **No usar este artículo como antecedente de un modelo de inventarios ya validado** — no lo es. Podría eventualmente citarse solo como evidencia de contexto/diagnóstico (mismo sector, mismos síntomas que la MYPE), nunca atribuyéndole resultados cuantitativos o una implementación real que el artículo no tiene.
    - Verificar directamente con la revista o con Crossref si el DOI 10.23857/pc.v11i7.12063 fue corregido/depositado posteriormente (es posible que sea un problema de registro tardío de la propia revista, no necesariamente una falsificación) antes de citarlo con ese DOI.
    - Confirmar independientemente que "Polo del Conocimiento" no tiene cuartil ni indexación Scopus/WoS si se necesita justificar por qué no cuenta como evidencia Q1/Q2 — el pipeline hizo una búsqueda activa pero no logró acceso directo a Scimago (bloqueo anti-bot).
    - Si se decide usar este artículo, clasificarlo explícitamente como evidencia complementaria de contexto (similar al tratamiento que CLAUDE.md da a tesis/repositorios), no como antecedente metodológico de Línea 2.

---

## Tabla comparativa resumida

| Criterio | L1-001 (Vietnam, BPR/VSM) | L1-002 (Italia, MES/KPI) | L2-001 (Ecuador, Diagnóstico/FODA) |
|---|---|---|---|
| Línea | Procesos | Procesos | Inventarios |
| Año | 2024 | 2024 | 2026 |
| Revista | Business Process Management Journal (Emerald) | Sustainability (MDPI) | Polo del Conocimiento |
| DOI | Resuelve | Resuelve (Crossref) | **No resuelve (404)** |
| Indexación Scopus/WoS | Indicio indirecto (no confirmado en fuente primaria) | NO VERIFICADO (no llegó a esta etapa) | Ninguna detectada |
| Cuartil | Q1 (mejor reportado), con variabilidad no resuelta | NO VERIFICADO | NO VERIFICADO (no encontrado en Scimago/JCR) |
| Acceso a la fuente | Metadata + Abstract (paywall en texto completo) | Solo metadata (ni el abstract está confirmado) | Texto completo |
| Resultados cuantitativos | Sí, verificados por abstract (186→25 operaciones, -8.5% ENVA, -100% NVA) | No verificados / no reportados | No disponibles (solo metas futuras, sin medición) |
| Carácter aplicado | Caso real implementado, con duda Lean/BPR abierta | Implementación indicada en el título, sin confirmar | Propuesta no implementada |
| Score final | **64/100** | 39/100 | 34/100 |
| Estado | **Candidato** (LISTO PARA DECISIÓN FINAL) | Descartado (screening) | Descartado (no alcanza umbral) |
| Principal pendiente para Prisila | Resolver ambigüedad Lean/BPR; conseguir texto completo; confirmar cuartil en fuente primaria | Conseguir acceso real al texto (probable solo bloqueo anti-bot, no paywall) | No usar como antecedente metodológico; verificar el DOI directamente con la revista |
