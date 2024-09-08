## Pento Coding challenge

### Readme
The initial problem involves classifying images of 4 dog breeds. Subsequently, the task is to classify images that do not belong to these breeds into another category called "other."
To solve the initial problem, a Transfer Learning strategy using ResNet152V2 was employed. For the second instance of categorization, one strategy was implemented and another proposed.

### Content

- MLChallenge.ipynb: The notebook containing the solution to the problem
- Pruebas: Repository of borderline image cases
- dogs: Original images
- output: Images divided into train, test, and val sets
- Machine Learning Engineer Challenge.pdf : Rubricas 

### Testing

To evaluate the dog breed classification model, you can use `model.evaluate`, after generating a new testing set with corresponding labels. For the "other" evaluation, I created a function called `classifyimg(path,threshold)`, which takes the image path and a threshold (I set it at 0.97) to separate other dog breeds. This function returns the prediction and the highest output of the original model.
