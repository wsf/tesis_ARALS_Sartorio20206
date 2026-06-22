# Protocolo de Revisión Sistemática de Literatura (RSL)

**Versión**: 1.0  
**Fecha**: Agosto 2024  
**Autor**: Alejandro S. Sartorio (wsf)  
**Marco metodológico**: Kitchenham & Charters (2007), PRISMA 2020 (Page et al., 2021)  
**Aplicación**: Tesis doctoral — Arquitecturas con Adaptación Runtime y Loop MAPE-K (ARALS)

---

## 1. Pregunta de investigación (PICo)

| Elemento | Descripción |
|---|---|
| **Population (P)** | Sistemas software auto-adaptables con loop MAPE-K |
| **Intervention (I)** | Arquitecturas, frameworks y patrones que habilitan adaptación runtime |
| **Comparison (C)** | Soluciones estáticas, sin auto-adaptación |
| **Outcomes (O)** | Latencia de adaptación, precisión de inferencia, estabilidad, overhead de monitoreo, tiempo de convergencia |

### Preguntas de investigación derivadas

- **RQ1**: ¿Qué patrones arquitectónicos se utilizan para implementar el loop MAPE-K en sistemas software auto-adaptables?
- **RQ2**: ¿Qué métricas se reportan para evaluar la calidad de la adaptación runtime?
- **RQ3**: ¿Qué desafíos y trade-offs emergen en la integración del componente de Knowledge?

---

## 2. Criterios de inclusión

### Criterios de inclusión (todos deben cumplirse)

| # | Criterio |
|---|---|
| 1 | Aborda explícitamente uno o más componentes del loop MAPE-K |
| 2 | Publicación con peer-review verificable |
| 3 | Presenta evidencia empírica (case study, experimento, simulación) o revisión sistemática |
| 4 | Publicada entre enero 2010 y diciembre 2024 |
| 5 | Idioma: inglés, español, portugués, alemán o francés |

### Criterios de exclusión

| # | Razón |
|---|---|
| 1 | Fuera del dominio MAPE-K / sistemas auto-adaptables |
| 2 | Sin evidencia empírica ni revisión sistemática (e.g., tutorial, opinion piece) |
| 3 | Editorial, keynote, foreword sin contenido técnico sustancial |
| 4 | Texto completo no accesible tras 3 intentos + solicitud al autor |
| 5 | Calidad metodológica insuficiente (scoring < 0.55) |

---

## 3. Estrategia de búsqueda

### Bases de datos consultadas (7)

- Scopus
- Web of Science (WoS)
- IEEE Xplore
- ACM Digital Library
- ScienceDirect
- SpringerLink
- Google Scholar (validación cruzada)

### Cadenas de búsqueda

Se ejecutaron **37 cadenas de búsqueda** distribuidas en 4 categorías:
- Categoría A — Core MAPE-K (12 queries)
- Categoría B — Frameworks y patrones (10 queries)
- Categoría C — Métricas y calidad (10 queries)
- Categoría D — Casos de estudio y validación (5 queries)

Ver `corpus/search_strings.md` para el detalle completo.

---

## 4. Proceso de screening

### Round 1 — Título + Abstract

- Aplicado a **3.734 registros** (post-deduplicación)
- Criterio: al menos 1 criterio temático + 1 criterio metodológico
- Resultado: **676 registros** avanzan a Round 2

### Round 2 — Texto completo

- Aplicado a **676 reportes** recuperados
- Criterio: los 4 criterios de inclusión estrictos
- Resultado: **106 estudios** conforman el corpus final

Ver `corpus/screening_log.md` para el log completo con razones de exclusión.

---

## 5. Quality Assessment

Cada estudio del corpus final fue evaluado con un scoring de **calidad metodológica** (rango 0–1) basado en 5 dimensiones:

| Dimensión | Peso |
|---|---|
| **Rigor metodológico** | 0.25 |
| **Relevancia temática** | 0.25 |
| **Evidencia empírica** | 0.20 |
| **Reproducibilidad** | 0.15 |
| **Claridad de la contribución** | 0.15 |

**Umbral mínimo de inclusión**: 0.55

Ver `results/quality_assessment.csv` para los scores individuales.

---

## 6. Extracción de datos

Para cada estudio incluido se extrajeron los siguientes campos:

- Identificador (study_id)
- Metadatos bibliográficos (título, autores, año, venue, DOI)
- Tipo de contribución (7 categorías)
- Idioma y open access
- Métricas reportadas (latencia, overhead, precisión, estabilidad, convergencia)
- Patrón arquitectónico del loop MAPE-K
- Caso de estudio o dominio de aplicación

---

## 7. Síntesis

La síntesis se realizó mediante **meta-análisis narrativo estructurado** (Popay et al., 2006), agrupando los estudios por:

- Tipo de contribución
- Componente MAPE-K focalizado
- Métrica evaluada
- Dominio de aplicación

Los resultados se presentan en las Secciones 3, 4 y 5 de la tesis (Capítulos 3, 4, 5).

---

## 8. Roles y simulación de revisión

> Los perfiles **R1 y R2** descritos en la Sección 2.2.3.1 de la tesis son **roles funcionales ejercidos por el autor** como estrategia de **revisión simulada por roles múltiples**, técnica utilizada en revisiones sistemáticas conducidas por un único investigador \cite{okoli2010guide, pautasso2013ten}.
>
> Esto significa que **una misma persona aplicó ambos perfiles** (R1 con foco en criterios temáticos, R2 con foco en rigor metodológico) en momentos distintos del proceso. El log de screening documenta el resultado agregado.

---

## 9. Limitaciones reconocidas

| Limitación | Mitigación |
|---|---|
| SLR de un único investigador | Revisión simulada por roles múltiples (R1/R2) |
| Posible sesgo de interpretación | Protocolo pre-especificado y revisado por director |
| Solo 7 bases de datos | Validación cruzada con Google Scholar |
| Rango temporal 2010–2024 | Justificado por la evolución reciente del campo MAPE-K |

---

## 📚 Referencias metodológicas

- Kitchenham, B. & Charters, S. (2007). *Guidelines for performing Systematic Literature Reviews in Software Engineering*. EBSE Technical Report.
- Page, M.J. et al. (2021). The PRISMA 2020 statement. *BMJ*, 372, n71.
- Okoli, C. & Schabram, K. (2010). A Guide to Conducting a Systematic Literature Review of Information Systems Research. *Sprouts: Working Papers on Information Systems*, 10(26), 1–49.
- Pautasso, M. (2013). Ten Simple Rules for Writing a Literature Review. *PLoS Computational Biology*, 9(7), e1003149.
- Popay, J. et al. (2006). Guidance on the conduct of narrative synthesis in systematic reviews. *ESRC Methods Programme*.