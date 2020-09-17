# Summery for [ML RoadMap](https://youtu.be/pHiMN_gy9mk)

> I decided to lose the particularities such as software names or algorithm types. They do not mean much to me so far anyway. In any case, this is an overview

ML is a way for computers to be  able to process data and find patterns in it without being **explicitly programmed**.

Can be effectively applied to deal with 
- **problems with a long list of rules**, when it is impossible to take all the aspects into account.
-   **problems in continually changing environments**, where flexibility and quick adaptation are crucial.
-  **discovering insights withing large collections of data**

## Types of ML

 **Supervised Machine Learning (SML)**
All data is labeled. Machine tries to find correlation patterns between data and labels. Problem domains include:
- **Classification.** Assigns labels to data (e.g. labeling email as spam)
- **Regression.** Predicts tendencies for data (e.g. price of real estate).
-  **Sequence to Sequence.** Transforms one kind of data into another (e.g. sound into text).

**Unsupervised Machine Learning (UML)**
Data is not labeled. Machine tries to find patterns in the unlabeled data. Problem domains include:
- **Clustering.** Groups data in clusters according to some similarities. Clusters can then be labeled.
- **Dimensionality reduction.** Points out the meaningful parameters in data and discards the 'noise'.

**Transfer learning**
Using knowledge, learned by a model on other data.

**Reinforcement learning**
Algorithm acts in an environment and gets rewarded or punished based on what actions it performs.

## Stages of ML process

1. **Data collection**
>Data is chosen based on its availability, the problem in question. Privacy concerns should also be taken into account. Data can be **structured** (in tables, e.g. statistics) or **unstructured** (e.g. images, sounds etc.)

2. **Data preparation** 
> Consists of:
>- Exploratory Data Analysis (EDA); 
>- Preprocessing (feature encoding, feature normalization, scaling, feature engineering) 
>- Data splitting

3. **Choosing an algorithm**

4. **Training on data**
>Type of learning depends on the state of data. 
  It can be 
  **batch learning**, 
**online learning**, 
**transfer learning**, 
**human-in-the-loop learning** 
or combinations of the above.

5. **Regularization**
>Dealing with problems such as **underfitting** and **overfitting** *(when model works well on data it was trained on and bad on the new data)*; tuning the **hyperparameters**, setting the **learning rate**.

6. **Analysis and Evaluation**
>To define error rate and home much time (and resources) does learning require. Also analyzing the model with **what-if tools** to understand the principles by which it came to be guided.

7. **Serving the model**
>Putting into product and adjusting it for mass-usage.
8. **Retraining the model**
> Just in case. For example new data arrived.

## Tools for creating ML

**Libraries (mostly for Python)**
>- PyTorch
>- Scikit-Learn
>- Tensor Flow

**Experiment tracking tools**

**Pre-trained models**

**Hyperparameter tuning tools**

**Tools for analyzing and explaining ML models**

**ML LifeCicle tools**
(what are these?)

**User Interface Design tools**

## ML mathematics

- **Linear Algebra**

- **Matrix Manipulation**
Data can be arranged in matrixes.
>The video had it as a separate thing, but it's part of linear algebra, isn't it?
- **Multivariable calculus**
For optimizing functions.

- **Optimization**
For the same thing I guess.

- **Probability and probability distributions**
For many things including data preparation.

- **Chain rule**
For *backpropagation* (?)


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTc1Njg1MDc3Nl19
-->