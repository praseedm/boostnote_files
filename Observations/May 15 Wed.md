### May 15 Wed
##### SpeedUp Model Loading
- Multiprocess : 
    - Multiprocessing.Pool()
TypeError: can't pickle _thread.RLock objects

  - Multiprocess.pool.ThreadPool
  Solved by replacing multiprocess with multithread
  
##### pickle vs dill
[python - Why does pickling a tensorflow Tensor fail? - Stack Overflow](https://stackoverflow.com/questions/43769390/why-does-pickling-a-tensorflow-tensor-fail)
##### multiprocessing vs pathos

##### Tensorflow
* tools.inspect_checkpoint
```bash
python -m tensorflow.python.tools.inspect_checkpoint --file_name=./checkpoints/model-0
``` 
* tensorboard
```bash
tensorboard --logdir=./checkpoints/
```
##### GridSearch with OnevsRest
https://stackoverflow.com/questions/12632992/gridsearch-for-an-estimator-inside-a-onevsrestclassifier