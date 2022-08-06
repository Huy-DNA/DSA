# Bucket sort
> Say hellllo to the dreaded **Segmentation fault**. Implementing this algorithm has taught me the lesson to plan anything you're going to code me up front. It was a mess patching things up!!!.

Notes about this implementation of Bucket sort:
* Assumptions:
    * All elements are of floating point type.
    * All elements lie within [0, 1).
* Time complexity: With the assumptions that the elements are generated from a uniform distribution over [0, 1),
    * Average-case running time: $\Theta(n)$
    * Best-case running time: $\Theta(n)$ (ex. when every bucket has exactly one element)
    * Worst-case running time: $\Theta(n^2)$ (ex. when all elements end up in one bucket)
* Space complexity: $\Theta(n)$
* Other technical:
    * NOT stable because this specific version of Insertion sort is not stable). However, fixing this is quite trivial.
    * NOT inplace
    * Only works with random-access iterator (in C++ terminology)

Observations:
* Among the linear-time sorting algorithms I have implemented, this is the only one that works with floating point numbers and also relies on its fast average-case running time.