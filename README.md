# [hy-numpy](http://cs231n.github.io/python-numpy-tutorial/)

* 1. numpy
```clojure
=> (import [numpy :as np])
=> (setv a (np.array [1 2 3]))
=> (type a)
<type 'numpy.ndarray'>
=> a.shape
(3,)
=> (print a[0] a[1] a[2])
[1 2 3] [0L] [1 2 3] [1L] [1 2 3] [2L]
=> a[0]
array([1, 2, 3])
[0L]
=> a[-1]
array([1, 2, 3])
[-1L]
=>
```
* 2. numpy + matplotlib + pandas

```clojure
=> (import [matplotlib.pyplot :as plt])
=> (import [numpy :as np])
=> (import [pandas :as pd])
=> (setv df (pd.read_csv "https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data" :header None))
=> (setv x (. df.iloc [(slice 0 100)] [[0 2]] values))
=> (. x [(slice None 50)] [0])
array([ 5.1,  1.4])
=>
```
* 3. 用matplotlib绘图
```clojure

```
