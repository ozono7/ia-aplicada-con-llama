# Módulo 2 — Agentes conversacionales con Llama y WhatsApp

## Qué se aprende

- **Agente conversacional:** no solo responde una pregunta aislada; recibe mensajes, identifica al usuario, conserva el contexto y decide si responde con el modelo o aplica una regla fija.
- **Memoria por usuario:** un segundo mensaje puede depender del primero.
- **Function calling:** el modelo llama herramientas, por ejemplo consultar disponibilidad y preguntas frecuentes.
- **Despliegue:** webhook con FastAPI, túnel con ngrok y API de WhatsApp (Meta).

## Componentes

Ollama ejecuta Llama 3.1 dentro de Colab. Llama Stack administra las
conversaciones. FastAPI recibe las solicitudes del webhook. ngrok expone el
servidor temporalmente. La API de WhatsApp envía las respuestas.

Flujo: WhatsApp → Webhook → Regla / memoria → Llama 3.1 → Respuesta.

Las credenciales del proyecto (WHATSAPP_ACCESS_TOKEN, PHONE_NUMBER_ID,
NGROK_AUTHTOKEN, VERIFY_TOKEN) se guardan en Colab Secrets.

## Material

- `02_Hands_On_Diseño_de_Agentes_Conversacionales_v1.ipynb` (Sesión 09).
- `Hands_On_Integración_entre_Llama_y_WhatsApp_(Solución)_COMENTADO.ipynb` — versión con function calling.
- Proyecto demostrativo **El Comandero de Chida Café** (Sesión 04, carpeta Sensei en [clase-4/sensei/](../clase-4/sensei/)): mesero de WhatsApp con RAG sobre el menú, clasificador de mensajes con LoRA y app de Gradio.

Las guías paso a paso y el manual de ngrok y Meta están en el material de
apoyo (Drive).
