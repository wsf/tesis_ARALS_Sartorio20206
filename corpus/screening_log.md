# Screening Log — 2 Rondas

Este documento registra el proceso de screening aplicado a los **3.734 registros** identificados tras la deduplicación inicial, siguiendo el protocolo PRISMA 2020.

---

## 📊 Resumen ejecutivo

| Fase | Criterio | Registros evaluados | Excluidos | Incluidos |
|---|---|---|---|---|
| **Round 1** | Título + Abstract | 3.734 | 3.058 | 676 |
| **Round 2** | Texto completo | 676 | 570 | **106** |

**Tasa de inclusión final**: 106 / 3.734 = **2.84%**

---

## 🔬 Round 1 — Screening por título y abstract

**Criterios de inclusión (cumplir al menos 1 de cada categoría)**:

| Categoría | Criterio |
|---|---|
| **Temático** | Aborda sistemas auto-adaptables, MAPE-K, o arquitecturas con adaptación runtime |
| **Temático** | Presenta framework, caso de estudio, o evaluación de adaptación |
| **Metodológico** | Emplea evidencia empírica (case study, experimento, simulación) o revisión sistemática |
| **Metodológico** | Publicación con peer-review verificable |

**Criterios de exclusión**:

| Categoría | Razón |
|---|---|
| **Temático** | Fuera del dominio (e.g., biología, sistemas biológicos no computacionales) |
| **Metodológico** | Sin evidencia empírica ni revisión sistemática (e.g., tutorial, opinion piece) |
| **Editorial** | Editorial, keynote, foreword, sin contenido técnico sustancial |
| **Idioma** | Idioma no cubierto por el equipo (fuera de EN/ES/PT/DE/FR) |
| **Acceso** | Texto completo no accesible tras 3 intentos |

**Resultado Round 1**: 676 estudios avanzan a Round 2.

### Razones de exclusión (Round 1)

| Razón | n | % de excluidos |
|---|---|---|
| Fuera de dominio temático | 1.842 | 60.2% |
| Sin evidencia empírica ni SLR | 487 | 15.9% |
| Editorial / keynote / foreword | 318 | 10.4% |
| Idioma fuera del alcance | 234 | 7.7% |
| Texto completo no accesible | 177 | 5.8% |
| **Total** | **3.058** | **100%** |

---

## 🔬 Round 2 — Screening por texto completo

**Criterios de inclusión (todos deben cumplirse)**:

| # | Criterio |
|---|---|
| 1 | Aborda explícitamente uno o más componentes MAPE-K (Monitor, Analyze, Plan, Execute, Knowledge) |
| 2 | Presenta evidencia empírica, framework, o evaluación de la adaptación en runtime |
| 3 | Aporta métricas, patrones, o análisis arquitectónico de la adaptación |
| 4 | Publicación peer-reviewed con rigor metodológico verificable |

**Criterios de exclusión**:

| Categoría | Razón |
|---|---|
| **Temático** | Aborda adaptación solo tangencialmente (menciona MAPE-K pero el foco es otro) |
| **Metodológico** | Sin suficientes detalles técnicos (e.g., solo menciona adaptación sin desarrollar) |
| **Calidad** | Calidad metodológica insuficiente (scoring < 0.55 en el quality assessment) |
| **Duplicado** | Duplicado del mismo estudio en múltiples venues (se conserva el más completo) |

**Resultado Round 2**: **106 estudios** conformar el corpus final.

### Razones de exclusión (Round 2)

| Razón | n | % de excluidos |
|---|---|---|
| Solo tangencial al MAPE-K | 198 | 34.7% |
| Detalles técnicos insuficientes | 142 | 24.9% |
| Calidad metodológica insuficiente | 121 | 21.2% |
| Duplicado en múltiples venues | 67 | 11.8% |
| No accesible tras solicitud al autor | 42 | 7.4% |
| **Total** | **570** | **100%** |

---

## 🎯 Distribución del corpus final por tipo de contribución

| Tipo | n | % |
|---|---|---|
| Empirical Case Study | 31 | 29.2% |
| Framework/Architecture | 24 | 22.6% |
| System Implementation | 18 | 17.0% |
| Evaluation/Comparison | 14 | 13.2% |
| Tool/Methodology | 8 | 7.5% |
| Literature Review | 7 | 6.6% |
| Position/Discussion | 4 | 3.8% |
| **Total** | **106** | **100%** |

---

## 📅 Distribución por año

| Rango | n | % |
|---|---|---|
| 2010–2014 | 7 | 6.6% |
| 2015–2019 | 21 | 19.8% |
| 2020–2024 | 78 | 73.6% |
| **Total** | **106** | **100%** |

---

## ⚠️ Disclaimer sobre roles R1/R2

> Los revisores R1 y R2 descritos en la Sección 2.2.3.1 de la tesis son **roles funcionales ejercidos por el autor** como estrategia de **revisión simulada por roles múltiples**, técnica utilizada en SLRs conducidas por un único investigador \cite{okoli2010guide, pautasso2013ten}.
>
> Esto significa que **una misma persona aplicó ambos perfiles** (R1 con foco en criterios temáticos, R2 con foco en rigor metodológico) en momentos distintos del proceso. El screening log documentado arriba refleja el resultado agregado de ambas pasadas.

---

## 📚 Referencias del protocolo

- **Okoli, C. & Schabram, K. (2010)**. A Guide to Conducting a Systematic Literature Review of Information Systems Research. *Sprouts: Working Papers on Information Systems*, 10(26), 1–49.
- **Pautasso, M. (2013)**. Ten Simple Rules for Writing a Literature Review. *PLoS Computational Biology*, 9(7), e1003149.
- **Page, M.J. et al. (2021)**. The PRISMA 2020 statement: an updated guideline for reporting systematic reviews. *BMJ*, 372, n71.