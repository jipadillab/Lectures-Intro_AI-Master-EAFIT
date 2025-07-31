# Contenido del archivo
markdown_content = """# 🤖 Introducción a Agentes Lógicos en Inteligencia Artificial

Este repositorio ofrece una introducción práctica y conceptual a los **agentes lógicos**, pensada para estudiantes que inician en ingeniería y desean aprender inteligencia artificial de forma progresiva y aplicada, utilizando Python.

---

## 🧠 ¿Qué es un Agente?

Un **agente** es cualquier entidad que puede percibir su entorno mediante sensores y actuar sobre él mediante actuadores.

Ejemplos:
- Un robot autónomo.
- Una app que recomienda productos.
- Un asistente inteligente que responde preguntas.

---

## 🔎 ¿Qué es un Agente Lógico?

Un **agente lógico**:
- Tiene una **base de conocimiento** (Knowledge Base - KB).
- Realiza inferencias lógicas para deducir nuevas verdades.
- Decide qué hacer basándose en lo que sabe y percibe.

---

## 🧩 Componentes de un Agente Basado en Conocimiento

| Componente   | Descripción |
|--------------|-------------|
| **Sensores** | Lo que percibe del entorno. |
| **Actuadores** | Acciones que puede ejecutar. |
| **Entorno** | Contexto donde actúa. |
| **KB (Base de conocimiento)** | Conjunto de oraciones o reglas conocidas. |
| **Inferencia** | Lógica usada para deducir nueva información. |
| **TELL** | Agrega conocimiento a la KB. |
| **ASK** | Consulta la KB para tomar decisiones. |

---

## 🧪 Actividad Conceptual Inicial

**Situación:** Estás en una habitación oscura y sientes una brisa.  
**Pregunta:** ¿Qué podrías deducir? ¿De dónde podría venir la brisa?  
Esto introduce el concepto de **inferencias** basadas en percepciones parciales.

---

## 🐍 Ejemplo Simple en Python

```python
# Base de Conocimiento
knowledge_base = []

# Operaciones TELL y ASK
def TELL(sentence):
    knowledge_base.append(sentence)

def ASK(query):
    return query in knowledge_base

TELL("No hay pozo en [1,1]")
TELL("Hay brisa en [1,2]")

print("¿Hay brisa en [1,2]? ", ASK("Hay brisa en [1,2]"))
print("¿Hay pozo en [1,1]? ", ASK("Hay pozo en [1,1]"))  # False
