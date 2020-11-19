# Skelnet2D
 
| **SHREC 14**       |            |            |            |
|----------------|------------|------------|------------|
|                | 16 filters | 32 filters | 64 filters |
| AveragePooling | 95.24%          | 95.24%          | %          |
| MaxPooling     | 94.76%     | 95.60%     | 95.24%          |
| **SHREC 28**       |            |            |            |
|                | 16 filters | 32 filters | 64 filters |
| AveragePooling | 93.21%          | 93.93%          | %          |
| MaxPooling     | 92.98%          | 93.21%          | 93.45%          |


Conclusion: Average seems to works slightly better than Max, specifically for the 28 classes case.

Choice: continue Skelnet2D with Average Pooling and GlobalAveragePooling2D.