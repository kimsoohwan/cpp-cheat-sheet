# Summary
## Sequence Containers
**array** (C++11)
   * **[]: random access O(1)**

**vector**
   * []: random access by index, O(1)
   * **push_back, pop_back: dynamic allocation, O(1)**
   
**deque** (contiguous memory not guaranteed)
   * []: random access by index, O(1)
   * push_back, pop_back: dynamic allocation, O(1)
   * **push_front, pop_front: dynamic allocation, O(1)**

**list**, **forward_list**(C++11) (double/single linked list)
   * push_back, pop_back: dynamic allocation, O(1)
   * push_front, pop_front: dynamic allocation, O(1)
   * **insert: O(1)**


## Associative Containers
**set, multiset** (ordered, binary search tree)
   * **insert, remove, find: O(log(n))**

**map, multimap** (ordered, binary search tree)
   * insert, remove, find: O(log(n))
   * **[]: random access by key, O(log(n))**
   * [] (overwrite) vs. insert (if no key exists)

**unorderd_set, unorderd_multiset** (C++11, unordered, hash table)
   * **insert, remove, find: O(1)**

**unorderd_map, unorderd_multimap** (C++11, unordered, hash table)
   * insert, remove, find: O(1)
   * **[]: random access by key, O(1)**
   * [] (overwrite) vs. insert (if no key exists)


## Container Adaptors
**stack** (LIFO, standard container: deque)
   * push, pop, top, O(1)

**queue, priority_queue** (FIFO, standard container: deque, ordered/unordered)
   * push, pop, front, back, O(1)


## Some Links
* https://baptiste-wicht.com/posts/2012/12/cpp-benchmark-vector-list-deque.html
* http://www.ccplusplus.com/2014/01/stl-deque-example-c.html
* http://homepages.e3.net.nz/~djm/cppcontainers.html
