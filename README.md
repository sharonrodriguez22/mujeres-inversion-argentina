# Mujeres e inversión en Argentina

Análisis de la evolución de la participación de las mujeres en el mercado de capitales argentino.

> Estado: 🚧 En desarrollo — etapa de revisión de fuentes.

## Pregunta principal

¿Cómo evolucionó la participación de las mujeres en el mercado de capitales argentino, qué cambios pueden observarse en sus patrones de inversión y qué factores podrían ayudar a explicar esa evolución?

Definición completa del proyecto: [`docs/project_definition.md`](docs/project_definition.md) · Variables necesarias: [`docs/variables.md`](docs/variables.md)

## Fuentes de datos

| ID | Institución | Qué mide | Período |
|----|-------------|----------|---------|
| SRC001 | BCRA | Adultos con cuentas bancarias / de pago, por género | T1 2019 – T4 2025 |
| SRC002 | BYMA | % de cuentas comitentes nuevas abiertas por mujeres | 2023 – 2025 |
| SRC003–005 | CNV | Informes de género (2021–2023) — sobre todo mujeres en directorios | 2021 – 2023 |
| SRC006–008 | INDEC | Contexto del mercado laboral (EPH) y metodología | 2016 – 2026 |

- Catálogo completo, limitaciones y alertas de calidad: [`docs/data_inventory.xlsx`](docs/data_inventory.xlsx)
- Ficha de cada fuente: [`docs/sources/`](docs/sources/)

## Estructura del proyecto

```
mujeres-inversion-argentina/
├── data/
│   ├── raw/          # Archivos originales, nunca se modifican
│   ├── processed/    # Tablas limpias (una fila = una observación)
│   └── external/     # Tablas de referencia (por ej. población)
├── notebooks/        # Análisis en Python
├── sql/              # Consultas SQL
├── powerbi/          # Dashboard
├── docs/             # Definición, inventario, fichas de fuentes
└── README.md
```

## Flujo de trabajo

1. **Revisión de fuentes** → catalogar cada fuente en el inventario ← *paso actual*
2. **Selección de variables** → definir qué indicadores responden la pregunta
3. **Limpieza** → `raw` → `processed`
4. **Análisis** → SQL + Python
5. **Dashboard** → Power BI
6. **Conclusiones**

## Criterios de calidad de datos

- Los archivos originales nunca se editan.
- No se agrega ninguna dimensión que la fuente no tenga (por ej., no hay columna `genero` en tablas sin desglose por género).
- Una relación entre inclusión financiera y participación en el mercado no se interpreta como causalidad.
- Las inconsistencias encontradas en las fuentes se registran en la columna `notas` del inventario.

## Herramientas

Excel · SQL · Python · Power BI

## Autora

Sharon Rodríguez Liendo
