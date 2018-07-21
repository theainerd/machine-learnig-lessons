# machine-learnig-lessons
Technical Strategy for Machine Learning &amp; Deep Learning Engineers

001. **Don’t be afraid to launch a product without machine learning.**</br>
If machine learning is not absolutely required for your product, don't use it until you have data.

002. **First, design and implement metrics.**</br>
Notice a problem? Add a metric to track it! Excited about some quantitative change on the last release? Add a metric to track it!

003. **Choose machine learning over a complex heuristic.**</br>
in most software engineering tasks, you will want to be constantly updating your approach, whether it is a heuristic or a machine­learned model, and you will find that the machine­-learned model is easier to update and maintain.

004. **Give feature columns owners and documentation.**</br>
If the system is large, and there are many feature columns, know who created or is maintaining each feature column. If you find that the person who understands a feature column is leaving, make sure that someone has the information. Although many feature columns have descriptive names, it's good to have a more detailed description of what the feature is, where it came from, and how it is expected to help.

005. **Choose a simple, observable and attributable metric for your first objective.**<br>
The ML objective should be something that is easy to measure and is a proxy for the "true" objective

Note : Use proxies: if the user is happy, they will stay on the site longer. If the user is satisfied, they will visit again tomorrow. Insofar as well-being and company health is concerned, human judgement is required to connect any machine learned objective to the nature of the product you are selling and your business plan.

006.  **Starting with an interpretable model makes debugging easier.**</br>
Linear regression, logistic regression, and Poisson regression are directly motivated by a probabilistic model. Each prediction is interpretable as a probability or an expected value. This makes them easier to debug than models that use objectives (zero­-one loss, various hinge losses, and so on) that try to directly optimize classification accuracy or ranking performance.

007. **Plan to launch and iterate.**</br>
Don’t expect that the model you are working on now will be the last one that you will launch, or even that you will ever stop launching models. Thus consider whether the complexity you are adding with this launch will slow down future launches. 

008. **Start with directly observed and reported features as opposed to learned features.**</br>
This might be a controversial point, but it avoids a lot of pitfalls. First of all, let’s describe what a learned feature is. A learned feature is a feature generated either by an external system (such as an unsupervised clustering system) or by the learner itself (e.g. via a factored model or deep learning). Both of these can be useful, but they can have a lot of issues, so they should not be in the first model.

009. **Combine and modify existing features to create new features in human­-understandable ways.**</br>
There are a variety of ways to combine and modify features. Machine learning systems such as TensorFlow allow you to pre-process your data through transformations. The two most standard approaches are "discretizations" and "crosses".

010. **The number of feature weights you can learn in a linear model is roughly proportional to the amount of data you have.**</br>
There are fascinating statistical learning theory results concerning the appropriate level of complexity for a model, but this rule is basically all you need to know. I have had conversations in which people were doubtful that anything can be learned from one thousand examples, or that you would ever need more than one million examples, because they get stuck in a certain method of learning.
