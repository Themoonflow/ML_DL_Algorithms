
![Residual Neural Networks](https://miro.medium.com/max/1400/1*cIKFeG7ZIl9D-VnSF0KAZA.png)

### Residual Neural Networks 
#### Assumption
Theoretically, neural networks should get better results as they have more layers.
An identity mappping be added as part of output X. A neural network should be able to learn at least the identity mapping if it doesn’t find something better than that.

#### Reality
But in practice, as we add more layers, the network gets better results until at some point; then as we continue to add extra layers, the accuracy starts to drop.

#### ResNet as a Solution
Residual Networks attempt to solve this issue by adding the so-called skip connections. 
Deeper networks should be able to learn at least identity mappings; this is what skip connections do: they add identity mappings from one point in the network to a forward point, and then lets the network to learn just that extra 𝐹(𝑥). If there are no more things the network can learn, then it just learns 𝐹(𝑥) as being 0. It turns out that it is easier for the network to learn a mapping closer to 0 than the identity mapping.
