# Personal Discovery Engine

Personal Discovery Engine es un sistema inteligente de priorización y recomendación de contenido cuyo objetivo es ayudar al usuario a decidir qué información merece más la pena consumir según sus intereses, prioridades y tiempo disponible.

El proyecto combina ingesta de datos, validación, almacenamiento local, extracción de características y procesamiento semántico. Además, está diseñado para evolucionar incorporando embeddings, técnicas de machine learning y modelos LLM para generar explicaciones y resúmenes.

## Descripción general

El objetivo del proyecto es construir un sistema capaz de:

- recopilar contenido desde fuentes externas;
- validar y normalizar datos heterogéneos;
- evitar contenido duplicado;
- extraer características deterministas y semánticas;
- priorizar contenido según su relevancia;
- adaptar las recomendaciones a los intereses del usuario;
- tener en cuenta el tiempo disponible;
- generar explicaciones y resúmenes mediante LLMs.

El MVP actual está centrado inicialmente en contenido de noticias.

## Arquitectura actual

El flujo principal del sistema es:

APIs externas  
↓  
Ingesta de datos  
↓  
Validación con Pydantic  
↓  
Control de duplicados  
↓  
Almacenamiento en DuckDB  
↓  
Extracción de características  
↓  
Clasificación semántica  
↓  
Recomendación  
↓  
Explicaciones y resúmenes con LLMs

## Procesamiento semántico

Una de las áreas principales de desarrollo actual consiste en sustituir la clasificación simple basada en palabras clave por técnicas semánticas más robustas.

La evolución prevista incluye:

- generación de embeddings;
- comparación mediante similitud semántica;
- representación de temas e intereses;
- clasificación mediante machine learning;
- puntuación de relevancia;
- ranking personalizado según las preferencias del usuario.

El objetivo es que el sistema pueda comprender mejor el significado del contenido y no dependa únicamente de coincidencias exactas de palabras.

## Integración con LLMs

Los modelos LLM se plantean como una capa de razonamiento y explicación situada por encima del procesamiento determinista y semántico.

Estos modelos pueden:

- generar resúmenes concisos;
- explicar por qué se recomienda determinado contenido;
- aportar contexto adicional;
- mejorar la interacción con el sistema;
- generar explicaciones comprensibles para el usuario.

La arquitectura busca separar claramente la lógica determinista, el procesamiento semántico y el uso de LLMs.

## Tecnologías

- Python
- DuckDB
- Pydantic
- APIs REST
- Procesamiento de datos
- Machine Learning
- Embeddings
- Clasificación semántica
- LLMs

## Alcance de este repositorio

Este repositorio es una versión pública orientada a mostrar el proyecto dentro de mi portfolio profesional.

Aquí se incluye documentación, arquitectura y evolución del proyecto.

La implementación completa y el código fuente principal se mantienen en un repositorio privado.