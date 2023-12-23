#import needed files

from mpl_toolkits import mplot3d
import numpy as np
import matplotlib.pyplot as plt

#creating figures and axes
fig = plt.figure()
ax = plt.axes(projection='3d')

#gathering values

z = np.linspace(0, 1, 100)
x = z * np.sin(20 * z)
y = z * np.cos(20 * z)

#plotting the graph

ax.plot3D(x, y, z, 'gray')

#giving it a title :)

ax.set_title('3D line plot')

#to show the graph

plt.show()
