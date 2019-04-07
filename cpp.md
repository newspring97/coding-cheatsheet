# C++ Cheatsheet
Cheatsheet for PS.

C++ Version: C++11

## Header files
```c++
#include <iostream> // standard library for C++
#include <string> // string library for C++
#include <algorithm> // includes functions such as sort, find, etc
```

## Data Types
```c++
void // Void type
char // Character type
bool // Boolean type
int // Integer type
long // Long Integer type
```

## Data Structures

### Vector
```c++
/*
  vector<T> is a dynamic container for certain data type T.
  include "vector" header file to use vector.
*/

#include <vector>

// vector of int element
vector<int> vec, vec2;
int n;
vector<int>::iterator loc;
// size of vec. return int.
vec.size();
// add n to the end of vec. return nothing.
vec.push_back(n);
// delete the last element of vec. return nothing.
vec.pop_back();
// return the first element of vec.
vec.front();
// return the last element of vec.
vec.back();
// return the n-th element of vec.
vec.at(n);
// clear vec. return nothing.
vec.clear();
// check if vec is empty. return bool.
vec.empty();
// insert n on the location loc of vec.
// return the location of the inserted element.
vec.insert(loc, n);
// insert the vec2's elements(from vec2.begin() to vec2.end()-1) on the loc.
// return the location of the first of the newly inserted elements.
vec.insert(loc, vec2.begin(), vec2.end());
// swap the element of two vectors. return nothing.
vec.swap(vec2);
```

### Deque, Stack, Queue
* Deque: double-ended queue
```c++
/*
  stack<T> is a deque for certain data type T.
  include "deque" header file to use deque.
*/

#include <deque>

// deque of int element
deque<int> dq, dq2;
int n, m;
deque<int>::iterator loc;
// add n at the front/back. return nothing.
dq.push_front(n);
dq.push_back(n);
// remove the first/last element of dq. return nothing.
dq.pop_front();
dq.pop_back();
// return the first/last element of dq
dq.front();
dq.back();
// return the size of dq
dq.size();
// insert n on the certain location loc of dq. return the location of n
dq.insert(loc, n);
// insert n on the certain location loc of dq m times
dq.insert(loc, m, n);
// insert dq2's elements (from dq2.begin() to dq2.end()-1) on the certain location loc
dq.insert(loc, dq2.begin(), dq2.end());
// clear contents of the dq. return nothing
dq.clear();
// check if dq is empty. return bool.
dq.empty();
// swap contents of two dqs. return nothing.
dq.swap(dq2) // swap(dq, dq2);
```

* Stack
```c++
/*
  stack<T> is a stack for certain data type T.
  include "stack" header file to use stack.
*/

#include <stack>

// stack of int element
stack<int> stk, stk2;
int n;
// add n on stk. return nothing.
stk.push(n);
// remove the top element of stk. return nothing.
stk.pop();
// return the top element of stk
stk.top();
// clear stk. return nothing
stk.clear();
// return the size of stk.
stk.size();
// check if stk is empty. return bool.
stk.empty();
// swap the element of two stacks. return nothing.
stk.swap(stk2); // swap(stk, stk2);
```

* Queue
```c++
/*
  queue<T> is a queue for certain data type T.
  include "queue" header file to use queue.
*/

#include <queue>

// queue for int elements
queue<int> q, q1;
int n;
// add element n on q. return nothing.
q.push(n);
// remove the tail element of q. return nothing.
q.pop();
// return the top element of q
q.front();
// return the tail element of q
q.back();
// return the size of q
q.size();
// clear the queue. return nothing.
q.clear();
// check if q is empty. return bool.
q.empty();
// swap the element of two queues. return nothing.
q.swap(q2); // swap(q, q2);
```

### Pair, Tuple
* Pair
```c++
/*
  pair<T1, T2> is a pair that has data type T1 as first and data type T2 as second.
  include "utility" header to use pair
*/
#include <utility>

// pair for <int, int>
pair<int, int> p, p1;
// make pair
p = make_pair(1, 2);
// first element of pair
p.first;
// second element of pair
p.second;
```

* Tuple
```c++
/*
  tuple<T1, T2> is a tuple that has data type T1 as first element and data type T2 as second element.
  include "tuple" header to use tuple.
*/
#include <tuple>

// make tuple
int n, m;
tuple<int, int> t(n, m);
auto t1 = make_tuple("a", n, 1.2, 'a');
// return the n-th element of tuple
get<0>(t); // return n
// unpack elements of tuple
tie (e1, e2) = t; // e1 = n, e2 = m
```


### Map, Set
* Map
```c++
/*
  map<T1, T2> is a map that use data type T1 as a key and data type T2 as an element.
  include "map" header to use map.
*/
#include <map>

// map for int key & int element
map<int, int> m, m1;
int k, n;
map<int, int>::iterator it, it1;
// add <k, n> where k is the key & n is the element
m.insert(pair<int, int>(k, n)); // m.emplace(k, n);
// get the iterator of the element with key k
it = m.find(k);
// erase the element
m.erase(k); // m.erase(it);
// get the element with key k
m[k];
// empty, clear, swap do as same as other ds's member functions
// key_comp/value_comp: compare key/value. return the comparison object
m.key_comp(it, it1);
// return the number of elements with key k
m.count(k);
```

* Set
```c++
```

### etc

## Iterator

## Algorithm
Built-in functions in algorithm header file.
```c++
```
