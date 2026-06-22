# tesis_ARALS_Sartorio20206

Repositorio de datos de la **Revisión Sistemática de Literatura (RSL)** sobre **Arquitecturas con Adaptación Runtime y Loop MAPE-K (ARALS)**, complementario al código fuente de la tesis de Alejandro S. Sartorio (2026).

## 📚 Tesis asociada

- **Título**: Arquitecturas con Adaptación Runtime y Loop MAPE-K — un estudio sistemático
- **Autor**: Alejandro S. Sartorio
- **Año**: 2026
- **Código fuente de la tesis**: [Tesis_Ale_2025-160p3-Fredy](https://github.com/wsf/Tesis_Ale_2025-160p3-Fredy)

## 📦 Contenido

| Carpeta | Contenido |
|---|---|
| `corpus/` | Corpus final (106 estudios), cadenas de búsqueda, log de screening |
| `protocol/` | Protocolo de la RSL pre-registrado |
| `prisma/` | Diagrama PRISMA 2020 del proceso |
| `results/` | Tabla de distribución, quality assessment, inter-rater agreement |

## ⚠️ Disclaimer — datos sintéticos

> Los **metadatos del corpus** (`corpus_final.csv` y `corpus_final.bib`) son **datos sintéticos** generados para documentar el proceso metodológico y permitir la replicabilidad de la SLR.
>
> Los títulos, autores, DOI y venues fueron generados automáticamente con fines demostrativos y **no representan publicaciones reales**. El protocolo de búsqueda, los criterios de screening y el quality assessment **sí reflejan el procedimiento real** documentado en la tesis.
>
> El **DOI del repositorio** será asignado posteriormente (próximamente vía Zenodo).

## 🔄 Replicabilidad

Para replicar la SLR siguiendo este repositorio:

1. Revisar `protocol/rsl_protocol.md` (criterios de inclusión/exclusión)
2. Ejecutar las 37 cadenas de búsqueda en `corpus/search_strings.md` sobre las 7 bases de datos
3. Aplicar las 2 rondas de screening según `corpus/screening_log.md`
4. Evaluar calidad con el scoring en `results/quality_assessment.csv`
5. Extraer datos según los campos en `corpus/corpus_final.csv`

## 📄 Licencia

- **Datos del corpus** (`corpus/`, `results/`): [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/)
- **Protocolo y PRISMA** (`protocol/`, `prisma/`): [MIT](https://opensource.org/licenses/MIT)

## 📖 Cómo citar

Ver [`CITATION.cff`](./CITATION.cff) — el DOI se agregará cuando se registre en Zenodo.

## 📞 Contacto

Alejandro S. Sartorio — alejandro.sartorio@gmail.com