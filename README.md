# Isaac Run Predictor

Proyecto de fin de máster en fase inicial. La idea es crear un mod para *The Binding of Isaac: Repentance+* que estime qué probabilidad tienes de conseguir una marca de completado según cómo va la partida.

De momento, el proyecto se centra en preparar los datos. La primera prueba usa una partida real de Isaac en dificultad Hard, registrada con Isaac Run History. La notebook convierte esa exportación en un CSV con una fila por piso. El modelo y la integración con el menú de pausa quedan para más adelante.

## Cómo ejecutar la notebook

1. Coloca la exportación de Isaac Run History en `data/raw/save1.dat`.
2. En tu entorno de Python, instala las dependencias con `python -m pip install pandas ipykernel`.
3. Abre [02_preparacion_datos.ipynb](notebooks/02_preparacion_datos.ipynb), selecciona ese entorno y ejecuta todas las celdas. El resultado se guarda en `data/gold/isaac_floors.csv`.

La documentación de las entregas está en [docs/entregas](docs/entregas/).
