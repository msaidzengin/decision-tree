# Decision Tree

This is BIL 212 Data Structures Homework 2, completed on 22 January 2019.

A binary decision tree plays an animal guessing game. Internal nodes are yes/no questions (the left child is yes, the right child is no) and leaves are animals. A wrong guess adds a new question and animal to the tree. The tree can be saved and loaded in preorder.

The assignment text is `bil212summer2018hw2.pdf`. `DT.pdf` is the tree stored in `DT.txt`. `interactions.txt` is a sample play session.

## Run

From the repository root:

```bash
javac -encoding UTF-8 -d bin src/tobb/etu/decisionTree/Node.java src/tobb/etu/decisionTree/DecisionTree.java src/tobb/etu/decisionTree/AnimalPredictor.java
java -cp bin tobb.etu.decisionTree.AnimalPredictor
```

Answer the prompts with `evet` or `hayir`. To start from a saved tree, answer `evet` and give `DT.txt` or `DT2.txt`.

## Tests

The tests use JUnit 4. With `junit4.jar` on the classpath:

```bash
javac -encoding UTF-8 -cp junit4.jar -d bin src/tobb/etu/decisionTree/*.java
java -cp bin:junit4.jar junit.textui.TestRunner tobb.etu.decisionTree.TestDecisionTree
```

`query1.txt` through `query4.txt` are the query files used by the tests.
