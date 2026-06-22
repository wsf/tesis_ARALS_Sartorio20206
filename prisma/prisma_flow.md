# PRISMA 2020 Flow Diagram

Diagrama de flujo del proceso de revisión sistemática, siguiendo la declaración **PRISMA 2020** \cite{page2021prisma}.

> **Nota**: Este es el diagrama en formato markdown. Para la versión visual (PDF/SVG) incluida en la tesis, ver `prisma_flow.pdf` y `prisma_flow.svg` en este repositorio.

---

## 📊 Identification (Phase 1)

```
┌─────────────────────────────────────────────────────────┐
│  Records identified through database searching         │
│  (n = 5,923)                                            │
└─────────────────────────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────┐
│  Records identified through other sources              │
│  (n = 47)                                               │
│  • Hand-search of key authors                          │
│  • Snowballing from seminal works                      │
│  • Recommendations from domain experts                 │
└─────────────────────────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────┐
│  Records screened (after deduplication)                │
│  (n = 3,734)                                            │
└─────────────────────────────────────────────────────────┘
```

---

## 🔬 Screening (Phase 2)

```
┌─────────────────────────────────────────────────────────┐
│  Records screened by title + abstract (Round 1)         │
│  (n = 3,734)                                            │
│                                                         │
│  Excluded (n = 3,058):                                  │
│  • Out of domain: 1,842                                │
│  • No empirical/SLR evidence: 487                      │
│  • Editorial / keynote: 318                            │
│  • Language out of scope: 234                          │
│  • Full text inaccessible: 177                         │
└─────────────────────────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────┐
│  Reports sought for retrieval (Round 2 — full text)     │
│  (n = 676)                                              │
│                                                         │
│  Excluded (n = 42):                                     │
│  • Full text not accessible after author request       │
└─────────────────────────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────┐
│  Reports assessed for eligibility (full text)          │
│  (n = 634)                                              │
│                                                         │
│  Excluded (n = 528):                                    │
│  • Tangential to MAPE-K only: 198                      │
│  • Insufficient technical detail: 142                  │
│  • Quality score < 0.55: 121                           │
│  • Duplicate across venues: 67                         │
└─────────────────────────────────────────────────────────┘
                          │
                          ▼
┌─────────────────────────────────────────────────────────┐
│  Studies included in corpus final                      │
│  (n = 106)                                              │
└─────────────────────────────────────────────────────────┘
```

---

## 📚 Citation

```
Page, M.J., McKenzie, J.E., Bossuyt, P.M., Boutron, I.,
Hoffmann, T.C., Mulrow, C.D., et al. (2021). The PRISMA
2020 statement: an updated guideline for reporting
systematic reviews. BMJ, 372, n71.
https://doi.org/10.1136/bmj.n71
```