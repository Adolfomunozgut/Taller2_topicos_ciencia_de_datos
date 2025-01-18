# Predicción Automática de GRD en el Hospital El Pino con Aprendizaje Profundo

## Descripción

La optimización de la gestión hospitalaria es un desafío constante para los sistemas de salud en todo el mundo. En este contexto, los Grupos Relacionados por el Diagnóstico (GRD) han emergido como una herramienta fundamental para vincular a los pacientes con los recursos que consumen durante su estancia hospitalaria. Este sistema no solo mejora la planificación presupuestaria y la asignación de recursos, sino que también promueve una atención equitativa y eficiente. Sin embargo, su implementación efectiva enfrenta limitaciones significativas debido a errores humanos, tecnologías desactualizadas y la creciente complejidad de los diagnósticos y tratamientos médicos.

El aprendizaje profundo ha demostrado ser una tecnología clave para abordar estos desafíos, ofreciendo soluciones avanzadas para mejorar la precisión y eficiencia en la asignación de GRD. Modelos como las redes LSTM (Hochreiter & Schmidhuber, 1997) y Transformers (Vaswani et al., 2017) han revolucionado el procesamiento de datos secuenciales y la modelación de relaciones complejas. Estas arquitecturas, combinadas con técnicas modernas de interpretabilidad como SHAP y LIME, permiten no solo automatizar la clasificación, sino también generar explicaciones claras y comprensibles para el personal sanitario.

A nivel global, los sistemas de salud enfrentan una demanda creciente debido al envejecimiento de la población y el aumento en la prevalencia de enfermedades crónicas. La Organización Mundial de la Salud (OMS) proyecta que el gasto sanitario global deberá incrementarse en un 50% para 2030 solo para mantener los niveles actuales de atención (World Health Organization, 2022). En este escenario, herramientas como los GRD son esenciales para garantizar una distribución eficiente de los recursos. Sin embargo, estudios recientes han revelado que hasta el 15% de las asignaciones de GRD contienen errores de codificación, generando gastos innecesarios estimados en $30 mil millones anuales (Murphy et al., 2022).

En Chile, el gasto hospitalario constituye aproximadamente el 70% del presupuesto de la red pública de salud, pero este gasto no siempre se traduce en una atención eficiente y equitativa. El Hospital El Pino, perteneciente a la Red del Servicio de Salud Metropolitano Sur, enfrenta problemas como una ocupación de camas superior al 95%, inconsistencias en el 20% de las codificaciones de GRD y una limitada capacitación del personal responsable. Estas limitaciones no solo afectan la calidad de la atención, sino también la capacidad del hospital para planificar y optimizar sus recursos.

El presente informe se enfoca en el desarrollo de un sistema de predicción automática de GRD mediante técnicas avanzadas de aprendizaje profundo, evaluando arquitecturas como LSTM, Embeddings y Transformers. Este enfoque tiene como objetivo no solo mejorar la precisión en la clasificación de diagnósticos y procedimientos, sino también optimizar la asignación de recursos y reducir costos operativos en el Hospital El Pino. Además, busca contribuir a la equidad y sostenibilidad del sistema de salud chileno, ofreciendo una solución replicable para otros contextos hospitalarios.

## Modelos Entrenados

Se entrenaron varios modelos utilizando arquitecturas avanzadas de redes neuronales, tales como:

1. **LSTM (Long Short-Term Memory)**:
   - Utilizado para modelar secuencias de datos, como diagnósticos médicos y procedimientos a lo largo del tiempo.
   - Requiere datos secuenciales para realizar predicciones precisas en el contexto de GRD.

2. **Embeddings y Modelos de Redes Neuronales**:
   - Utiliza la técnica de Embeddings para representar de manera eficiente las palabras en vectores de características, facilitando la predicción de GRD.
   
3. **Transformers**:
   - Implementación de modelos basados en la arquitectura Transformer para capturar relaciones complejas en los datos médicos.

### Técnicas de Interpretabilidad

Para hacer que los modelos sean más interpretables para el personal sanitario, se utilizaron técnicas como **SHAP** y **LIME**, que permiten explicar las predicciones realizadas por el modelo de manera comprensible.

## Requisitos

Este proyecto fue desarrollado utilizando Python y requiere las siguientes bibliotecas:

- **TensorFlow / Keras** para la implementación de los modelos de aprendizaje profundo.
- **scikit-learn** para la evaluación del modelo y preprocesamiento de datos.
- **Matplotlib / Seaborn** para la visualización de resultados.

```bash
pip install tensorflow scikit-learn matplotlib seaborn
