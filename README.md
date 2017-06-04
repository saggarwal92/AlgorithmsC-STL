# Algorithms C++ STL
Basic Functions And Usage Of C++ Standard Template Library

To use algorithms in your code, always include
```
#include<algorithm>
```

### Vectors (Dynamic Arrays)
```
  #include<vector>
```

#### Declaration: 
``` 
  vector<int> vi;
```
#### Functions:
```
  vi.size();        //Get size of vector
  vi.push_back(3);  //Pushes 3 in the end
  vi.front();       //Access the front element
  vi.back();        //Access the last element
  vi.pop_back();    //Pop the last element
```

### Sorting a vector
```
sort(vi.begin(), vi.end());   //Sorts all the elements in Ascending Order
sort(vi.begin(), vi.end(), greater<int>());   //Sorts all the elements in Descending Order
```

### Stack
```
  #include<stack>
```
#### Declaration:
```
  stack<int> s;
```
#### Functions:
```
  s.top();        //Access the top element
  s.push(3);      //Pushes 3 to the top;
  s.pop();        //Pop's the top element
  s.empty();      //Returns True if there is no element in the stack
  s.size();       //Returns the number of elements in the stack
```

### Queue
```
  #include<queue>
```
#### Declaration:
```
  queue<int> q;
```
#### Functions:
```
  q.front();      //Access the first(front) element
  q.push(3);      //Pushes 3 in the end 
  q.pop();        //Pop's the first(front) element
  q.empty();      //Returns True if there is no element in the queue
  q.size();       //Returns the number of elements in the queue
```


### Dequeue
```
  #include<queue>
```
#### Declaration:
```
  dequeue<int> dq;
```
#### Functions:
```
  dq.front();         //Access the (first)front element
  dq.back();          //Access the last element
  dq.push_back(3);    //Pushes 3 in the end - Now, 3 becomes the last element
  dq.push_front(3);   //Pushes 3 in the first - Now, 3 becomes the first element
  dq.pop_back();      //Pop's the last element in the dequeue
  dq.pop_front();     //Pop's the front element in the queue
  dq.empty();         //Returns True if there is no element in the dequeue
  dq.size();          //Returns the number of elements in the dequeue
```
#### Difference between dequeue and vector is that you can iterate through all the elements int the vector and can access any element at any position in O(1) while dequeue combines the properties of a stack and queue.


### Priority Queue
```
  #include<queue>
```
#### Declaration:
```
  priority_queue<int> pq;     //Keeps all the elements in Descending Order (Max-Heap)
  priroity_queue<int,vector<int>, greater<int>> pq;  //Keeps all the elements in Ascending Order (Min-Heap)
```  
#### Functions:
```
  pq.top();      //Access the top element
  pq.push();     //Pushes the element in the priority queue
  pq.pop();      //Pop the top element (min or max depending on the type of the priorty queue)
  pq.empty();    //Returns True if there is no element in the queue
```

#### Priority Queue can also be thought of as a heap. So, whenever you want to use Heap DataStructure, use Priority Queue.


### Map
```
  #include<map>
```
### Declaration:
```
  map<char,int> m;  //general declaration map<key_type,value_type> m;
```
### Functions:
```
  m.find('a');  //map.find(key) 
  //if key exists - it will return iterator to that key else it will return m.end()
```

  

