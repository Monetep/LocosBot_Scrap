                                                            Proyecto LocosBot

-Objetivos del proyecto:
    1. Generar una nota con nivel de redacción humano.         
    2. Generar la nota en base a las notas mas repetidas en otras fuentes.
    3. Publicar la nota en Locosxlosjuegos.com.
    
Se marcará en el documento con el estado ACTUAL para indicar en que etapa se encuentra el desarrollo.    
    
-Pasos a seguir:    
    1. Scrapear las páginas en inglés más importantes.
        a. Seleccionar cuales son las páginas más importantes que voy a querer utilizar. 
            COMPLETO
        b. Aprender a usar BeautifulSoup 4 para hacer el parseo de las páginas web. 
            COMPLETO
        c. Medir necesidad de usar Scrapy para hacer el scrapeo de las páginas web seleccionadas en punto 1.a, y ver si es necesario su aprendizaje. 
            POR AHORA PARECIERA QUE NO NECESITO LA ESCALABILIDAD QUE ME OTORGA SCRAPY, PREFIERO USAR ALGO MAS SENCILLO COMO BS4, PERO HAY QUE EVALUARLO MAS ADELANTE A LA HORA DE ENTRENAR CON UN CORPUS DE TEXTO CONSIDERABLE. PENDIENTE.
        d. Revisar de cada página seleccionada en 1.a usando lo aprendido en 1.b que información es la que quiero capturar (noticias, reviews, etc.). ACTUAL
        e. Usando lo aprendido en los puntos anteriores, hacer un script para cada página para capturar la información que en el punto 1.d definí como objetivo.
        f. Evaluar viabilidad para unificar esos scripts en un solo proceso.
        g. Almacenar lo obtenido en una base de datos, detallado en punto 2.


    2. Almacenar lo obtenido en el punto 1 en una Base de Datos.
        a. Evaluar viabilidad de utilizar mongoDB como base de datos para almacenar lo obtenido de cada página en el punto 1.
            a*. En caso de no haber viabilidad de mongoDB revisar que otras bases de datos SQL o NoSQL se podrían utilizar de forma gratuita.
            b*. Evaluar viabilidad de cada base.
            c*. Seleccionar una para utilizar.
        b. Instalar la base de datos seleccionada en el punto 2.a haciendo uso del tutorial que esté provisto por la herramienta a utilizar.
        c. Aprender a usar la herramienta seleccionada en 2.a e instalada en 2.b.
        d. Diseñar un modelo de datos que responda a la necesidad.
        e. Crear el modelo de datos diseñado en el punto 2.d usando la base de datos seleccionada en el punto 2.a.
        f. Almacenar lo obtenido en el punto 1, en la base de datos para que sea explotado con facilidad.
        
        
    3. Analizar la información usando técnicas de text mining.
        a. Buscar distintas técnicas que desconozca para hacer uso de text mining para analizar y limpiar la información.
        b. Aprender las técnicas que sean aprendidas y necesarias en 3.a en la información almacenada en 2.
        c. Aplicar las técnicas de limpiado de palabras (bag of words, eliminacion de stopwords, seleccionar las palabras mas repetidas, entre otras técnicas).
        d. Almacenar toda la información limpia nuevamente en la base del punto 2.
        
        
    4. Servidor para correr los algoritmos mas pesados:
        a. Muchos de los algoritmos que se planean utilizar en este documento requieren un alto nivel de procesamiento, por lo que hay que buscar un servidor para que haga las tareas mas pesadas.
        b. Analizar viabilidad de utilzar la cuenta de Google Cloud, u otra herramienta en la nube.
        c. Analizar viabilidad de utilizar Colab.
        d. Aprender a usar la herramienta seleccionada en 4.b o aprender a hacer puntos de control usando la herramienta seleccionada en 4.c.    
        e. Armar arquitecturas de prueba que sirvan para lo que se va a desarrollar en los puntos siguientes.
        
        
    5. Embedding.
        a. Buscar ejemplos y el concepto para entenderlo bien de embedding.
        b. Buscar que cantidad de información es necesaria para poder hacer un buen embedding, verificar embeddings preexistentes ya entrenados.
        c. Seguramente se necesite una gran cantidad de informacion, por lo que usando las herramientas desarrolladas en 1 y almacenadas en 2, obtener de las fuentes seleccionadas en 1 una gran cantidad (la necesaria) para poder entrenar un embedding.
        d. Haciendo uso de las herramientas aprendidas en 3, y lo aprendido en 5.a y 5.b, y lo aprendido en el curso de IA, limpiar la informacion obtenida en 5.c para poder tener lista la informacion para entrenar un embedding de videojuegos (word2vec seguramente se esté utilizando).
        e. Analizar viabilidad para entrenar ese embedding desde la pc local, en caso contrario usar la arquitectura seleccionada en 4.
        f. Una vez entrenado el embedding analizar utilidad del mismo, y si quedó del a forma que sea útil para lo que vamos a utilizar.
        
        
    6. Generacion de la red neuronal para el armado de la nota:
        a. En este punto utilizando el embedding entrenado en el punto 5 y haciendo uso de las herramientas aprendidas en el curso de IA y buscando informacion sobre el problema, analizar cual es la mejor forma de encarar el problema usando redes neuronales.
        b. Estos puntos van a ser mas de investigacion que de desarrollo en un principio ya que nunca se hizo algo similar.
        c. Se puede hacer uso del ejemplo que se vio de Artear para desarrollar la solucion, dividir en titulo, bajada y parrafos la nota que se quiera realizar, usando como ejemplo el corpus de notas similares.
        d. Aprender a usar redes neuronales para la generacion de texto, cosa que no usé hasta ahora.
        
        
       
        
    
   
