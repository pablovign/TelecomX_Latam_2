Metodología

El análisis se llevó a cabo en varias etapas:

Análisis Exploratorio: se calculó la matriz de correlación entre las variables numéricas y la cancelación para identificar las relaciones iniciales.

Preprocesamiento: se aplicó el método SMOTE (Synthetic Minority Over-sampling Technique) sobre los datos de entrenamiento para balancear la clase minoritaria ("cancelado"), lo que asegura que los modelos no se sesguen.

Modelado: se entrenaron dos modelos de clasificación: un Árbol de Decisión y un Random Forest.

Evaluación: se comparó el rendimiento de ambos modelos utilizando métricas clave como la exactitud, la precisión, el recall, el F1-score y la matriz de confusión.

Análisis de importancia de variables: se identificaron las variables más influyentes en las predicciones del modelo.

Análisis y resultados clave

Rendimiento del modelo: el modelo de Random Forest superó consistentemente al Árbol de Decisión. Su F1-score de 0.58 para la clase de "cancelación" demuestra una mejor capacidad para equilibrar la precisión y la exhaustividad en la identificación de clientes en riesgo, en comparación con el 0.51 del Árbol de Decisión. Este resultado confirma que el Random Forest es una opción más confiable para este problema.

Factores Clave que influyen en la cancelación: el análisis de la importancia de las variables reveló los siguientes factores como los más influyentes en la predicción de la cancelación:

Antigüedad del cliente (cliente_antiguedad): es el factor más importante. Los modelos confirman que cuanto más tiempo un cliente ha estado con la compañía, menos probable es que cancele el servicio.
Cargos totales (cuenta_cargos_totales): esta variable es altamente significativa, lo que refuerza la conclusión anterior. Los clientes con un historial de gasto elevado son más propensos a ser leales.
Método de pago (cuenta_metodo_pago_Electronic check): los clientes que pagan con cheque electrónico tienen un riesgo significativamente mayor de cancelar. Esta es una variable crítica para segmentar a los clientes.
Tipo de contrato (cuenta_contrato_Two year): los clientes con contratos de dos años tienen una fuerte correlación negativa con la cancelación, lo que indica que es un factor de retención muy poderoso.
Servicio de Internet (internet_servicio_Fiber optic): los clientes con servicio de fibra óptica son un segmento de alto riesgo para la cancelación, lo que sugiere posibles problemas de satisfacción o precio en este tipo de servicio.
Cargos mensuales (cuenta_cargos_mensuales): el costo del servicio es un factor importante, lo que sugiere que los aumentos de tarifas o un precio percibido como alto pueden ser un catalizador para la cancelación.
Estrategias de retención propuestas

Se proponen las siguientes estrategias para mitigar la cancelación de clientes:

Fomentar la lealtad y la permanencia:

Ofrecer incentivos a la fidelidad a los clientes a medida que su antigüedad aumenta.
Implementar programas de reconocimiento para clientes de largo plazo.
Optimizar las ofertas de contrato:

Promover los contratos a dos años mediante descuentos o beneficios exclusivos, ya que es la variable con mayor poder predictivo para retener clientes.
Aumentar los esfuerzos de retención cuando los contratos mensuales se acercan al período en el que la mayoría de los clientes cancelan.
Monitorear y mejorar segmentos de alto riesgo:

Identificar a los clientes que usan el cheque electrónico y aquellos con servicio de fibra óptica para ofrecerles una atención al cliente proactiva y personalizada.
Realizar encuestas de satisfacción o contactar a estos segmentos para entender sus preocupaciones antes de que decidan cancelar.
Gestión de costos y servicios:

Analizar la competitividad de los precios, especialmente para los clientes con cargos mensuales elevados, para asegurar que el valor percibido justifique el costo.
