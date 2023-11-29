# Casos de uso

Aprender a cargar y utilizar modelos de lenguaje para tareas como generación de texto, traducción, resumen, entre otros.

Encada uno de los siguientes conceptos se propocionara de un ejemplo practico donde se plantearan casos de usos para cada uno de los temas.

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

## Memoria o Memory 

Un componente esencial de una conversación es poder referirse a la información introducida anteriormente en la conversación. Como mínimo, un sistema conversacional debería ser capaz de acceder directamente a alguna ventana de mensajes pasados.

A esta capacidad de almacenar información sobre interacciones pasadas la llamamos "memoria". LangChain proporciona muchas utilidades para agregar memoria a un sistema. Estas utilidades se pueden utilizar por sí solas o incorporarse sin problemas a una chain.

### Tipos de memoria

Hay muchos tipos diferentes de memoria. Cada uno tiene sus propios parámetros, sus propios tipos de valor devuelto y es útil en diferentes escenarios.

* [``ConversationBufferMemory``](https://python.langchain.com/docs/modules/memory/types/buffer): Almacena los mensajes de chat en una lista en memoria. Puede devolver los mensajes como una cadena concatenada o como una lista de objetos ``ChatMessage``.

* [``ConversationBufferWindowMemory``](https://python.langchain.com/docs/modules/memory/types/buffer_window): Esto puede resultar útil para mantener una ventana deslizante de las interacciones más recientes, de modo que el búfer no crezca demasiado.

* [``Entity``](https://python.langchain.com/docs/modules/memory/types/entity_summary_memory): La memoria de entidad recuerda hechos dados sobre entidades específicas en una conversación (Una entidad en una conversacion hace referencia a algo o alguien).

* [``Conversation Knowledge Graph``](https://python.langchain.com/docs/modules/memory/types/kg):  Este tipo de memoria utiliza grafos para recrear una memoria.

* [``Conversation Summary``](https://python.langchain.com/docs/modules/memory/types/summary): Este tipo de memoria crea un resumen de la conversación a lo largo del tiempo.

* [``Conversation Summary Buffer``](https://python.langchain.com/docs/modules/memory/types/summary_buffer): Mantiene un buffer de interacciones recientes en la memoria, pero en lugar de simplemente eliminar por completo las interacciones antiguas, las compila en un resumen y usa ambas, utiliza la longitud del token en lugar del número de interacciones para determinar cuándo eliminar las interacciones..

* [``Conversation Token Buffer``](https://python.langchain.com/docs/modules/memory/types/token_buffer) Mantiene un búfer de interacciones recientes en la memoria y utiliza la longitud del token en lugar del número de interacciones para determinar cuándo eliminar las interacciones.

* [Backed by a Vector Store](https://python.langchain.com/docs/modules/memory/types/vectorstore_retriever_memory): VectorStoreRetrieverMemory almacena recuerdos en un almacén de vectores y consulta los documentos más "destacados" cada vez que se llama.

#### Recursos

[Memory | 🦜️🔗 Langchain](https://python.langchain.com/docs/modules/memory/)

### Material de estudio

[Memoria.ipynb](./Memoria.ipynb)