# Control de eficiencia por ronda

Registro ligero para detectar si el pipeline se está profundizando
demasiado pronto en una ronda (`CLAUDE.md` secciones 16 y 20). **No se
estiman tokens ficticios** — solo se cuentan candidatos y se listan fuentes
bloqueadas/consultas ya intentadas, para evitar repetir trabajo.

## Rondas

| Ronda | Fecha | Researcher | Descubiertos | Descartados en prefiltro | Sobrevivientes | Enviados a verificación | Enviados a abstract screening | Enviados a full text | Finalistas | Fuentes bloqueadas | Verificaciones manuales pendientes | Notas |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| — | — | — | — | — | — | — | — | — | — | — | — | *(sin rondas todavía — pendiente de aprobación del usuario para iniciar Fase 1)* |

## Consultas / URLs ya intentadas

Registro para no repetir búsquedas equivalentes entre rondas. Formato por
entrada: `[fecha] [fuente/plataforma] — [consulta o URL] — [resultado breve:
N candidatos / bloqueado / sin resultados / pendiente manual]`.

*(Sin entradas todavía.)*

## Fuentes que requieren intento manual de la tesista

Registro de las cinco plataformas priorizadas (`CLAUDE.md` sección 11)
cuando no sean automatizables (login, interfaz conversacional sin API
accesible, bloqueo anti-bot persistente). Formato: `[plataforma] — [motivo]
— [qué buscar manualmente]`.

*(Sin entradas todavía.)*
