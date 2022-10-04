# Usage
* **Paper**  
[Squeeze-and-Excitation Networks](https://arxiv.org/abs/1709.01507)

* **Usage Code**
```
from SEAttention import SEAttention
import torch

input = torch.randn(50,512,7,7)
se = SEAttention(channel=512,reduction=8)
output = se(input)

print(output.shape)
```