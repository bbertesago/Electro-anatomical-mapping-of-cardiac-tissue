# Problem

The first checkpoint requires the development of an algorithm to interpolate/extrapolate the activation time field from timings recorded in the 20 electrodes of the mapping catheter. 
The available data consists of 100 recordings, which include the location of the measurements and the recorded timings \[s\].

The algorithm should output the following information:
- a reconstruction of the activation times evaluated at each point of a structured grid on the square (-1.5, 1.5)x(-1.5, 1.5) \[cm^2\], 
- an approximation of the conduction velocity \[cm/s\] (a clinical biomarker) evaluated at each point of a structured grid on the same square.

The algorithm should be uploaded to the group's branch of the main repository following the signature proposed in the checkpoint1.ipynb file.

## Evaluation

The evaluation of the checkpoint will be based on a test dataset that is not available to you. Your algorithm's performance will be scored out of a maximum of 2 points and the evaluation metric will consider the accuracy of the approximation.
A bonus point will be awarded to the group of students who implement the algorithm with the best balance between efficiency and accuracy.

## Dataset

The dataset comprises a set of 100 recordings composed by:
1. location of the measurements,
2. recorded timings.


## Checkpoint organization


### Step 1: problem conceptualization

Create a conceptual model of the problem.

### Step 2: mathematical formulation

Formulate the problem in a mathematical form.

### Step 3: design of the algorithm

Select a proper strategy to solve the problem.

### Step 4: implementation

Implement your strategy, ensuring that it is fully reproducible by others.

### Step 5: testing phase

Your algorithm will be tested on a new dataset, to verify the effectiveness and efficiency of the procedure.

### Step 6: analysis of the performances

Review your results in view of the modeling and implementation strategies that you have employed.
