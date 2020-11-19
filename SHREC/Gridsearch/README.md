# Skelnet2D

Initial hyperparameters:
1. Batch_size = 32
2. Dropout = 0.1
3. Initialization
4. LeakyRelu = 0.2
5. Optimizer: Adam
6. Sequence Length = 32
7. Spatial Dropout = 0.1
8. Dense 2 layers 128 perceptrons

**Training callbacks**: 
ReduceLROnPlateau(monitor='val_loss', factor=0.2,
                              patience=10, min_lr=1e-8)

EarlyStopping(monitor='val_loss', mode='min', verbose=1, patience=50)
 
##Order of optimization:


* **AveragePool vs MaxPool**

| **SHREC 14**       |            |            |            |
|----------------|------------|------------|------------|
|                | 16 filters | 32 filters | 64 filters |
| AveragePooling | 95.24%          | 95.24%          | 95.48%          |
| MaxPooling     | 94.76%     | 95.60%     | 95.24%          |
| **SHREC 28**       |            |            |            |
|                | 16 filters | 32 filters | 64 filters |
| AveragePooling | 93.21%          | 93.93%          | 92.62%          |
| MaxPooling     | 92.98%          | 93.21%          | 93.45%          |

Conclusion: Average seems to works slightly better than Max

Choice: continue Skelnet2D with Average Pooling and GlobalAveragePooling2D.

* **Optimizer**

* **SequenceLength**

* **Batch_size**

* **SpatialDroput**

* **Dropout**

* **Init**

* **LeakyRelu*