# Firearm Shot Detection System

## Contexto y Objetivo (Context and Objective)

La biodiversidad se está perdiendo a nivel mundial a un ritmo sin precedentes, debido a los acelerados impactos humanos. La sobreexplotación de especies se encuentra entre los principales impulsores de la pérdida de biodiversidad global y amenaza a más de una cuarta parte de todas las especies de animales terrestres. Esta amenaza se expresa con especial fuerza en las regiones tropicales y ocurre con frecuencia dentro de áreas protegidas, donde amenazas como la pérdida de hábitat comúnmente coexisten con la caza excesiva y/o furtiva para exacerbar el problema.

En la actualidad, una de las herramientas principales para el monitoreo de diferentes hábitats resulta en la instalación de grabadores de audio, que graban (valga la redundancia) la presencia de todo lo que emita sonido. Una desventaja, es que se producen volúmenes de datos grandes, y la mayoría de las veces resulta inviable extraer información de manera manual (humano especializado escuchando años de grabaciones). Esto constituye un excelente campo de aplicación para las herramientas que abarcan la inteligencia computacional.

El objetivo del trabajo consta de determinar en audios provenientes de grabadores reales la existencia de disparos de armas de fuego. Si se hallan evidencias de los mismos, es importante conocer en qué estampa de tiempo y en qué audios están. Con esta información, podría solicitarse a un experto la validación de los hallazgos. Además, lo ideal es que el modelo resulte lo más pequeño y eficiente posible.

Biodiversity is being lost globally at an unprecedented rate due to accelerated human impacts. The overexploitation of species stands among the primary drivers of global biodiversity loss and threatens over a quarter of all terrestrial animal species. This threat is particularly pronounced in tropical regions and often occurs within protected areas, where challenges such as habitat loss commonly coexist with overhunting and/or poaching, exacerbating the problem.

Currently, one of the primary tools for monitoring various habitats involves the installation of audio recorders that capture (pardon the redundancy) the presence of any sound-emitting source. One disadvantage is the generation of large volumes of data, and most of the time, extracting information manually (a specialized human listening to years of recordings) becomes impractical. This scenario presents an excellent application area for tools incorporating computational intelligence.

The objective of the work is to determine the presence of firearm shots in audio recordings from real-life recorders. If evidence of such shots is found, it is important to identify the timestamp and the corresponding audio files. This information could be used to request validation from an expert. Additionally, the ideal outcome is for the model to be as small and efficient as possible.

## Datos disponibles (Data Available)

Se cuenta con un dataset de base, conformado por recortes de aproximadamente 4 segundos de duración, los cuales contienen eventos con disparos (a diferentes distancias, distintos tipos de armas, etc.). Estos eventos se corresponden a ocurrencias en entornos selváticos. Además, se disponen de recortes con características similares, pero sin eventos de disparo. Varios de
estos recortes, presentan eventos que un mal modelo podría considerar un disparo, pero no lo son (rupturas de ramas, golpes, etc.). Estos archivos pueden utilizarse como base para identificar el preprocesamiento adecuado, diseñar una estrategia para la detección, plantear y validar hipótesis, entrenar modelos, entre otros.

Por otra parte, se dispone de aproximadamente 28 horas de grabación, en archivos de audio de 10 minutos, para validar y poner a prueba el modelo. Pudiendo estimar costos de cómputo y otras métricas que se crean convenientes. Determinar si existen disparos en este lote de audios sin procesar, si es así, cuántos y dónde se localizan.

A base dataset is available, consisting of approximately 4-second clips containing gunshot events (at different distances, with various types of firearms, etc.). These events correspond to occurrences in jungle environments. Additionally, clips with similar characteristics are provided but without gunshot events. Some of these clips feature events that a flawed model might mistakenly consider a gunshot, but they are not (branch breaks, impacts, etc.). These files can be used as a foundation for identifying proper preprocessing, devising a detection strategy, formulating and validating hypotheses, training models, among other tasks.

On the other hand, there is approximately 28 hours of recording, in 10-minute audio files, available to validate and test the model. This allows for estimating computational costs and other relevant metrics. The goal is to determine if there are gunshots in this batch of raw audio, and if so, how many and where they are located.