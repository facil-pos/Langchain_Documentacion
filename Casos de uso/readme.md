# Casos de uso

Aprender a cargar y utilizar modelos de lenguaje para tareas como generación de texto, traducción, resumen, entre otros.

# Conceptos necesarios

## Prompt

Un prompt es un conjunto de instrucciones o entrada proporcionada por un usuario para guiar la respuesta de un modelo de lenguaje. 

Ayuda al modelo a comprender el contexto y generar una salida relevante y coherente basada en el lenguaje, como responder preguntas, completar frases o participar en una conversación, los prompts pueden ser plantillas parametrizadas que especifican entradas específicas para el modelo, ejemplos seleccionados dinámicamente o datos etiquetados, los prompts efectivos suelen estar relacionados con el dominio de la tarea y calibrar la probabilidad previa de las palabras clave.

### Prompt Templates o plantillas

Antes de mirar los casos de uso de las langchain debemos entender que es un Prompt templates o plantilla y para que nos sirve.

La mayoría de las aplicaciones LLM no pasan la entrada del usuario directamente a un LLM. Por lo general, añaden a la entrada del usuario a un fragmento de texto más grande, denominado plantilla de instrucciones, que proporciona contexto adicional sobre la tarea específica en cuestión.

Tenemos como caso de uso un traductor automatico, nuestro Prompt seria algo como ``Identicia el idioma del siguiente texto "Texto a traducir" y traducelo al español``, el usuario tendria que esbrir siemple este texto largo para darle contexto e intrucciones al modelo, la plantilla nos permite definir este texto largo como una plantilla, esto le permite al usuario solo dar la tarea màs no la instruccion.

### Material de estudio

* [Prompts.ipynb](.\Prompts.ipynb)

## [Chains o cadenas](https://python.langchain.com/docs/modules/chains/)

Una chain (cadena) en el contexto de Langchain se refiere a la secuencia de llamadas a componentes o modelos de lenguaje que se utilizan para realizar tareas más complejas. Langchain proporciona dos enfoques para crear cadenas: el enfoque heredado utilizando la interfaz Chain y el enfoque actualizado utilizando el LangChain Expression Language (LCEL).

Una chain en Langchain es una secuencia de llamadas a componentes o modelos de lenguaje que se utilizan para realizar tareas más complejas, como responder preguntas, traducir texto o generar texto.

### Material de estudio

* [Chains.ipynb](.\Chains.ipynb)

## Agentes

La idea central de los agentes es utilizar un modelo de lenguaje para elegir una secuencia de acciones a realizar. En las cadenas, la secuencia de acciones está codificada (en código). En los agentes, se utiliza un modelo de lenguaje como motor de razonamiento para determinar qué acciones realizar y en qué orden, estas son algunas de las cosas que nos ofrecen los agentes.

* Los agentes en Python se basan en un modelo de lenguaje y un conjunto de herramientas que les permiten realizar tareas específicas.

* Los agentes pueden tomar decisiones utilizando un modelo de lenguaje para razonar y determinar qué acciones tomar y en qué orden.

* Los agentes pueden utilizar herramientas para realizar acciones específicas, como buscar información, realizar cálculos, interactuar con APIs, entre otros.

* Los agentes en Python se pueden inicializar utilizando diferentes tipos de agentes, como ZERO_SHOT_REACT_DESCRIPTION o OPENAI_FUNCTIONS, dependiendo de los requisitos y la naturaleza de la tarea.

* Los agentes en Python pueden ejecutarse utilizando el AgentExecutor, que es el tiempo de ejecución del agente. El AgentExecutor se encarga de llamar al agente y ejecutar las acciones que el agente selecciona.

* Los agentes en Python también pueden utilizar toolkits, que son grupos de herramientas necesarias para lograr objetivos específicos.

### Recursos 

[Tools | 🦜️🔗 Langchain](https://python.langchain.com/docs/integrations/tools/).

### Material de estudio

[Agentes.ipynb](./Agentes.ipynb)