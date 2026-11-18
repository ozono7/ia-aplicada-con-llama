# Clase 2 — Prompt Engineering y sistemas RAG

[Ver esta carpeta en nbviewer](https://nbviewer.org/github/ozono7/ia-aplicada-con-llama/tree/main/clase-2)

## Qué se aprende

- **Zero-shot vs. few-shot:** pedir una tarea sin ejemplos, o con ejemplos que muestran el formato esperado.
- **Chain-of-thought:** pedirle al modelo que razone paso a paso antes de responder.
- **El límite del prompt:** mejorar la instrucción no agrega conocimiento nuevo; cuando la respuesta depende de información que el modelo no vio, hace falta darle documentos.
- **RAG (Retrieval-Augmented Generation):** buscar el fragmento relevante en una base de conocimiento y entregárselo al modelo como contexto antes de responder.

## Challenge

Asistente de políticas con RAG: el asistente responde preguntas usando un
documento de políticas como fuente, en vez de inventar la respuesta.

## Notebooks

- `Modulo1_Clase2_HandsOn_COMENTADO_y_Ejemplo_Challenge_RAG.ipynb` — versión Groq. · [Abrir en Colab](https://colab.research.google.com/github/ozono7/ia-aplicada-con-llama/blob/main/clase-2/Modulo1_Clase2_HandsOn_COMENTADO_y_Ejemplo_Challenge_RAG.ipynb)
- `Hands_On_2_Prompt_Engineering_y_RAG_Comentado.ipynb` — Sesión 02, versión Gen 2 con Ollama en Colab. · [Abrir en Colab](https://colab.research.google.com/github/ozono7/ia-aplicada-con-llama/blob/main/clase-2/Hands_On_2_Prompt_Engineering_y_RAG_Comentado.ipynb)
- `GEN2_2_Ejemplo_challange__Prompt_Engineering_y_Sistemas_RAG.ipynb` — Sesión 02, ejemplo del challenge con Ollama. · [Abrir en Colab](https://colab.research.google.com/github/ozono7/ia-aplicada-con-llama/blob/main/clase-2/GEN2_2_Ejemplo_challange__Prompt_Engineering_y_Sistemas_RAG.ipynb)
- `Practica 2_ Prompt Engineering y Sistemas RAG.ipynb` — Sesión 02, versión Gen 1 con Groq. · [Abrir en Colab](https://colab.research.google.com/github/ozono7/ia-aplicada-con-llama/blob/main/clase-2/Practica%202_%20Prompt%20Engineering%20y%20Sistemas%20RAG.ipynb)
- `m1-c2-politicas-rag.ipynb` — Challenge 2 resuelto: asistente de políticas con RAG sobre el protocolo de cultivo del laboratorio (medio BG-11, OD680 cada 24 h, cosecha a 4,000 rpm/15 min), con búsqueda por similitud coseno y comparación con/sin RAG. · [Abrir en Colab](https://colab.research.google.com/github/ozono7/ia-aplicada-con-llama/blob/main/clase-2/m1-c2-politicas-rag.ipynb)
