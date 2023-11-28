# Primeros pasos

Aqui conoceras sobre los principos de fundamentales de langchain y te familiarizarás con los Modelos de OpenAi

# Temario

1. Entender los principios fundamentales de LangChain y cómo se utiliza para desarrollar aplicaciones basadas en modelos de lenguaje.
2. Aprender a instalar LangChain y configurar el entorno de desarrollo necesario.
3. Conocer los requisitos de hardware y software para ejecutar LangChain de manera eficiente.
4. Familiarizarse con los módulos y componentes principales de LangChain, como modelos, cadenas, agentes y memoria.

# Introduccion a Lanchaing

Langchain es un framework que nos premite desarrollar aplicacion usando LLM como GPT-4, Llama, entre otros, permite que nuestras aplicaciones:

* Contexto consciente: LangChain permite que las aplicaciones basadas en modelos de lenguaje estén conscientes del contexto. Esto implica conectar un modelo de lenguaje con fuentes de contexto, como instrucciones de entrada, ejemplos de pocos disparos y contenido relevante, para mejorar la calidad y relevancia de las respuestas generadas.

* Razonamiento: LangChain permite que las aplicaciones basadas en modelos de lenguaje razonen y tomen decisiones basadas en el contexto proporcionado. Esto implica utilizar el modelo de lenguaje para tomar decisiones sobre cómo responder en función del contexto y las directivas de alto nivel.

## Usos de Lanchaing

LangChain tiene una amplia gama de casos de uso en el desarrollo de aplicaciones basadas en modelos de lenguaje. Algunos de los casos de uso comunes de LangChain incluyen:

* Chatbots: LangChain se puede utilizar para desarrollar chatbots conversacionales que pueden interactuar con los usuarios, responder preguntas, brindar recomendaciones y realizar tareas específicas.

* Asistentes personales: LangChain permite crear asistentes personales virtuales que pueden ayudar a los usuarios en diversas tareas, como recordatorios, planificación de eventos, búsqueda de información y más.

* Preguntas y respuestas: LangChain se puede utilizar para desarrollar sistemas de preguntas y respuestas que pueden responder consultas basadas en documentos específicos o conocimiento almacenado.

* Generación de texto: LangChain es útil para generar texto en diversos contextos, como la generación de contenido para sitios web, redacción automática de informes, resúmenes de texto y más.

* Traducción automática: LangChain se puede utilizar para desarrollar sistemas de traducción automática que pueden traducir texto de un idioma a otro de manera eficiente.

* Análisis de sentimientos: LangChain puede ayudar en el análisis de sentimientos al procesar texto y determinar la polaridad emocional asociada con él.

* Extracción de información: LangChain puede utilizarse para extraer información estructurada de texto no estructurado, como nombres de entidades, fechas, ubicaciones, etc.

## Infraestructura de langchain

* LangChain Libraries : Las bibliotecas Python y JavaScript.
* LangChain Templates: Una colección de arquitecturas de referencia fácilmente desplegables para una amplia variedad de tareas.
* LangServe: Libreria para despliegue de api REST
* LangSmith: Una plataforma para desarrolladores que permite depurar, probar, evaluar y supervisar.

![Arquitectura](https://python.langchain.com/assets/images/langchain_stack-7568bff0848b6ff94a66aff96d074da5.svg)

## [Infraestructura](https://python.langchain.com/docs/integrations/components)

En LangChain, los componentes son abstracciones que permiten trabajar con modelos de lenguaje y se utilizan como bloques de construcción modulares en el desarrollo de aplicaciones. Estos componentes son fáciles de usar y se pueden personalizar según las necesidades específicas de cada aplicación. Algunos ejemplos de componentes en LangChain son:

- Model I/O (Entrada/Salida de Modelo): Proporciona interfaces para interactuar con modelos de lenguaje, como cargar y guardar modelos, realizar inferencias y ajustar hiperparámetros.
- Data connection (Conexion de Datos): Permite conectar la inferfaz con los dato sespecificos de la aplicación. Facilita la conexion entre LangChain y las fuentes de datos externas, permitiendo qeu los datos se pasen entre ambos.
- Chains (cadenas): Son secuencias estructuradas de llamadas que se pueden construir utilizando componentes de LangChain. Estas cadenas definen el flujo de trabajo de la aplicación y cómo se utilizan los modelos de lenguaje y otros componentes.
- Agents (Agentes): Este componente permite que las cadenas elijan qué herramientas usar dadas directivas de alto nivel. FAcilita la toma de decisines sobre qeu acciones tomar o que herramientas usar en fuancion de las necesidades de la aplicacion.
- Memory (memoria): Permite persistir el estado de la aplicacion entre ejecuciones de una cadena. Facilita la gestion de la memoria, permitiendo que los datos se almacenen y reucperen entre diferentes ejecuciones de una cadena. Facilita la gestion de la memoria, permitiendo que los datos se almacenen y recuperen entre diferentes ejecuciones de la aplicacion.
- Callbacks (Retrollamadas): Permite registrar y transcribir los pasos intermedios de cualquier cadena. Facilita la monitorizacion y el registro de las actividades de la aplicacion, permitiendo que se puedan realizar seguimientos y analisis detallados de las operaciones de la aplicacion.

## Instalacion

Langchain nospermite tener varias forma de instalarlo

### Instalacion minima
* pip

  ```bash
  pip install langchain
  ```
* conda

  ```bash
  conda install langchain -c conda-forge
  ```

### Instalacion LangServe

```bash
pip install "langserve[all]"
```

### LangChain CLI

```bash
pip install langchain-cli
```

### LangSmith

```
pip install langsmith
```

# Familiarizacion con los modelos de OpenIA

Como conseguir los modelos de OpenIA

1. Nos vamos a la pagina de (https://openai.com/pricing)
2. Developers
3. Documentacion
4. Models que esta a la izquierda
5. Tocamos donde dice GPT-3.5
6. LATEST MODEL mostrará todos los modelos como el de 'text-davinci-003'

Ejercicio practico para conocer los fundamento de Langchain con OpenIA

* [Fundamentos.ipynb](./Fundamentos.ipynb)