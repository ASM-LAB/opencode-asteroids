---
description: Presenta una visión general de la aplicación, su arquitectura y su funcionamiento
agent: plan
---

Proporciona una visión general de esta aplicación.

Sigue las indicaciones de `AGENTS.md` y usa el código como fuente de verdad: si la documentación existente contradice al código, describe lo que hace el código.

Alcance opcional: $ARGUMENTS (si está vacío, cubre toda la aplicación).

Proceso:

1. Explora la estructura del proyecto y localiza los archivos principales, la documentación y la configuración.
2. Lee el código y la documentación necesarios para entender qué hace la aplicación y cómo está organizada.
3. Si algo no queda claro, compruébalo en el código antes de afirmarlo; no inventes funcionalidades ni archivos.

La respuesta debe incluir, en este orden:

- **Propósito**: qué es la aplicación y qué problema resuelve.
- **Tecnologías y requisitos**: lenguajes, librerías y dependencias relevantes (o ausencia de ellas).
- **Estructura**: árbol breve de archivos y carpetas con la responsabilidad de cada uno.
- **Arquitectura y flujo principal**: cómo se conectan las piezas y qué ocurre desde que arranca la aplicación hasta la acción principal del usuario.
- **Funcionalidades**: lista de características visibles para el usuario.
- **Cómo ejecutarla**: pasos concretos para ponerla en marcha.
- **Observaciones**: limitaciones, deuda técnica, inconsistencias entre README y código o puntos que conviene revisar.

Responde en español, en Markdown, de forma clara y concisa, sin repetir el contenido de los archivos textualmente. No modifiques archivos: esta tarea es solo de análisis. Si el usuario pide guardar la visión general en un archivo, propón una ruta y créala.
