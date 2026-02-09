# Segmentación Semántica de Heridas en Salmón del Atlántico mediante U-Net

## 📌 Descripción General

Este repositorio presenta el desarrollo de un anteproyecto de título en **Ingeniería Civil en Automatización**, cuyo objetivo es la implementación y evaluación de técnicas de **procesamiento digital de imágenes** y **aprendizaje profundo** para el análisis de la **reparación tisular en la piel del salmón del Atlántico** bajo distintas condiciones de temperatura.

El foco principal del proyecto es la **segmentación automática de heridas** presentes en imágenes digitales, utilizando una **red neuronal convolucional del tipo U-Net**, con el fin de obtener máscaras precisas que permitan un análisis cuantitativo reproducible y objetivo del proceso de cicatrización.

---

## 🎯 Objetivo

Desarrollar un modelo de segmentación semántica basado en la arquitectura **U-Net** que permita identificar automáticamente regiones de heridas en imágenes de salmón del Atlántico, mejorando la precisión y consistencia respecto a métodos clásicos de segmentación.

---
## 🏗️ Arquitectura del Modelo U-Net

El modelo propuesto se basa en la arquitectura **U-Net**, una red neuronal convolucional de tipo **encoder–decoder** con conexiones de salto (*skip connections*), diseñada para preservar información espacial de alta resolución.

### Características principales:

- Encoder:
  - Bloques de convolución 3×3
  - Activación ReLU
  - Max Pooling 2×2
- Decoder:
  - Deconvoluciones
  - Concatenación de mapas de características
- Normalización:
  - Batch Normalization posterior a cada convolución
- Salida:
  - Un solo canal correspondiente a la máscara binaria de la herida

  ![Estructura U-Net](/images/Propuesta_final1.png)


Esta arquitectura permite un equilibrio adecuado entre **precisión**, **robustez** y **eficiencia computacional**, siendo especialmente apropiada para aplicaciones con recursos limitados.

## 🛠️ Tecnologías Utilizadas

- Python
- PyTorch
- OpenCV
- NumPy
- Label Studio
- Google Colab (GPU)


