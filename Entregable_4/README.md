#  Entregable

##  Ejercicio pre-entregable: "AI Agent implementando RAG: decisión de modelo + implementación"

Contexto
El objetivo de esta práctica es consolidar la estructura lógica de un agente de IA haciendo uso de RAG. Deberás diseñar la solución técnica y estratégica antes de la implementación final en producción.

##  Pasos a seguir:

###  1) Definición del Caso de Uso: 
Describe el negocio y la función principal del bot (ej. agendamiento, soporte, FAQ), especifica el tipo de mensajes que recibirá

###  2) Justificación de Infraestructura (Local vs. Nube)
Analiza si usarás un modelo local (Ollama) o en la nube (OpenAI/Anthropic). Basa tu decisión en tres pilares: privacidad de datos, costos operativos y latencia.

### 3)Implementación del Pipeline de Ingesta
Implementación del Pipeline de Ingesta y Recuperación, cargá el documento base, procesalo y guardalo en la Vector Store con su correspondiente modelo de embeddings.

###  4)Configurá el nodo del LLM
Conectalo al retriever de la Vector Store para responder preguntas basándose exclusivamente en el contexto cargado
Ingeniería de Prompt: Redacta el System Prompt optimizado. Recuerda que el canal requiere brevedad y un tono específico. Define qué hacer cuando el agente no conozca una respuesta.

###  5)Análisis de Escalabilidad 
Respondé en 3-4 líneas: si el volumen de mensajes se multiplicara por 10, ¿tu decisión del punto 2 se sostiene? Indicá qué cambiarías en la arquitectura (local vs. nube) o en el flujo para sostener costo, privacidad y tiempos de respuesta.