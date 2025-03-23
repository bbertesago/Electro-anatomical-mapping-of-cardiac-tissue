# Problem

The third checkpoint requires the development of a numerical strategy to estimate the unknown parametric field $ c(x,y)$, describing the velocity in the tissue, from timings recorded in the 20 electrodes of the mapping catheter. 

The algorithm should output the following information:
- your estimates of the unknown parametric field $c(x,y)$.

The algorithm should be uploaded to the group's branch of the main repository following the signature proposed in the checkpoint3.ipynb file.

# Physics based model

Let us consider the Eikonal model: given c(x,y), find T(x,y)

\begin{aligned}
  & c(x,y) \sqrt{ \nabla T(x,y) D \nabla T(x,y)} = 1  \,, \quad (x,y) \in [-1.5,1.5] \times [-1.5,1.5]\,,\\
  & u(x,y) = 0  \,, \qquad \qquad \qquad \qquad \qquad x=x_0,y=y_0 \,, \\
\end{aligned}

where 
\begin{aligned}
D = 1\ \vec{b} \otimes \vec{b} + \frac{1}{a_{ratio}}  \ \vec{a} \otimes \vec{a},
\end{aligned}
being $ \vec{b} = \vec{b}(\theta) $ the fiber orientation and $ \vec{a} = \vec{a}(\theta) $ the cross-fiber orientation (orthogonal to $ \vec{b}$).

The following parameters are unknown, but they take the same value for all samples:
- the fiber angle $\theta$, 
- anisotropy ratio $a_{ratio}$,
- the starting point position $y_0$.


## Evaluation

The evaluation of the checkpoint will be based on a test dataset that is not available to you. Your algorithm's performance will be scored out of a maximum of 2 points and the evaluation metric will consider the accuracy of the approximation.
A bonus point will be awarded to the group of students who implement the algorithm with the best balance between efficiency and accuracy.

## Dataset

The dataset comprises a set of 100 recordings composed by:
1. location of the measurements,
2. recorded timings.
2. associated field.


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