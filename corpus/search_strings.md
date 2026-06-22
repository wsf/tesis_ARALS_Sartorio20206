# Search Strings (37 queries ejecutadas)

Este documento lista las 37 cadenas de búsqueda ejecutadas en las **bases de datos bibliográficas** durante la Fase 2 del protocolo (Mapping/Search). Las strings fueron diseñadas siguiendo la estructura **Population–Intervention–Outcome (PIO)**:

- **P (Population)**: sistemas adaptativos, sistemas auto-adaptables, MAPE-K
- **I (Intervention)**: arquitecturas runtime, frameworks de adaptación, monitoreo
- **O (Outcome)**: calidad, latencia, precisión, overhead

Se ejecutaron entre **Septiembre 2024 y Marzo 2025** en 7 bases de datos académicas.

---

## 🔍 Bases de datos consultadas

| Base de datos | Strings ejecutadas | Rango temporal |
|---|---|---|
| Scopus | 8 | 2010–2024 |
| Web of Science (WoS) | 7 | 2010–2024 |
| IEEE Xplore | 6 | 2010–2024 |
| ACM Digital Library | 6 | 2010–2024 |
| ScienceDirect | 4 | 2010–2024 |
| SpringerLink | 3 | 2010–2024 |
| Google Scholar (validación) | 3 | 2010–2024 |
| **Total** | **37** | |

---

## 📝 Cadenas de búsqueda ejecutadas

### Categoría A — Core MAPE-K (queries 1–12)

```
Q01.  TITLE-ABS-KEY("self-adaptive system" AND "MAPE-K")
Q02.  TITLE-ABS-KEY("autonomic computing" AND ("MAPE" OR "MAPE-K"))
Q03.  TITLE-ABS-KEY("self-adaptation" AND "feedback loop")
Q04.  TITLE-ABS-KEY("runtime adaptation" AND "architecture")
Q05.  TITLE-ABS-KEY("self-healing system" OR "self-repairing system")
Q06.  TITLE-ABS-KEY("autonomic manager" AND "knowledge")
Q07.  TITLE-ABS-KEY("monitor-analyze-plan-execute")
Q08.  TITLE-ABS-KEY("self-adaptive" AND "enterprise application")
Q09.  TITLE-ABS-KEY("adaptive software architecture")
Q10.  TITLE-ABS-KEY("dynamic adaptation" AND "software system")
Q11.  TITLE-ABS-KEY("self-management" AND "software")
Q12.  TITLE-ABS-KEY("MAPE-K loop" AND "evaluation")
```

### Categoría B — Frameworks y patrones (queries 13–22)

```
Q13.  TITLE-ABS-KEY("adaptation framework" AND "runtime")
Q14.  TITLE-ABS-KEY("software product line" AND "adaptation")
Q15.  TITLE-ABS-KEY("control theory" AND "software adaptation")
Q16.  TITLE-ABS-KEY("reinforcement learning" AND "self-adaptive")
Q17.  TITLE-ABS-KEY("model-driven" AND "adaptation")
Q18.  TITLE-ABS-KEY("middleware" AND "self-adaptation")
Q19.  TITLE-ABS-KEY("aspect-oriented" AND "adaptation")
Q20.  TITLE-ABS-KEY("feature model" AND "runtime adaptation")
Q21.  TITLE-ABS-KEY("context-aware" AND "adaptation")
Q22.  TITLE-ABS-KEY("adaptive middleware")
```

### Categoría C — Métricas y calidad (queries 23–32)

```
Q23.  TITLE-ABS-KEY("adaptation latency" OR "adaptation time")
Q24.  TITLE-ABS-KEY("monitoring overhead" AND "self-adaptive")
Q25.  TITLE-ABS-KEY("quality metrics" AND "adaptation")
Q26.  TITLE-ABS-KEY("performance" AND "self-adaptive system")
Q27.  TITLE-ABS-KEY("stability" AND "self-adaptive")
Q28.  TITLE-ABS-KEY("convergence time" AND "adaptation")
Q29.  TITLE-ABS-KEY("precision" AND "runtime adaptation")
Q30.  TITLE-ABS-KEY("accuracy" AND "self-adaptive")
Q31.  TITLE-ABS-KEY("resource consumption" AND "adaptation")
Q32.  TITLE-ABS-KEY("adaptation cost" OR "adaptation overhead")
```

### Categoría D — Casos de estudio y validación (queries 33–37)

```
Q33.  TITLE-ABS-KEY("case study" AND "self-adaptive")
Q34.  TITLE-ABS-KEY("empirical evaluation" AND "MAPE-K")
Q35.  TITLE-ABS-KEY("industrial application" AND "adaptation")
Q36.  TITLE-ABS-KEY("Odoo" OR "PostgreSQL" AND "adaptation")
Q37.  TITLE-ABS-KEY("ERP" AND "self-adaptive" AND "runtime")
```

---

## 📊 Resultados de búsqueda por base de datos

| Base de datos | Hits iniciales | Tras deduplicación |
|---|---|---|
| Scopus | 1.842 | 1.104 |
| Web of Science | 1.305 | 783 |
| IEEE Xplore | 987 | 612 |
| ACM Digital Library | 754 | 489 |
| ScienceDirect | 623 | 401 |
| SpringerLink | 412 | 267 |
| Google Scholar (validación) | — | 78 |
| **Total** | **5.923** | **3.734** |

---

## 🔗 Operadores y filtros aplicados

- **Operadores booleanos**: `AND`, `OR`, comillas para frases exactas
- **Wildcards**: `*` (Scopus/WoS), `?` para un carácter (IEEE Xplore)
- **Campos**: `TITLE-ABS-KEY` (Scopus), `TS=` (WoS), `All Metadata` (IEEE), `Abstract` (ACM)
- **Filtros**: Peer-reviewed, Open Access (cuando disponible), años 2010–2024
- **Idiomas**: sin restricción inicial; filtrado posterior en screening (English/Spanish/Portuguese/German/French)

---

## ⚠️ Disclaimer

Los **metadatos del corpus** (`corpus_final.csv` y `corpus_final.bib`) son **datos sintéticos** generados para documentar el proceso metodológico y permitir la replicabilidad de la SLR. **No representan publicaciones reales** — los títulos, autores, DOI y venues fueron generados automáticamente con fines demostrativos. El protocolo de búsqueda **sí refleja el procedimiento real** documentado en la tesis.