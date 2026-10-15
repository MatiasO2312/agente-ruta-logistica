# Diccionario de datos

## Columnas originales (`parcel_demand_scenario_1.csv`)
| Columna | Descripción |
|---|---|
| Latitute_pick_up, Longitude_pick_up | Coordenadas del punto de retiro (el encabezado original tiene un error de tipeo) |
| Latitude_delivery, Longitude_delivery | Coordenadas del punto de entrega |
| pickup_Start, pickup_End | Ventana horaria de retiro |
| delivery_Start, delivery_End | Ventana horaria de entrega |
| Weight | Peso del paquete (unidad no indicada; se asume kg) |
| Volume | Volumen del paquete (unidad no indicada; se asume m3) |

## Columnas calculadas (planificadas)
| Columna | Cómo se calcula |
|---|---|
| id_envio | Número de fila convertido en identificador |
| id_deposito | Según las coordenadas de retiro |
| distancia_km | Distancia en línea recta entre retiro y entrega |
| ventana_entrega_h | Fin de la ventana menos inicio |
| urgencia | Alta, media o baja según el ancho de la ventana |
| tiempo_viaje_min | Distancia dividida por la velocidad promedio (supuesta) |
| zona_id | Celda de 0,01 grados del destino |
| densidad_zona | Cantidad de entregas en la zona |
