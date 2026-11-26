# Sistema analítico BI y Big Data - Clínica Jesús del Norte

Proyecto final del curso Base de Datos Avanzadas y Big Data (2026-2).



# Problemática:



La clínica no puede analizar de forma oportuna sus tiempos de atención, rentabilidad y satisfacción del usuario porque cada análisis recorre todo el volumen histórico de citas, pagos y facturación, sin mecanismos para reducirlo ni filtrar por fechas, tipo de pago, cantidad de citas o facturación de citas. Además, las causas de los retrasos y del malestar del paciente se registran como texto libre en bitácoras y libros de reclamaciones, aislado de los datos de facturación y farmacia, y su procesamiento sobre el volumen completo supera la capacidad de los sistemas transaccionales actuales. Por ello, se requiere una solución de Inteligencia de Negocios (BI) y una solución Big Data que modele indicadores estructurados (tiempos, tasas de cancelación, ingresos) sobre un subconjunto filtrado del volumen total y que procese de forma optimizada el texto histórico asociado a ese subconjunto para identificar patrones de fallas en el flujo de atención.



# KPIs:



* Ingresos totales: Suma de Suma\_TOTAL\_PAGO (monto autoritativo).
* Unidades vendidas: Volumen físico despachado.
* Pagos (tickets): Cada fila = una transacción de farmacia.
* Ticket promedio: Ingreso medio por transacción (44,730 / 861).
* Ticket máximo: La compra más grande registrada.
* Pacientes únicos: Clientes distintos que compraron al menos una vez.
* Farmacéuticos: Personal de farmacia que registró ventas.
* Medicamentos: Catálogo vendido.
* Billeteras digitales: YAPE + PLIN concentran casi la mitad de los ingresos.







## Requisitos

* Windows 11 con WSL2
* SQL Server 2022
* Power BI Desktop

## Estructura

* sql/: scripts DDL y consultas
* etl/: consultas de Power Query (ETL)
* bi/: dashboard de Power BI
* docs/: diagramas y diccionario de datos
* BigData/: procesamiento y análisis de Big Data
* ExperimentosDocumentados/: registro de los experimentos realizados

