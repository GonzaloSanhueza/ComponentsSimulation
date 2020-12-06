# Simulación de Préstamos

## Instrucciones del proyecto (simulación Monte Carlo)

En este problema, pronosticará el resultado de un portafolio de préstamos. Cada préstamo está calendarizado para ser repagado en 3 años y se estructura como sigue:

- Primero, el prestatario recibe los fondos. Este evento es llamado "origination".
- Después, el prestatario realiza pagos regulares, hasta que uno de los siguientes casos  ocurre:

i) El prestatario deja de pagar, típicamente debido a dificultades financieras, antes que del término de los 3 años. Este evento es llamado "charge-off", y se dice que el préstamo se canceló.

ii) El prestatario continúa pagando hasta 3 años después de la fecha de "origination". En este momento, la deuda ha sido pagada completamente.

En el [CSV adjuntado](https://github.com/bot13956/Monte_Carlo_Simulation_Loan_Status/blob/master/loan_timing.csv), cada fila corresponde a un préstamo, y las columnas se definen como sigue:

- La columna con encabezado "days since origination" indica el número de días que transcurrieron entre "origination" y la fecha en que los datos fueron recolectados.

- Para préstamos que cancelaron antes que los datos fueran recolectados, la columna con encabezado "days from origination to charge-off" indica el número de días transcurridos entre "origination" y "charge-off". Para los demás préstamos, esta columna no tiene valor.

OBJETIVO	
Queremos que estime qué fracción de estos préstamos se habrán cancelado para cuando terminen sus plazos de 3 años. Por favor, incluya una explicación rigurosa de cómo llegó a su respuesta, e incluya cualquier código que use. Podrá hacer uso de supuestos simplificadores, pero explique claramente.