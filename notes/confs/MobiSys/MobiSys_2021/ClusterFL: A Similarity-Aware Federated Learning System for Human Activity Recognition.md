# Contributions ```C```:
The authors propose aims at learning a better model and simultaenously reduce communication overhead in the Federated Learning paradigm. To that end, the authors
propose (1) Cluster-wise straggler dropout and (2) Correlation-based node selection to intelligently drop stragglers and select more related nodes in each cluster
to be sent through the network.

# Main Idea ```M```:
The main idea is based on some observations on case study. First, they invesitgate the structurability on the dataset. Hopkin statistics is used on on 6 different 
HAR datasets and they found strong clusterability. That is, there exist cluster structures in the data. Another pivot study shows that Centralized-cluster models 
yield higher accuracy and less standard devation. 

# Limitations ```L```:
Given a large amount of data, Centralized learning is better in Fig. 12.
Trained models contain some information of users, there are some potential privacy concern if information can be recovered from the model.

# Takeaways
In FL paradigm, users' models are sent through the network instead of data due to privacy concern.
Hopkin statistics to learn clusterability.
KL divergence to measure classifiers' similarities.
