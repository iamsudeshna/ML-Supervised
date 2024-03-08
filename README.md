# ML-Supervised Decision Tress
Parameter Sweep on Decision Trees

Dataset: https://www.kaggle.com/datasets/uciml/mushroom-classification
•	We will do parameter sweep along both size and purity threshold as follows
def tree_sweep(train, test, 
                              size = [10, 20, 30, 40, 50, 60, 70, 80, 90, 100], 
                              purity = [60, 65, 70, 75, 80, 85, 90, 95]):

•	Generate the following csv file by building a decision tree with information gain as the purity measure for EACH COMBINATION of the two parameters (size, purity) i.e. (10, 60), (10, 65), …, (10, 95) … (100, 95).
tree_sweep.csv = [size, purity, training-accuracy, test-accuracy]
•	Find the most optimal tree among these with highest test-accuracy
•	Generate the Rules from the optimal tree (automatically) for the two classes
•	For the optimal value of size, plot purity vs .train/test accuracy curves 
•	For the optimal value of purity, plot size vs. train/test accuracy curves

