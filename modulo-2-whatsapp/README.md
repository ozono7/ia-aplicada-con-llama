# Módulo 2 — Agentes conversacionales con Llama y WhatsApp

[Ver esta carpeta en nbviewer](https://nbviewer.org/github/ozono7/ia-aplicada-con-llama/tree/main/modulo-2-whatsapp)

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

- `02_Hands_On_Diseño_de_Agentes_Conversacionales_v1.ipynb` (Sesión 09). · [Abrir en Colab](https://colab.research.google.com/github/ozono7/ia-aplicada-con-llama/blob/main/modulo-2-whatsapp/02_Hands_On_Dise%C3%B1o_de_Agentes_Conversacionales_v1.ipynb)
- `Hands_On_Integración_entre_Llama_y_WhatsApp_(Solución)_COMENTADO.ipynb` — versión con function calling. · [Abrir en Colab](https://colab.research.google.com/github/ozono7/ia-aplicada-con-llama/blob/main/modulo-2-whatsapp/Hands_On_Integraci%C3%B3n_entre_Llama_y_WhatsApp_%28Soluci%C3%B3n%29_COMENTADO.ipynb)
- `m2-c1-estatus-pedidos-whatsapp.ipynb` — Challenge 1 resuelto: asistente de estatus de pedidos por WhatsApp (webhook con FastAPI, ngrok, saludo a usuarios nuevos). · [Abrir en Colab](https://colab.research.google.com/github/ozono7/ia-aplicada-con-llama/blob/main/modulo-2-whatsapp/m2-c1-estatus-pedidos-whatsapp.ipynb)
- `m2-c2-agente-veterinaria.ipynb` — Challenge 2 resuelto: agente de una veterinaria con memoria por número (Llama Stack), lock por número y regla de escalamiento. · [Abrir en Colab](https://colab.research.google.com/github/ozono7/ia-aplicada-con-llama/blob/main/modulo-2-whatsapp/m2-c2-agente-veterinaria.ipynb)
- `m2-c3-atencion-pedidos.ipynb` — Challenge 3 resuelto: agente de atención a pedidos con function calling (consultar_pedido, buscar_pregunta_frecuente), reglas de cargos y escalación. · [Abrir en Colab](https://colab.research.google.com/github/ozono7/ia-aplicada-con-llama/blob/main/modulo-2-whatsapp/m2-c3-atencion-pedidos.ipynb)
- `m2-hackathon2-agente-whatsapp.ipynb` — Hackathon 2 resuelto: agente de reservas de prácticas de laboratorio (UASLP FCQ) con function calling real, FAQ y capa de seguridad contra inyección de prompts. · [Abrir en Colab](https://colab.research.google.com/github/ozono7/ia-aplicada-con-llama/blob/main/modulo-2-whatsapp/m2-hackathon2-agente-whatsapp.ipynb)
- Proyecto demostrativo **El Comandero de Chida Café** (Sesión 04, carpeta Sensei en [clase-4/sensei/](../clase-4/sensei/)): mesero de WhatsApp con RAG sobre el menú, clasificador de mensajes con LoRA y app de Gradio.

Las guías paso a paso y el manual de ngrok y Meta están en el material de
apoyo (Drive).
