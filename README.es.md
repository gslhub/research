<div align="center">

# GSLHub Research

### Búsqueda Generativa · GEO · Evaluación de IA · Investigación reproducible

**Protocolos canónicos, metodología, codebooks y materiales públicos de estudio de GSLHub**

[English](./README.md) · **Español**

[Web](https://gslhub.com) · [Plataforma](https://github.com/gslhub/website) · [Benchmarks](https://github.com/gslhub/benchmarks) · [Software](https://github.com/gslhub/software) · [Organización](https://github.com/gslhub)

[![Licencia: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

</div>

---

## Propósito

Este repositorio es la **capa metodológica canónica de investigación** de **GSLHub — Generative Search Lab Hub**.

GSLHub investiga cómo los sistemas de IA generativa **descubren, seleccionan, citan y recomiendan información**, con especial atención a la **Búsqueda Generativa** y la **Generative Engine Optimization (GEO)**.

El repositorio separa la metodología científica del código de aplicación que ejecuta y gobierna el flujo de investigación. De este modo, protocolos, codebooks, decisiones metodológicas y materiales de reproducibilidad pueden inspeccionarse, citarse y versionarse de forma independiente a la plataforma de software.

## Modelo canónico de investigación

```text
Problema científico
→ Hipótesis
→ Experimento
→ Ejecución controlada
→ Artefacto de investigación preservado
→ Evidencia
→ Observación
→ Cita / Métrica
→ Revisión de reproducibilidad
→ Difusión pública
```

Una métrica no se trata como un número aislado. Cuando la metodología lo exige, el resultado debe mantener trazabilidad mediante observaciones y ejecuciones gobernadas hasta la evidencia preservada.

Consulta la [`Matriz del Proyecto`](methodology/PROJECT-MATRIX.md).

## Enfoque actual de investigación

- **Búsqueda Generativa** — cómo los sistemas generativos recuperan, sintetizan y muestran información.
- **Generative Engine Optimization (GEO)** — factores asociados a selección de fuentes, citación y recomendación.
- **Evaluación de sistemas de IA** — comparación controlada del comportamiento de modelos/interfaces bajo condiciones registradas.
- **Visibilidad de fuentes** — resultados medibles de inclusión, citación, posición y consistencia.
- **Gobernanza de evidencia** — procedencia entre prompts, ejecuciones, artefactos, observaciones y métricas.
- **Reproducibilidad** — protocolos versionados, snapshots del entorno, controles de integridad y procedimientos de revisión.

## Métricas principales

| Código | Métrica | Propósito |
|---|---|---|
| **AIR** | Answer Inclusion Rate | Frecuencia con la que un target definido aparece en respuestas elegibles |
| **CR** | Citation Rate | Frecuencia con la que un target definido es citado en respuestas elegibles |
| **MCP** | Mean Citation Position | Posición media visible de la primera cita válida del target |
| **RCR** | Response Consistency Rate | Consistencia entre respuestas repetidas y controladas según la regla de codificación definida |

Las definiciones métricas y los resultados individuales se versionan por separado.

### Frontera entre especificación e implementación

Este repositorio define el **significado científico, las reglas de codificación y el contexto de protocolo**. Las especificaciones normativas versionadas del benchmark viven en [`gslhub/benchmarks`](https://github.com/gslhub/benchmarks), mientras que las implementaciones deterministas reutilizables viven en [`gslhub/software`](https://github.com/gslhub/software).

La primera implementación reutilizable, [`@gslhub/metrics-core`](https://github.com/gslhub/software/tree/main/packages/metrics-core), calcula AIR, CR, MCP y RCR de forma independiente de Payload CMS, MongoDB o Next.js. Sus tests automatizados reproducen el fixture sintético de validación publicado en el repositorio de benchmarks; esos valores son datos de validación de software, **no hallazgos empíricos de investigación**.

Esta separación permite una cadena auditable:

```text
significado científico / reglas de codificación
→ especificación de benchmark
→ implementación independiente
→ integración gobernada en plataforma
→ resultado de investigación validado
```

## Material metodológico canónico

### Modelo del proyecto

- [`methodology/PROJECT-MATRIX.md`](methodology/PROJECT-MATRIX.md) — modelo conceptual y operativo que conecta problema científico, hipótesis, experimentos, ejecuciones, evidencias, observaciones, citas, métricas y reproducibilidad.

### Primer piloto GEO controlado

- [`protocols/GSL-GEO-BENCH-01/PILOT-PROTOCOL-v0.1.0-ES.md`](protocols/GSL-GEO-BENCH-01/PILOT-PROTOCOL-v0.1.0-ES.md) — cinco repeticiones independientes controladas, preservación de evidencia, captura del contexto de ejecución, reglas de exclusión y cálculo de métricas.

### Codebook de observaciones y citas

- [`codebooks/OBSERVATIONS-CITATIONS-v0.1.0-ES.md`](codebooks/OBSERVATIONS-CITATIONS-v0.1.0-ES.md) — reglas formales de codificación, revisión, inclusión, exclusión y validación de observaciones y citas.

## Estructura del repositorio

```text
research/
├── protocols/       # Protocolos versionados de investigación y pilotos
├── studies/         # Definiciones públicas y documentación por estudio
├── codebooks/       # Reglas de codificación de observaciones, citas y evidencia
├── methodology/     # Principios metodológicos estables y gobernanza
├── templates/       # Plantillas reutilizables de estudios/protocolos
├── CITATION.cff     # Metadatos de citación del repositorio
├── LICENSE          # Texto legal CC BY 4.0
├── NOTICE.md        # Copyright, atribución y exclusiones
└── LICENSING.md     # Modelo de licencias por tipo de resultado
```

## Desarrollo frente a datos de investigación

GSLHub separa deliberadamente la **validación de desarrollo de software** de la **recogida científica de datos**.

```text
DESARROLLO
construir → probar → detectar → corregir → validar → limpiar

INVESTIGACIÓN
congelar protocolo → establecer baseline limpia → ejecutar → preservar → validar → analizar → publicar
```

Los registros TEST sintéticos y los fixtures deterministas nunca deben presentarse como hallazgos científicos.

## Principios de reproducibilidad

La investigación de GSLHub se diseña alrededor de:

- protocolos y definiciones métricas versionados;
- snapshots controlados del entorno de ejecución;
- sesiones aisladas cuando el protocolo lo exige;
- preservación de outputs raw e interfaces visibles;
- comprobaciones SHA-256 de integridad de artefactos;
- criterios explícitos de inclusión/exclusión;
- sellado del ciclo de vida de registros gobernados;
- almacenamiento persistente y verificación de recuperación;
- desviaciones documentadas en lugar de sustituciones silenciosas;
- revisión independiente cuando el diseño del estudio lo requiere.

Consulta [`methodology/REPRODUCIBILITY.md`](methodology/REPRODUCIBILITY.md) y [`methodology/GOVERNANCE.md`](methodology/GOVERNANCE.md).

## Licencias

Salvo que un archivo o resultado indique expresamente lo contrario, la **documentación original de investigación de este repositorio se publica bajo CC BY 4.0**.

Datasets, publicaciones, software, materiales de terceros y activos de marca GSLHub pueden utilizar licencias o condiciones distintas. Consulta [`LICENSE`](LICENSE), [`NOTICE.md`](NOTICE.md) y [`LICENSING.md`](LICENSING.md).

## Citación

El repositorio incluye [`CITATION.cff`](CITATION.cff). Cuando un estudio o publicación proporcione instrucciones de citación propias, debe citarse ese resultado específico además del repositorio cuando corresponda.

## Contacto

Colaboración científica y preguntas metodológicas: **research@gslhub.com**

---

© 2026 Eduardo Yauri · GSLHub — Generative Search Lab Hub
