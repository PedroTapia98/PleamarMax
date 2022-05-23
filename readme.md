# Cálculo de la pleamar máxima de un sitio de interés donde no hay datos mareográficos del lugar

### Pleamar máxima
Es el nivel más alto del agua registrado, debido a las oscilaciones de la marea astronómica y meteorológica, consideradas durante treinta días consecutivos con base en datos registrados o estimados durante diecinueve años o menos, según la disponibilidad de los mismos.

Para calcular el valor de la pleamar máxima en un sitio de interés que no esté especificado en las tablas numéricas de predicción de mareas de la Secretaría de Marina, se usará la ubicación de los 2 mareógrafos más cercanos en ambas direcciones de la costa. Se deberá obtener una estimación de la distancia lineal hacia cada uno de los dos mareógrafos y se implementará un cálculo de interpolación lineal empleando la siguiente ecuación:

 NPM = D1 X F1 + NP1
 
 Donde:
 
 - NPM = Nivel de pleamar máxima interpolado
 - D1 = Distancia lineal entre el sitio donde se desea conocer la marea y el primer mareógrafo de referencia en unidades de kilómetros
 - FI = Factor de interpolación en m/km
 - NP1 = Nivel de pleamar máxima de referencia indicado en las tablas numéricas de predicción de mareas de la Secretaría de Marina, en unidades de metros
 
 El factor de interpolación(FI) se cálcula como:
 
 FI = (NP2 - NP1) / (D1 + D2)
 
 Donde:
 - NP2 = Nivel de pleamar máxima indicado en las tablas numéricas de predicción de mareas de la Secretaría de Marina para el segundo mareógrafo
 - D2 = Distancia lineal desde el sitio de interés hacia el segundo mareógrafo

En este caso de cálcula la pleamar de máxima de un sitio en Veracruz usando los datos del mareógrafo de Veracruz y de Coatzacoalcos, el programa calcualrá las distancias teniendo las coordenadas geográficas del punto de interes y de los 2 mareógrafos y a partir de esto calcular la pleamar máxima. También se requiere ingresar los datos de nivel de pleamar máxima indicado en las tablas numéricas de predicción de mareas de la Secretaría de Marina de los mareógrafos usados.
