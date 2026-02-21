
# Embeddings y Preprocesamiento de Texto – LLMs desde cero

## Introducción

Este repo lo armé para entender, paso a paso y de forma práctica, cómo se procesan textos y se generan embeddings, siguiendo el Capítulo 2 de "Build a Large Language Model (From Scratch)" de Sebastian Raschka. El objetivo es desmenuzar el flujo real que usan los LLMs modernos, pero explicando cada parte en español y con ejemplos claros.

Me enfoqué en dos cosas:
- que el código y los notebooks sean fáciles de seguir (sin magia negra), y
- que las explicaciones cuenten una historia coherente sobre por qué cada paso importa para los modelos de lenguaje y sistemas agenticos.

## ¿Qué hay en este repo?

- **embeddings.ipynb**: Notebook principal. Incluye:
	- Importación de librerías (`torch`, `tiktoken`, etc.)
	- Carga y tokenización del texto base (`the-verdict.txt`)
	- División en fragmentos (chunks) con solapamiento
	- Construcción de embeddings con una capa de embedding de PyTorch
	- Experimento propio cambiando `max_length` y `stride` para ver el efecto del overlap
	- Explicaciones personales (en español) sobre cada paso y su relevancia para LLMs

- **the-verdict.txt**: Texto base (cuento corto, dominio público)

## Requisitos

- Python 3.x
- torch
- tiktoken

## ¿Cómo lo corrí en mi máquina (Windows)?

1. Abrí el notebook `embeddings.ipynb` en VS Code/Jupyter.
2. Ejecuté las celdas de arriba hacia abajo (Run All también funciona).
3. Si falta alguna librería, la instalé con `pip install torch tiktoken`.
4. Los outputs muestran los fragmentos, embeddings y resultados del experimento.

## Comentarios finales

El enfoque es didáctico y directo, sin rodeos. Si quieres entender cómo los LLMs "ven" el texto y por qué los embeddings son la base de todo, este notebook te lo muestra con ejemplos y explicaciones en español, sin perder el rigor técnico.

---

**Autor**: Esteban Aguilera Contreras  
**Universidad**: Escuela Colombiana de Ingeniería Julio Garavito  
**Asignatura**: Arquitecturas Empresariales (AREP)

