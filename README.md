# YOLO Object Detection & Segmentation

Este repositorio contiene un proyecto de **detección de objetos** y **segmentación de instancias** con datasets de placas de vehículos y botellas obtenidos desde **Roboflow Universe**.

El objetivo es mostrar, paso a paso:

1. Cómo entrenar un modelo de **detección de objetos** con YOLO.
2. Cómo entrenar un modelo de **segmentación** con YOLO.
3. Cómo influye la **calidad del dataset** en las métricas (mAP, precisión, recall).

---

**DETECCIÓN DE PLACAS VEHICULARES (OBJECT DETECTION)**

1.1.Descripción: La detección de objetos consiste en identificar qué objeto aparece en una imagen y en qué ubicación, utilizando bounding boxes.

En este proyecto, se entrenó un modelo YOLO12x para: Detectar placas vehiculares en imágenes de autos.

1.2.Sobre el Dataset – Placas de Vehículos

Origen: Roboflow Universe

Tipo: Object Detection

Clase principal: license_plate

Características del dataset:

Imágenes con vehículos vistos desde diferentes ángulos.

Placas claramente visibles y anotadas correctamente.

Fondo moderado (calles, parqueos, tráfico).

🔗 https://app.roboflow.com/projectevelynsanchez/clean-yzsmx-o6xw6/1

1.3.Resultados:

mAP50: 0.995

mAP50-95: 0.817

Precisión: 0.998

Recall: 0.998

*El alto mAP50-95 confirma que las cajas generadas por el modelo se ajustan con gran exactitud a las anotaciones del dataset, reflejando una excelente calidad de entrenamiento.
*Las bounding boxes se ajustan bien incluso en vehículos inclinados.
*La calidad del dataset permite lograr buenos IoU en mAP50-95.

---
