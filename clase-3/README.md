# Clase 3 — Fine-tuning con LoRA

## Qué se aprende

- **Línea base:** medir cómo responde el modelo base antes de afinarlo, para poder comparar después.
- **Preparar los datos de entrenamiento:** ejemplos de entrada y salida con el tono o el comportamiento que se quiere enseñar.
- **LoRA:** ajustar solo una parte pequeña del modelo (adaptadores de bajo rango) en vez de reentrenarlo completo; se entrena rápido y con poca memoria.
- **Medir la mejora:** comparar las respuestas antes y después del ajuste con los mismos prompts.

## Challenge

Ajuste de tono con LoRA: afinar el modelo para que responda con un tono
definido y comprobar la diferencia contra la línea base.

## Notebooks

- `Modulo1_Clase3_HandsOn_COMENTADO_y_Ejemplo_Challenge_LoRA.ipynb` — versión Groq (PEFT/TRL).
- `GEN_2_Hands_On_Fine_Tuning_con_LoRA.ipynb` — Sesión 03, versión Gen 2 con Ollama.
- `Practica 3_ Fine-Tuning con LoRA.ipynb` — Sesión 03, versión Gen 1 con Groq.

La guía paso a paso en DOCX para el fine-tuning con LoRA está en el material
de apoyo (Drive).
