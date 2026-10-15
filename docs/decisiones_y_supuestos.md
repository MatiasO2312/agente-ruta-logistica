# Decisiones y supuestos

## Dataset
- Se eligió `parcel_demand_scenario_1.csv`: más de 5.000 registros y trae coordenadas, peso, volumen y ventanas horarias.
- El dataset ya llegó sin nulos ni duplicados, por lo que el trabajo se centra en validar y calcular columnas nuevas.
- Los otros archivos del paquete original quedan fuera por ahora.

## Datos generados
Hoy no hay datos generados (0 %). Lo que se genere se declarará aquí, con su justificación.

## Flota (propuesta, a confirmar)
Se propone una tabla aparte, `flota.csv`, con 5 a 10 vehículos simulados. Columnas: identificador, tipo
de vehículo, capacidad de peso, capacidad de volumen, velocidad promedio, depósito base y horario de la
jornada. Los valores se definirán en grupo y se declararán como datos generados.

## Supuestos
- Unidades: peso en kg y volumen en m3.
- Urgencia: alta si la ventana de entrega dura 4 horas o menos, media hasta 9 horas, baja si dura más.
- Zona: celda de 0,01 grados de latitud y longitud, cerca de 1 km.
- Velocidad promedio: 25 km/h (valor supuesto).
- La distancia se calcula en línea recta, no por calles.
