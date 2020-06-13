# Regression Tree

1. While decision tree predict the category (binary or multiple), the regression Tree predict the real value.
2. To be the tree, we follow the following algorithm:

```
# define a number N (that minimum number of data that can is neccessary for the tree to continue building)

N=7
tree = Tree()

def build_tree(samples):
    if len(samples)>N:
        left_samples, right_samples, node = find_node()
        add_node_to_the_tree(node, tree)
        build_tree(left_sample)
        build_tree(right_sample)
    else:
        add_leaf_to_the_tree(average(value(samples)), tree)

def find_node():
    # find the candidate of the node by
    # - calculate the Sum of Square Risidual(SSQ) of the sample of each feature
    # - choose the feature that has the least SSQ

# How to calulate the SSQ on each feature
- calculate the threshold between each two
-

```
