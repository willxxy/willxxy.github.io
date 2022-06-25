## Intro to Machine Learning

Ever since I joined the [AI Club at UCI](https://aiclub.ics.uci.edu/){:target="_blank"} back in September 2021, I have been 
furiously studying machine learning. Machine learning is something that is quite magical, and the last 50 to 70 years of research in statistics, neural
networks, and more broadly, artificial intelligence, has definitely paved a 'work in progress' structure for people like myself to build upon.

So with that, I want to start this attempt to introduce machine learning with a definition coined by [Dr. Peter Chang](https://www.faculty.uci.edu/profile.cfm?faculty_id=6569){:target="_blank"}, 
a radiologist by training and Co-Director of the [Center for Artificial Intelligence in Diagnostic Medicine](https://www.caidm.som.uci.edu/){:target="_blank"}. He defines machine learning
algorithms as something that maps inputs to desired outputs through a model whose parameters may be trained through iterative exposure to data (1). 


<img src="/png/machine_learning.png" style="height: 100; width:300px; display: block; margin: 0 auto"/>


Let's break this down. First, what is an algorithm? The Oxford dictionary defines it as 'a process or set of rules to be followed in calculations or other problem-solving operations, especially by a computer.' So, in our case, the process or set of rules to be followed is to map inputs to desired outputs. The calculations or problem-solving operations would be performed in the model, and the parameters would be the variables that need to be computed while interacting with the inputs and outputs. These parameters than need to be exposed to an arbitrary set of data in a repetitive manner for it to 'train.' To further explain what the word 'trained' means in the definition, I believe a real-world example would be best.


Let's say you want to have muscles like the person shown below. 


<img src="/png/aesthetic.jpeg" style="height: 100; width:300px; display: block; margin: 0 auto"/>


The input would be one's body and the output would be muscles. The process or set of rules to be followed can be a strict diet or workout routine. Introducing your body to a strict diet and workout routine can be the mapping between the input and output. The model can be represented as the chosen diet or workout and the parameters would be the specific ingredients to the diet or workout, such as vegetables, meat, calisthenics, hard weights, etc. The training begins when you repeatedly engage your input (body) to the model (workout/diet), while continuously updating the parameters (best diet, best workout). In this example, the data would be somewhat synonymous with the parameters, but it can be set apart as the knowledge and experimentation of which diet or workout produces the desired output. If protein and pull ups seems to be producing the most muscle, one would want to constantly use and feed this data or knowledge into the model. If your model is trained successfully over a period of time, theoretically, you would have outputted some muscles. However, life and machine learning algorithms do not work this way and there are many confounding variables that you find along the process of training a successful model. For the sake of simplicity, I will not go into such adversarial components.


Hopefully, you now have a somewhat intuitive idea of what a machine learning algorithm is, and now I will propose three different categories of such algorithms. I would agree with Dr. Chang in that there are three different kinds of machine learning algorithms (1): 1) Traditional Statistics; 2) Traditional Machine Learning; 3) Neural Networks. 

An example of a traditional statistical machine learning algorithm can be something like `y = mx + b`. 
As we all learned in middle school, `x`, `y` denotes the input and output, and `m`, `b` represents the variable parameters (slope and intercept).
Traditional statistics is extremely good at finding linear relationships between variables but when data becomes more obscure and abstract, traditional machine learning algorithms tend to outperform in determining correlations. 

To battle complex inputs and non-linearity, traditional machine learning algorithms try to refine complex data (e.g. image) into numbers represented as a vector.
This distillation is called feature extraction and machine learning algorithms can capture rich traits of the data, such as spatial context, multi-resolution, locality, and globality. 


<img src="/png/mnist.png" style="height: 100; width:300px; display: block; margin: 0 auto"/>


It is important to note that these features do not need to be complex. However, in practice, data is multidimensional, therefore 
a huge amount of research has gone into transforming N-dimensional feature vector projections to something computers can understand. 
Given these feature vectors, the most common function machine learning algorithms face is classification, which can be described as making predictions with existing data. 
I will not go over any specific traditional machine learning algorithms, but here is a list of them for you to explore: 
- [Support Vector Machine](https://en.wikipedia.org/wiki/Support-vector_machine){:target="_blank"}
- [k-Nearest Neighbor](https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm){:target="_blank"}
- [XGBoost](https://xgboost.readthedocs.io/en/stable/){:target="_blank"}
- [Random Forest](https://en.wikipedia.org/wiki/Random_forest#:~:text=Random%20forests%20or%20random%20decision,class%20selected%20by%20most%20trees.){:target="_blank"}

Now, what if there are no apparent features or parameters within a dataset? This is where neural networks shine. 


<img src="/png/network.png" style="height: 200; width:400px; display: block; margin: 0 auto"/>


Neural networks were inspired by the activity of biological neurons in the human brain. Each circle in the image above is represented as a node, and there are 
three main layers that comprises a neural network: the input layer, hidden layer, and output layer. Each node is linked to another and has an assigned weight and 
threshold. If the output of any individual node is above a specified threshold value, the node is activated and sends the data to the next layer of the network (2). Otherwise,
no data is passed. A neural network with n > 1 hidden layers is categorized as a deep neural network. Voice recognition, autonomous vehicles, facial recognition are some of the many tasks
deep neural networks have made possible. 

Although neural networks have been able to do amazing things, an important con to note is that it requires huge amounts of data. Luckily, there are many areas of research in 
the machine learning community dedicated in solving complex problems with neural networks given very limited data. 

I hope you enjoyed my very brief introduction to machine learning. If you are curious to learn more about this fascinating topic, I will provide a list of resources
I used for myself. 
- [Machine Learning Course by Andrew Ng](https://www.coursera.org/learn/machine-learning){:target="_blank"}
- [Machine Learning Course by freeCodeCamp](https://www.youtube.com/watch?v=NWONeJKn6kc&t=50s){:target="_blank"}
- [Machine Learning Course by Geoffrey Hinton](https://youtube.com/playlist?list=PLoRl3Ht4JOcdU872GhiYWf6jwrk_SNhz9){:target="_blank"}
- [MNIST classifier with NumPy from scratch by George Hotz](https://www.youtube.com/watch?v=JRlyw6LO5qo&t=8s){:target="_blank"}
- [Introduction to Neural Networks by Victor Zhou](https://victorzhou.com/blog/intro-to-neural-networks/){:target="_blank"}


References

(1) [Machine Learning Definition](https://uci.yuja.com/V/MediaFile?mediaFile=420457&node=15536234&a=1231719205&autoplay=1){:target="_blank"}

(2) [Neural Networks](https://www.ibm.com/cloud/learn/neural-networks){:target="_blank"}
