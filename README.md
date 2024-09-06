## Pento Coding challenge

### Readme
El problema inicialmente en clasificar imagenes de 4 razas de perro. Posteriormente se pide clasificar imagenes que no tenemos dentro de otra categoría llama other.
Para resolver el problema inicial se uso una estrategia de TransferLearning con ResNet152V2, para la segunda instancia de categorización se empleo una estrategia y se propuso la idea de otra.

### Contenido

- MLChallenge.ipynb: El cuaderno de trabajo donde esta la solución al problema
- Pruebas: Repositorio de imágenes de casos borde
- dogs: Imagenes originales
- output: Imagenes dividas entre train, test, val
- Machine Learning Engineer Challenge.pdf : Rubricas 

### Testeo 
Para evaluar el modelo de clasificación de razas de perro se puede usar `model.evaluate` generando previamente un nuevo conjunto de testeo con sus correspondientes etiquetas. Para la evaluación con other cree una función llamada `clasificar_imagen(path,threshold)` que toma como argumentos el camino a 
la imagen y un threshold que yo defini sea 0.97 para separar otras razas de perro. Esta última devuelve la predicción y el output de mayor salida del modelo original.
