## Important Terminology related to Decision Trees

**Root Node**: It represents the entire population or sample and this further gets divided into two or more homogeneous sets.
**Splitting**: It is a process of dividing a node into two or more sub-nodes.
**Decision Node**: When a sub-node splits into further sub-nodes, then it is called the decision node.
**Leaf / Terminal Node**: Nodes do not split is called Leaf or Terminal node.
**Pruning**: When we remove sub-nodes of a decision node, this process is called pruning. You can say the opposite process of splitting.
**Branch / Sub-Tree**: A subsection of the entire tree is called branch or sub-tree.
**Parent and Child Node**: A node, which is divided into sub-nodes is called a parent node of sub-nodes whereas sub-nodes are the child of a parent node.

Assumptions while creating Decision Tree

## some of the assumptions we make while using Decision tree:

- In the beginning, the whole training set is considered as the root.
- Feature values are preferred to be categorical. If the values are continuous then they are discretized prior to building the model.
- Records are distributed recursively on the basis of attribute values.
- Order to placing attributes as root or internal node of the tree is done by using some statistical approach.

## How do Decision Trees work?

- The decision criteria are different for classification and regression trees.
- Decision trees use multiple algorithms to decide to split a node into two or more sub-nodes.
- The creation of sub-nodes increases the homogeneity of resultant sub-nodes.
- The decision tree splits the nodes on all available variables and then selects the split which results in most homogeneous sub-nodes.
- The algorithm selection is also based on the type of target variables. Let us look at some algorithms used in Decision Trees:

ID3 → (extension of D3)
C4.5 → (successor of ID3)
CART → (Classification And Regression Tree)
CHAID → (Chi-square automatic interaction detection Performs multi-level splits when computing classification trees)
MARS → (multivariate adaptive regression splines)

# ID3 algorithm --

- Buids descision tree using top down greedy search [ makes the choice that seem the best at the moment] approach through the space of possible branches with no backtracking.

- Steps in ID3 algorithm --
- - It begins with the original set S as the root node.
- - On each iteration of the algorithm, it iterates through the very unused attribute of the set S and calculates Entropy(H) and Information gain(IG) of this attribute.
- - It then selects the attribute which has the smallest Entropy or Largest Information gain.
- - The set S is then split by the selected attribute to produce a subset of the data.
- - The algorithm continues to recur on each subset, considering only attributes never selected before.

# Avoiding overfitting in descision trees--

- Pruning Decision Trees --

- - Fully grown trees is likely to ovefit the data , leading to poor accuracy on unseen data.
- - In pruning , we trim off the brnaches of the tree i.e. remove the descision nodes starting from the leaf node such that the overall accuracy is not disturbed.
- - This is done by segregating the actual training set into two sets: training data set, D and validation data set, V. Prepare the decision tree using the segregated training data set, D.
- - Then continue trimming the tree accordingly to optimize the accuracy of the validation data set, V.

- Random forest --

- - Random Forest is an example of ensemble learning, in which we combine multiple machine learning algorithms to obtain better predictive performance.
- - Two key concepts that give it the name random:

A random sampling of training data set when building trees.
Random subsets of features considered when splitting nodes.

- - Bagging is used to create an ensemble of tree where multiple training sets are generated with replacement.
- - In the bagging technique, a data set is divided into N samples using randomized sampling.
- - Then, using a single learning algorithm a model is built on all samples.
- - Later, the resultant predictions are combined using voting or averaging in parallel.

# Which is better Linear or tree-based models?

- Well, it depends on the kind of problem you are solving.

- If the relationship between dependent & independent variables is well approximated by a linear model, linear regression will outperform the tree-based model.

- If there is a high non-linearity & complex relationship between dependent & independent variables, a tree model will outperform a classical regression method.

- If you need to build a model that is easy to explain to people, a decision tree model will always do better than a linear model. Decision tree models are even simpler to interpret than linear regression!
