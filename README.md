# Semana-9-
Implementación de Data Augmentation y Transfer Learning en Imágenes en Google Colab
2. Impacto en la Capacidad de Generalización
La generalización es la habilidad del modelo para rendir bien en datos que nunca ha visto. Aquí es donde ambas técnicas funcionan por razones distintas:

A. Data Augmentation: Regularización a través de la Diversidad
El aumento de datos actúa como un regularizador. Obliga al modelo a ser "invariante". Por ejemplo, si se aplica rotación y brillo a la imagen de un auto, el modelo aprende que un auto sigue siendo un auto independientemente de su orientación o de si es de día o de noche.

Impacto: Reduce la brecha entre el error de entrenamiento y el error de validación.

Justificación: Evita que la red neuronal aprenda atajos estadísticos (como patrones de píxeles específicos en una esquina de la imagen).

B. Transfer Learning: Generalización mediante el Conocimiento Previo
El impacto aquí es estructural. Al reutilizar un modelo como ResNet o MobileNet, no se empieza desde una "pizarra en blanco" (inicialización aleatoria), sino desde un punto óptimo en el espacio de pesos.

Impacto: El modelo hereda la capacidad de generalización de un dataset masivo (ImageNet).

Justificación: Los filtros preentrenados ya son expertos en detectar conceptos universales (geometría, profundidad), lo que estabiliza el aprendizaje en problemas específicos.
