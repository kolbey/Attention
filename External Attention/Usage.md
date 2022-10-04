# Usage
* **Paper**  
[Beyond Self-attention: External Attention using Two Linear Layers for Visual Tasks](https://arxiv.org/abs/2105.02358)

* **Usage Code**
```
from ExternalAttention import ExternalAttention
import torch

input = torch.randn(50,49,512)
ea = ExternalAttention(d_model=512,S=8)
output = ea(input)
print(output.shape)
```