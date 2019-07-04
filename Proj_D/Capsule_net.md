# Capsule_net
27-May
[[GitHub - andyweizhao/capsule_text_classification](https://github.com/andyweizhao/capsule_text_classification)]
[Branch]:modularize/capsule_nets

* bacth size - 
  * upsampling in train
  * padding in predict
* renamed activation tensor

* inspect checkpoint
```bash
python -m tensorflow.python.tools.inspect_checkpoint --file_name=./checkpoints/model-0
``` 
* tensorboard
```bash
tensorboard --logdir=./checkpoints/
```
