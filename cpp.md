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
int n = 0;
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
* Deque
```c++
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

### Map, Set
* Map
```c++
```

* Set
```c++
```

### Pair, Tuple
* Pair
```c++
```

* Tuple
```c++
```

### etc

## Iterator

## Algorithm
Built-in functions in algorithm header file.
```c++
```
