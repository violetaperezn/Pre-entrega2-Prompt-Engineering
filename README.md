# Pre-entrega2-Prompt-Engineering
Markdown
# INMERSIA AI: Asistente de Museología Inteligente 🏛️

## Introducción
* **Nombre del proyecto:** INMERSIA AI - Fast Prompting POC.
* **Presentación del problema:** Los visitantes de museos y espacios culturales en Buenos Aires suelen sentirse abrumados por la cantidad de información en las exhibiciones. Las plataformas actuales de ticketing se limitan a la venta, pero no ofrecen una experiencia inmersiva ni contextualización interactiva durante el recorrido.
* **Propuesta de solución:** Implementar un motor de Inteligencia Artificial mediante técnicas de *Fast Prompting* que actúe como un guía cultural personalizado. El modelo tomará inputs sencillos del usuario (tiempo disponible, intereses específicos) y generará un recorrido estructurado y dinámico, mejorando la interacción del usuario con la exhibición.
* **Justificación de la viabilidad:** El proyecto es altamente viable. Al utilizar la API de OpenAI (gpt-4o-mini) estructurando llamadas mediante prompts optimizados, el costo por consulta es mínimo (fracciones de centavo). El tiempo de latencia es bajo, lo que permite una respuesta en tiempo real, y los recursos técnicos requeridos se limitan a Python y el acceso a la API.

## Objetivos
* **Objetivo General:** Demostrar la eficacia de las técnicas de Fast Prompting para transformar inputs no estructurados de usuarios en recomendaciones de recorridos culturales precisos y formateados en JSON.
* **Objetivos Específicos:**
  1. Reducir el número de llamadas a la API a una sola por flujo de usuario utilizando instrucciones unificadas.
  2. Implementar *Role Prompting* y *Output Formatting* para asegurar que la IA responda siempre en el tono adecuado y bajo una estructura de datos predecible.

## Metodología
El proyecto se desarrollará a través de una iteración de pruebas (POC) en una Jupyter Notebook:
1. **Definición del System Prompt:** Diseño del comportamiento base del asistente.
2. **Experimentación de Prompts (Zero-shot vs. Few-shot):** Comparación de salidas para validar la mejora en la calidad y estructura de la respuesta.
3. **Implementación de Código:** Desarrollo de la función en Python para interactuar con la API optimizando el consumo de tokens.
4. **Validación:** Pruebas interactivas simulando diferentes perfiles de visitantes.

## Herramientas y Tecnologías
* **Python y Jupyter Notebooks:** Para la creación y ejecución de la POC.
* **OpenAI API (gpt-4o-mini):** Modelo seleccionado por su excelente relación costo-eficiencia y velocidad.
* **Técnicas de Prompting utilizadas:**
  * *Role Prompting:* Para que asuma el rol de experto en arte e historia argentina.
  * *JSON Mode / Output Formatting:* Para garantizar que la respuesta pueda integrarse fácilmente en el backend de la app.
  * *Delimitadores:* Para separar claramente las instrucciones del texto del usuario y evitar inyecciones.
