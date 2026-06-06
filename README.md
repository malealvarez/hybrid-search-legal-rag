# Sistema de Búsqueda Híbrida + Re-ranking sobre Ley de Contrato de Trabajo (Argentina)

## Descripción del proyecto

Este proyecto implementa un sistema de recuperación de información (Information Retrieval) sobre la Ley de Contrato de Trabajo de Argentina, combinando técnicas modernas de NLP para mejorar la precisión en la búsqueda de información legal.

El sistema simula un pipeline de tipo **RAG (Retrieval-Augmented Generation)** utilizando múltiples estrategias de recuperación y un modelo de re-ranking.

---

## Arquitectura del sistema

El pipeline está compuesto por las siguientes etapas:

- Ingesta y preprocesamiento del documento legal
- Chunking con overlap para preservar contexto
- Generación de embeddings semánticos
- Indexación vectorial con FAISS
- Indexación léxica con BM25
- Búsqueda híbrida mediante fusión de rankings (RRF)
- Re-ranking con Cross-Encoder para refinamiento final

---

## Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Sentence Transformers
- FAISS
- Rank-BM25
- Scikit-learn
- Hugging Face Transformers

---

##  Estrategia de búsqueda

###  FAISS (Semantic Search)
Permite recuperar documentos basados en similitud semántica mediante embeddings.

###  BM25 (Keyword Search)
Recupera documentos basados en coincidencia de términos relevantes.

###  Hybrid Search (RRF)
Combina ambos rankings para mejorar recall y precisión.

###  Cross-Encoder Re-ranking
Modelo neuronal que evalúa directamente la relevancia entre query y chunk.

---

## Objetivo del proyecto

El objetivo es demostrar la implementación de un sistema moderno de recuperación de información combinando:

- Búsqueda semántica (embeddings)
- Búsqueda léxica (BM25)
- Fusión híbrida de rankings
- Re-ranking con modelos de lenguaje

Este enfoque es utilizado en sistemas reales de búsqueda, asistentes legales y motores de QA.

---

## Resultados

El sistema mejora significativamente la calidad de los resultados al combinar:

- Alta cobertura (FAISS + BM25)
- Alta precisión (Cross-Encoder)
- Robustez ante consultas ambiguas

---

## Link Google Colab

https://colab.research.google.com/drive/1IqjHlvJbd6d0e7Yd3aEMDwiI5khsfJSG?usp=sharing
