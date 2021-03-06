[<img src="https://github.com/QuantLet/Styleguide-and-FAQ/blob/master/pictures/banner.png" width="888" alt="Visit QuantNet">](http://quantlet.de/)

## [<img src="https://github.com/QuantLet/Styleguide-and-FAQ/blob/master/pictures/qloqo.png" alt="Visit QuantNet">](http://quantlet.de/) **XFGdtmDirichlet** [<img src="https://github.com/QuantLet/Styleguide-and-FAQ/blob/master/pictures/QN2.png" width="60" alt="Visit QuantNet 2.0">](http://quantlet.de/)

```yaml

Name of Quantlet: XFGdtmDirichlet

Published in: Applied Quantitative Finance (3rd Edition)

Description: Simulates and plots the Dirichlet distribution with various values for alpha.

Keywords: simulation, distribution, plot, graphical representation, visualization

Author[m]: Ernie Teo
Author[py]: Philipp Schneider, WK Härdle


See also : 

- LDA-DTM_Christmas_Song

Submitted[py] :  Wed 4. April 2019 by WK Härdle and Philipp Schneider


```

![Picture1](XFGdtmDirichlet_1.png)

![Picture2](XFGdtmDirichlet_2.png)

![Picture3](XFGdtmDirichlet_3.png)

![Picture4](XFGdtmDirichlet_4.png)

### PYTHON Code
```python



import numpy as np
import matplotlib.pyplot as plt
from mpl_toolkits.mplot3d import axes3d

n=2000

# Plot 1
fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')

a=(1,1,1)

s = np.random.dirichlet(a, n)
x = s[:,0].tolist()
y = s[:,1].tolist()
z = s[:,2].tolist()

ax.scatter(x, y, z, c='r', marker='o')

ax.set_xlabel('X Label')
ax.set_ylabel('Y Label')
ax.set_zlabel('Z Label')

ax.view_init(elev=40., azim=40)

plt.show()
#### STOP##########


# Plot 2
fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')

a=(0.1,0.1,0.1)

s = np.random.dirichlet(a, n)
x = s[:,0].tolist()
y = s[:,1].tolist()
z = s[:,2].tolist()

ax.scatter(x, y, z, c='r', marker='o')

ax.set_xlabel('X Label')
ax.set_ylabel('Y Label')
ax.set_zlabel('Z Label')

ax.view_init(elev=40., azim=40)

plt.show()
#### STOP##########


# Plot 3
fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')

a=(10,10,10)

s = np.random.dirichlet(a, n)
x = s[:,0].tolist()
y = s[:,1].tolist()
z = s[:,2].tolist()

ax.scatter(x, y, z, c='r', marker='o')

ax.set_xlabel('X Label')
ax.set_ylabel('Y Label')
ax.set_zlabel('Z Label')

ax.view_init(elev=40., azim=40)

plt.show()
#### STOP##########


# Plot 4
fig = plt.figure()
ax = fig.add_subplot(111, projection='3d')

a=(2,5,15)

s = np.random.dirichlet(a, n)
x = s[:,0].tolist()
y = s[:,1].tolist()
z = s[:,2].tolist()

ax.scatter(x, y, z, c='r', marker='o')

ax.set_xlabel('X Label')
ax.set_ylabel('Y Label')
ax.set_zlabel('Z Label')

ax.view_init(elev=40., azim=40)

plt.show()

```

automatically created on 2019-04-04

### MATLAB Code
```matlab

n = 2000;

% Plot 1
a = [1 1 1];
r = drchrnd(a,n);

HD        = scatter3(r(:,1),r(:,2),r(:,3),'MarkerFaceColor',[1 0 0]);
direction = [0 0 1];
view(-40,-18)

% Plot 2
a = [.1 .1 .1];
r = drchrnd(a,n);
HD        = scatter3(r(:,1),r(:,2),r(:,3),'MarkerFaceColor',[1 0 0]);
direction = [0 0 1];
view(-40,-18)

% Plot 3
a = [10 10 10];
r = drchrnd(a,n);
HD        = scatter3(r(:,1),r(:,2),r(:,3),'MarkerFaceColor',[1 0 0]);
direction = [0 0 1];
view(-40,-18)

% Plot 4
a = [2 5 15];
r = drchrnd(a,n);
HD        = scatter3(r(:,1),r(:,2),r(:,3),'MarkerFaceColor',[1 0 0]);
direction = [0 0 1];
view(-40,-18)
```

automatically created on 2019-04-04