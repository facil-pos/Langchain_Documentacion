# Lanchaing

`Nota: Se trabajara con openIA y python`

La siguiente documentacion pretende ensañar langchain desde 0 ofreciendo una documentacion clara y precisa para el equipo de moresale.


## Recursos

[Introduction | 🦜️🔗 Langchain](https://python.langchain.com/docs/get_started/introduction)

[Chat LangChain  🦜️🔗 ](https://chat.langchain.com/)

[YouTube videos | 🦜️🔗 Langchain](https://python.langchain.com/docs/additional_resources/youtube)

### Conocimientos Pre-quesitos

1. [Colab](https://colab.research.google.com/)  
2. Python
3. LLM

## Uso de Lanchaing

## Introduccion a Lanchaing

Langchain es un framework que nos premite desarrollar aplicacion usando LLM como GPT-4, Llama, entre otros, permite que nuestras aplicaciones:

*  Recibir contexto: Esto nos permite conectar un LLM con fuentes de datos externas.
* Razonamiento: Pormedio del contexto sumistrado el modelo razonara sobre este.

### Lanchaing ofrece

* LangChain Libraries : Las bibliotecas Python y JavaScript.
* LangChain Templates: Una colección de arquitecturas de referencia fácilmente desplegables para una amplia variedad de tareas.
* LangServe: Libreria para despliegue de api REST
* LangSmith: Una plataforma para desarrolladores que permite depurar, probar, evaluar y supervisar.

![Arquitectura](https://python.langchain.com/assets/images/langchain_stack-7568bff0848b6ff94a66aff96d074da5.svg)

### [Componentes](https://python.langchain.com/docs/integrations/components)

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



# Curso

A continuacion encontraras cursos practicos para el que aprendar langchain desde 0

1. [Primerso pasos](./Primeros%20Pasos/)


## EMBADDING

### ¿Qué son y para que sirven los embeddings de texto?
- Representaciones numéricas de los textos y tambien existen embeddings de imagen en un vector de numeros.
- Sirven para medir la relación y similitud entre dos piezas de texto que al pasarla a numeros se pueden medir estas distancias y mientras mas se acercan a eseta distancia los textos tienen similitud entre ellos.
- Distancia entre dos embeddings (Conceptos similares).
  - Clasifiación y/o agrupamiento de texto un ememplo el analisis de sentimientos donde se agrupan palabras o faces en sentimientos similares.
  - Repuestas a preguntas ej: si tenemos un pdf de una empresa y queremos hacer preguntas sobre la empresa sin leerlo completo, los embeddings nos va a permitir navegar en el pdf de forma eficiente y rapida para obtener la respuesta que necesitemos cuando encuentre estas distancias similares entre los vectores.

