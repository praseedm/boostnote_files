## ISSUES
- ##### TypeError: int64 is not JSON serializable
[["TypeError: (Integer) is not JSON serializable" when serializing JSON in Python? - Stack Overflow](https://stackoverflow.com/questions/11942364/typeerror-integer-is-not-json-serializable-when-serializing-json-in-python)]

It seems like there may be a issue to dump numpy.int64 into json string in Python 3

```python
def default(o):
    if isinstance(o, numpy.int64): return int(o)  
    raise TypeError

json.dumps({'value': numpy.int64(42)}, default=default)
```
- ##### Variable names that are saved in a TensorFlow checkpoint
```python
import tensorflow.python.tools.inspect_checkpoint
```

[[tensorflow - How do I find the variable names and values that are saved in a checkpoint? - Stack Overflow](https://stackoverflow.com/questions/38218174/how-do-i-find-the-variable-names-and-values-that-are-saved-in-a-checkpoint/41917296)]