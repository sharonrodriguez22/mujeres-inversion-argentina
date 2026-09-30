# BCRA

## Institución

Banco Central de la República Argentina

## Dataset

Tenencia de cuentas bancarias y de pago por género (hoja `2-1-2`).
Archivo: `data/raw/BCRA/inclusion-financiera-tenencia-cuentas-bancarias-pago-genero.xlsx`

## Qué mide

Cantidad de adultos (15 años o más) que tienen cuentas bancarias y/o cuentas de pago, por tipo de cuenta y género.

## Período

Marzo 2019 – diciembre 2025. Trimestral (28 trimestres).

## Unidad de observación

Cantidad de personas (CUIL/CUIT únicos de personas humanas) por trimestre, tipo de cuenta y género.

## Variables relevantes

- Sólo cuentas bancarias
- Sólo cuentas de pago
- Cuentas bancarias y de pago
- Al menos una cuenta bancaria
- Al menos una cuenta de pago
- Al menos una cuenta

## Desagregación por género

Sí: mujeres y varones. El género sale de los registros de AFIP.

## Limitaciones

- Son cantidades absolutas, no porcentajes: para calcular tasas hace falta un dato de población.
- Mujeres + varones < total: se excluyen titulares de género no binario o no informado.
- Solo cuenta cuentas de pago de proveedores registrados como PSP ante el BCRA.
- Mide tenencia de cuentas, **no** inversión.
- Las series pueden rectificarse (ver hoja "Notas" del archivo).

## Uso en el proyecto

Por evaluar. Candidata a fuente principal de inclusión financiera (es la serie con más datos).

## URL de origen

Pendiente (completar desde el sitio oficial).

---
Inventario: SRC001 en [`docs/data_inventory.xlsx`](../data_inventory.xlsx)
