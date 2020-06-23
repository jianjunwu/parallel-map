# A multiprocessing wrapper of map
# Install
```
pip install parallelmap
```
# Example
```
import numpy as np
from parallelmap import parallel_map

def add(x, y):
    return x + y

data1 = np.arange(1000000)
data2 = np.arange(1, 1000001)
```

```
# defualt all available CPUs will be used
parallel_map(add, data1, data2)
```

```
# set running workers
parallel_map(add, data1, data2, nb_workers=2)
```

```
# set progress bar
parallel_map(add, data1, data2, progress_bar=True)
```
![进度条](./images/img1.jpg)
 
