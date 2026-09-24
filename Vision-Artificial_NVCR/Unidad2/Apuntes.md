
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

## 24/09

Un sistema embebido de visión integra captura y procesamiento en un solo dispositivo compacto, de bajo consumo y dedicado a una tarea específica

- Características clave: Tiempo real, tamaño y peso reducidos, bajo consumo energético, coto optimizado para producción en volumen.

- Plataformas comunes: Raspberry PI, NIVIDA  (Nano/Orin), microcontroladores con cámara (ESP32-CAM), FPGA, DSP y cámara inteligentes (smart cameras).
- Criterios de selección: Capacidad de cómputo (CPU/GPU/NPU), soporte de liberías (OpenCV, TensorRT), entradas/salidas disponibles, consumo y costo.

Tendencia actual: Aceleración por hardware (NPU/GPU) para inferencia de modelos de IA en el borde (edge AI)

- Analizar un sistema embebido implica evaluar tres dimensiones: El ambiente de desarrollo, los operadors disponibles y el proceso de generación de la aplicación.
- Objetivo: Decidir si una plataforma es viable para los requisitos de precisión, velocidad y consumo del proyecto.

Este análisis se realiza antes de comprometer recursos de diseño o producción.

- Conjunto de herramientas para rpogramar, compilar, depurar y desplegar en el sistema embebido.
- Componentes típicos: Sistema operativo (Linux embebido, RTOS o bare-metak), SDK del fabricante, compilador cruzado, IDE, drivers de cámara.

Ejemplos: Raspberry Pi OS + Python/OpenCV, NVIDIA JetPack + CUDA, entornos de desarrollo para FPGA (Vivado)/Quartus

# Actividad
## Tarea

Desarrollar un sistema de aprendizaje automático capaz de analizar imágenes retinianas y clasificar el nivel de riesgo de enfermedad renal crónica a partir de patrones presentes en la retina.
## Experiencia

El entrenamiento del modelo se realizará utilizando imágenes retinianas provenientes de bases de datos públicas empleadas en investigaciones científicas sobre detección de enfermedad renal crónica mediante inteligencia artificial. Entre los conjuntos de datos considerados se encuentran las imágenes utilizadas en estudios recientes basados en fotografías de fondo de ojo, complementadas con procesos de preprocesamiento y etiquetado para el entrenamiento supervisado del modelo. Adicionalmente, podrán utilizarse imágenes capturadas durante la fase experimental del prototipo para validar el funcionamiento general del sistema.
## Evaluación

El desempeño del sistema será evaluado mediante métricas de clasificación utilizadas en aprendizaje automático, incluyendo exactitud (Accuracy), sensibilidad (Recall), especificidad, precisión (Precision) y el área bajo la curva ROC (AUC), lo que permitirá determinar la capacidad del modelo para identificar correctamente patrones asociados con enfermedad renal crónica y comparar los resultados obtenidos con los reportados en investigaciones previas.