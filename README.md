# Few-shot Learning with Reptile


<div align="center">
    <a href="https://colab.research.google.com/github/reshalfahsi/few-shot-learning-reptile/blob/master/Few_shot_Learning_with_Reptile.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="colab"></a>
    <br />
</div>


Just by seeing an object several times, humans can identify it easily. This concept can be applied to artificial neural networks (ANNs) as well (i.e., few-shot learning). Meta-learning appears as a way to achieve this goal: an artificial neural network (ANN) must learn one of the learning components (e.g., optimizers, models, etc.) to behave with virtually the same level of adaptability as humans. The reptile algorithm, one of the meta-learning techniques, makes sure the target model's initial weights are appropriate for identifying provided inputs (like images) in minuscule quantities. The method follows the steps below for each epoch. Select a task (n selected classes with k data points each) at random from the dataset (for example, the Omniglot dataset). Use SGD or Adam to optimize the target model several times on the task. Shift the target model's old weights to the direction of the new weights from the previous step.


## Experiment

This [notebook](https://github.com/reshalfahsi/few-shot-learning-reptile/blob/master/Few_shot_Learning_with_Reptile.ipynb) provides everything needed regarding the experiment of this project.


## Result

## Quantitative Result

Below is the quantitative result of the algorithm.

Test Metric | Score |
----------- | ----- |
Accuracy | 90.35%
Loss | 0.403


## Accuracy and Loss Curves

<p align="center"> <img src="https://github.com/reshalfahsi/few-shot-learning-reptile/blob/master/assets/loss_curve.png" alt="loss_curve" > <br /> The loss curve on the train and validation sets of the model. </p>

<p align="center"> <img src="https://github.com/reshalfahsi/few-shot-learning-reptile/blob/master/assets/acc_curve.png" alt="acc_curve" > <br /> The accuracy curve on the train and validation sets of the model. </p>


## Qualitative Result

These sets of images visually divulge the qualitative performance of the Reptile algorithm.

<p align="center"> <img src="https://github.com/reshalfahsi/few-shot-learning-reptile/blob/master/assets/qualitative.png" alt="qualitative" > <br /> The top five rows contain support images. Each row indicates a separate class (or way). Each class has been provided with five shots (or samples) of images. The query images and their respective predicted classes are shown in the very bottom row. </p>



## Credit

- [Omniglot](https://github.com/brendenlake/omniglot)
- [Human-level concept learning through probabilistic program induction](https://www.cs.cmu.edu/~rsalakhu/papers/LakeEtAl2015Science.pdf)
- [The Omniglot challenge: a 3-year progress report](https://arxiv.org/pdf/1902.03477)
- [Reptile: A scalable meta-learning algorithm](https://openai.com/index/reptile/)
- [On First-Order Meta-Learning Algorithms](https://arxiv.org/pdf/1803.02999)
- [Few-Shot learning with Reptile](https://keras.io/examples/vision/reptile/)
- [Tutorial 16: Meta-Learning - Learning to Learn](https://uvadlc-notebooks.readthedocs.io/en/latest/tutorial_notebooks/tutorial16/Meta_Learning.html)
- [PyTorch Lightning](https://lightning.ai/docs/pytorch/latest/)
