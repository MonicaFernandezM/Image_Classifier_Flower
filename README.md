🌸 Image Classifier - Flower Species

Este proyecto consiste en el desarrollo de un clasificador de imágenes que predice la especie de una flor a partir de una fotografía. Utiliza redes neuronales preentrenadas (transfer learning) para construir un modelo robusto de clasificación de imágenes.

⸻

🎯 Objetivo

Entrenar un modelo que, dado una imagen de flor, devuelva la clase o especie correspondiente, entre 102 categorías disponibles en el dataset.

⸻

🛠️ Tecnologías utilizadas
	•	Lenguaje: Python
	•	Frameworks: PyTorch, torchvision
	•	Entorno: Jupyter Notebook, Google Colab o consola local
	•	Red preentrenada: VGG16 

⸻

📦 Dataset
	•	Dataset de flores con 102 categorías
	•	Fuente: Oxford 102 Flower Dataset (descargado automáticamente mediante torchvision.datasets.ImageFolder)
	•	Imágenes divididas en:
	•	train/
	•	valid/
	•	test/

⸻

📌 Proceso
	1.	Carga y transformación de imágenes
	•	Transformaciones: redimensionamiento, normalización y aumentos
	•	Uso de DataLoader de PyTorch
	2.	Construcción del modelo
	•	Congelar pesos de red preentrenada
	•	Agregar capa clasificadora (classifier) personalizada
	3.	Entrenamiento y validación
	•	Optimización con Adam
	•	Función de pérdida: CrossEntropyLoss
	•	Validación en cada epoch
	4.	Evaluación
	•	Precisión sobre el conjunto de test
	•	Predicción individual de imágenes usando la función predict
	5.	Guardado y carga del modelo
	•	Checkpoint: arquitectura, pesos, clase a índice

⸻

✅ Resultados
	•	Se logró una precisión de test superior al 80%
	•	El modelo puede predecir correctamente la especie de una flor con solo una imagen como entrada
