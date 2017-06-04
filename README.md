# AlgorithmsC-STL
Basic Functions And Usage Of C++ Standard Template Library

To use algorithms in your code, always include
#include<algorithm>

### Vectors
```
#include<vector>
 
Declaration: 
  vector<int> vi;
Functions:
  vi.size();        //Get size of vector
  vi.push_back(3);  //Pushes 3 in the end
  vi.front();       //Access the front element
  vi.back();        //Access the last element
  vi.pop_back();    //Pop the last element
```

###Sorting a vector:
```
sort(vi.begin(), vi.end());   //Sorts all the elements in Ascending Order
sort(vi.begin(), vi.end(), greater<int>());   //Sorts all the elements in Descending Order
```

### Stack
```
#include<stack>

Declaration:
  stack<int> s;
Functions:
  s.top();     //Access the top element
  s.push(3);   //Pushes 3 to the top;
  s.pop();     //Pop's the top element
  s.empty();   //Returns True if there is no element in the stack
```

### Queue
```
#include<queue>

Declaration:
  queue<int> q;
Functions:
  q.front();      //Access the first(front) element
  q.push(3);      //Pushes 3 in the end 
  q.pop();        //Pop's the first(front) element
  q.empty();      //Returns True if there is no element in the queue
```


### Priority Queue
```
#include<queue>

Declaration:
  priority_queue<int> pq;     //Keeps all the elements in Descending Order (Max-Heap)
  priroity_queue<int,vector<int>, greater<int>> pq;  //Keeps all the elements in Ascending Order (Min-Heap)
Functions:
  pq.top();      //Access the top element
  pq.push();     //Pushes the element in the priority queue
  pq.pop();      //Pop the top element (min or max depending on the type of the priorty queue)
  pq.empty();    //Returns True if there is no element in the queue
  

Priority Queue can also be thought of as a heap. So, whenever you want to use Heap DataStructure, use Priority Queue.
```


  

