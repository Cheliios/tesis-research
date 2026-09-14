# Antecedentes finales

Este archivo contiene **únicamente** antecedentes que:

1. Tienen estado de verificación `VERIFICADO` o `PARCIALMENTE VERIFICADO`
   (ver `verification-log.md`).
2. Fueron analizados por `paper-analyst` con clasificación `ANTECEDENTE
   FUERTE` o `RESERVA` (score y umbrales, ver `CLAUDE.md` sección 17) y
   recomendación `LISTO PARA DECISIÓN FINAL`.
3. Fueron aprobados explícitamente por el usuario junto con el orquestador.

Ningún subagente puede añadir una entrada aquí por su cuenta (ver
`CLAUDE.md` sección 5). Este archivo se llena manualmente por el
orquestador después de la aprobación del usuario.

Formato por entrada:

```markdown
## [ID] — [Título]

- Línea: [Procesos | Inventarios]
- Autores: 
- Año: 
- País: 
- Tipo de publicación: [artículo científico | tesis | repositorio]
- Revista/Universidad: 
- DOI: 
- URL: 
- Indexación: 
- Cuartil: [o "No aplica (tesis/repositorio)"]
- Fuente de verificación del cuartil: 
- Estado de verificación: [VERIFICADO | PARCIALMENTE VERIFICADO]
- Full text access: [OPEN_ACCESS | REPOSITORY_COPY | AUTHOR_MANUSCRIPT | ABSTRACT_ONLY | PAYWALL | AUTOMATION_BLOCKED | UNAVAILABLE]
- Sector/contexto: 
- Problema investigado: 
- Herramienta/modelo: 
- Metodología: 
- Implementation status: [IMPLEMENTADO | PILOTO_SIMULACION | NO_IMPLEMENTADO | TEORICO]
- Indicadores: 
- Resultado antes → después: 
- Result type: [RESULTADO_MEDIDO | RESULTADO_SIMULADO | META_PROPUESTA | RECOMENDACION | SIN_RESULTADO]
- Mejora cuantitativa: 
- Similitud con la MYPE: 
- Score de relevancia final: X/100
- Clasificación (CLAUDE.md sección 17): [ANTECEDENTE FUERTE | RESERVA]
- Conflicto metodológico (si aplica): 
- Motivo de inclusión (por qué el usuario lo aprobó): 
- Observaciones: 
```

---

*(Sin entradas todavía — pendiente de aprobación de investigación por el
usuario.)*
