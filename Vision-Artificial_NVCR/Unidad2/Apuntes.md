
# Actividad 2.1
# ¿Qué es la Visión Artificial?

Es el reconocimiento de patrones por medio de imágenes previamente etiquetadas para entrenamiento de un modelo. Es decir, al etiquetar, se indica que una imagen pertenece a algo, por lo que el modelo aprende que una futura imagen, es ese mismo algo si comparte las mismas características 


Ciclo de vida:

1. Definición del problema y requisitos
2. Adquisición de datos
3. Preprocesamiento de datos
4. Etiquetado/anotación de datos
5. Selección y diseño del modelo/algoritmo
6. Entrenamiento del modelo
7. Evaluación y validación
8. Optimización y ajuste
9. Implementación/despliegue

definición del problema
requerimientos funcionales 

### 21/09
# Arquitectura de un sistema de visión (parte 1)


- Un sistema de visión se compone de una cadena de bloques funcionales, no solo de una cámara
- Bloques principales: Iluminación, óptica/lente, sensor de imagen, interfaz de aquisión, unidad de procesamiento, salida/actuador.

Cada bloque impacta directamente la calidad del resultado final; un error en iluminación no se corrige después en software.

Flujo de datos: Captura, digitalización, transferencia (USB, GigE, MIPI, CameraLink), memoria, algoritmo, decisión/comunicación (PLC, red, actuador)
Criterios de diseño: Resolución requerida 
