# color-detection
model 6 -> 
(currently) (using 10000 train data, 1000 val data, 200 test data)
conv, batchnorm, relu, maxpool, layer1(2 basic blocks), layer2(2 basic blocks), concat(GAP of layer 1 and GAP of layer 2), branching
branch 1 FC(192, 11)
branch 2 FC(192, 11)
val acc ~ 91%
(modifications possible)
1)Freeze resnet layers and then train others
2)Use full dataset
3)Remove GAP
4)Applying some conv layers to downscale the size of output of layer1 and layer2

