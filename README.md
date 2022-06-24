# Cobar 2021 miniproject - BIO-ENG456: Controlling animal behavior in animal and robots - EPFL

Team Super-duper

The finalised code can be found in the "Clean" Jupyter Notebook.

30 May 2021

# Abstract
This project aims at exploring neural activity and neurons correlations with behaviour in Drosophila flies. Data collected in the UPRAMDYA laboratory at EPFL provided neural activity, joint angles and
joint 3D poses of the Drosophila fly for 12 trials. This data was analyzed to better understand how neural signals control limb movement. Groups of neurons with similar signals were found, suggesting
that the motor control in Drosophila uses multiple neurons in parallel possibly for better robustness. Correlations between neurons and joint angles were stronger than those with behavior, suggesting
that the neurons recorded are Descending Neurons. Behavior classification from neuronal activity was found to be possible. In particular, with the implementation of a more advanced neural network
classifier remarkably good performance metrics were achieved for the prediction of multiple behaviors. A logistic regression method may be enough, depending on the level of accuracy needed, for a
reasonable enough quality prediction in the case of a binary classification. These results constitute an important step towards a more comprehensive understanding of the function of different neurons.

# Discussion
Through the data analysis done in this project, groups of neurons were found to have similar activities. Having multiple signals conveying similar information could be crucial for an organism, increasing robustness to noise. If an action was controlled by only one neuron, even a small signal perturbation could result in an unwanted action. Controlling an action with multiple neurons ensures that perturbation in one neuron's signal will not affect the final action done. The clustering of the neurons depends on the clustering method used and its hyper-parameters. More analysis could be done to improve the clustering by optimizing each method's parameters and more rigorously comparing the two methods.

Looking at correlation between individual neurons and binary behavior signals, we could identify different sets of neurons more likely to conserve information encoding for a particular behavior (either positively or negatively). This exploratory data analysis part was then used to improve the regression, providing a sorted neurons list with deceasing importance related to each behaviors. Indeed, sometimes regression is sensitive to the number of features provided as input; reducing the input data set allows to focus more on the provided information. Correlation was hence helpful to target desired behavior with the neurons that were considered important for each behavior.

Concerning the behavior classification from neuronal activity different methods were explored, highlighting their advantages and disadvantages. Particularly when predicting with a more advanced classifier as a neural network, it is possible to reliably classify multiple behaviors from the neural activities. In the multi-class task, implementing the logistic regression generated relatively poor results with about 70-100 neurons per class contributing to the classification. On the other hand, when dealing with a single behavior prediction, a simple logistic classifier may reach acceptable performance relying on about 40-50 neurons.

# Collaborators
Team Super-duper

Lorenzo Germini

Mathias Nuris_Souquet

Hila Vardi


Professor: Pavan Ramdya

