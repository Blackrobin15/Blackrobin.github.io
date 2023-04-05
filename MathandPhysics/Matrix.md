<head>
    <script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
    <script type="text/x-mathjax-config">
        MathJax.Hub.Config({
            tex2jax: {
            skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
            inlineMath: [['$','$']]
            }
        });
    </script>
</head>

# Matrix

This part is for some basic matrix operations and realize with numpy.

### Basic operation

1. Plus  
$$A+B = B+A$$  

In the math, the shapes of A and B should be <b>the same </b>for the plus-operation.
``` python
A = np.ones([5,3])
B = np.random.rand(5,3)
print("A =",A,'\n',
    "B=",B,'\n',
    "Sum",A+B)
```

The result is showed:
``` bat
A = [[1. 1. 1.]
 [1. 1. 1.]
 [1. 1. 1.]
 [1. 1. 1.]
 [1. 1. 1.]] 
 B= [[0.21061476 0.05742014 0.08478811]
 [0.51327516 0.19127396 0.52860533]
 [0.17499047 0.27733645 0.52808495]
 [0.14035961 0.92411563 0.65923648]
 [0.98960638 0.10502168 0.74458856]] 
 Sum [[1.21061476 1.05742014 1.08478811]
 [1.51327516 1.19127396 1.52860533]
 [1.17499047 1.27733645 1.52808495]
 [1.14035961 1.92411563 1.65923648]
 [1.98960638 1.10502168 1.74458856]]
```

In the numpy, we <b> do not have to</b> match the matrix in a same shape

``` python
import numpy as np
A = 1.
B = np.random.rand(5,3)
print("A =",A,'\n',
    "B=",B,'\n',
    "Sum",A+B)

```

The result is:
``` bat
A = 1.0 
 B= [[0.85485835 0.98161483 0.01390224]
 [0.79383868 0.29771132 0.0713353 ]
 [0.55058842 0.29345741 0.31880754]
 [0.05390459 0.68531902 0.35922624]
 [0.36074392 0.32126726 0.74901425]] 
 Sum [[1.85485835 1.98161483 1.01390224]
 [1.79383868 1.29771132 1.0713353 ]
 [1.55058842 1.29345741 1.31880754]
 [1.05390459 1.68531902 1.35922624]
 [1.36074392 1.32126726 1.74901425]]
```

2. Multiple  
It can 

3. Transpose
4. Determinant(行列式)
5. Jacobi
7. Inverse
8. Rank
9. Trace