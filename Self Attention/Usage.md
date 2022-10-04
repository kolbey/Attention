# Usage
* **Paper**  
[Attention Is All You Need](https://arxiv.org/pdf/1706.03762.pdf)

* **Usage Code**
```
from Self_Attention import ScaledDotProductAttention
import torch

input = torch.randn(50,49,512)
sa = ScaledDotProductAttention(d_model=512,d_k=512,d_v=512,h=8)
output = sa(input, input, input)
print(output.shape)
```