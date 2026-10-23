# 🦊 Capotis Study

**Capotis Study** es una aplicación móvil multiplataforma (Android e iOS) diseñada específicamente como un asistente de estudio local, minimalista y offline para estudiantes de ESO y Bachillerato. 

La aplicación integra procesamiento de texto local mediante **Google ML Kit** para escanear apuntes e imágenes, y un modelo de lenguaje local (`SmolLM2-360M`) optimizado para ejecutarse directamente en el dispositivo sin necesidad de conexión a internet ni servidores externos.

---

## 🚀 Características Principales

* **100% Offline y Privado:** Todo el procesamiento y almacenamiento de datos se realiza de forma local en el dispositivo del usuario. Sin fugas de datos ni servidores externos.
* **Asistente con IA Local:** Utiliza el modelo `SmolLM2-360M` (en formato `.gguf`) para generar explicaciones, resúmenes y resolver dudas de estudio.
* **Escaneo Inteligente (OCR):** Capacidad de extraer texto de imágenes y documentos PDF de hasta 20 páginas mediante Google ML Kit.
* **Planificación y Exámenes:** Herramientas integradas para organizar calendarios de estudio, flashcards y exámenes de práctica.
* **Lectura por Voz:** Soporte de síntesis de voz (*Text-to-Speech*) para la lectura de respuestas del asistente.

---

## 🛠️ Tecnologías Utilizadas

* **Framework:** Flutter / Dart
* **IA Local:** GGUF / Llama.cpp / SmolLM2-360M-Instruct
* **Gestión de Red y Archivos:** `dio`, `path_provider`, `shared_preferences`
* **OCR y Visión:** `google_mlkit_text_recognition`
* **Audio y Voz:** `flutter_tts`, `speech_to_text`

---

## 📥 Descarga del Modelo de IA

Para que la aplicación funcione al completo en local, es necesario descargar el archivo binario del modelo de IA (`smollm2-360m-instruct-q4_k_m.gguf`) y alojarlo en las **Releases** de este repositorio para que la app pueda descargarlo de forma automática en el primer arranque.

1. Descarga el modelo cuantizado desde [Hugging Face (SmolLM2-360M-Instruct-GGUF)](https://huggingface.co/HuggingFaceTB/SmolLM2-360M-Instruct-GGUF).
2. Súbelo a la sección de **Releases** de este repositorio bajo la etiqueta correspondiente (ej. `v1.0.0-model`).

---

## 📄 Licencia y Atribuciones

Este proyecto se distribuye bajo los términos de código abierto establecidos. 

* El software de la aplicación es propiedad de **Capotis Apps**.
* El modelo de lenguaje incorporado (**SmolLM2-360M**) ha sido desarrollado por *Hugging Face* y se distribuye bajo los términos de la licencia **Apache 2.0**. Puedes consultar los avisos legales completos dentro de los ajustes de la aplicación.

---

<p align="center">
  <b>Capotis Study · Desarrollado por Capotis Apps</b>
</p>
