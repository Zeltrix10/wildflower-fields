import matplotlib.pyplot as plt
import numpy as np

# Create random points for wildflowers
n_flowers = 500
x = np.random.rand(n_flowers) * 100
y = np.random.rand(n_flowers) * 100

# Create a scatter plot to represent the flowers
plt.figure(figsize=(10, 10))
plt.scatter(x, y, color='purple', s=20)

# Adding some green grass effect
for i in range(200):
    plt.scatter(np.random.rand(20) * 100, np.random.rand(20) * 100, color='green', s=2)

plt.title('Wildflower Field')
plt.xlabel('Width')
plt.ylabel('Height')
plt.show()
