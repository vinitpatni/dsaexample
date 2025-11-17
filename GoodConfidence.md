- num of islands (graph dfs)
     <pre markdown="2"> 
       TimeComplexity -> O(m*n)
       SpaceComplexity ->O(m*n) in the worst case due to the recursion stack but auxiallary space can be O(1) wtihout 
       using visibility matrix to track visited cell, just flip 1 to 0 after visiting</pre>
- all powersets (recursive backtracking)
- two numbers.  (array)
    <pre markdown="2">  
     TimeComplexity -> O(n) 
     SpaceComplexity -> O(n) Using Map to store number and index mapping</pre>
- two numbers sorted array
    <pre markdown="2">
    TimeComplexity -> O(n) 
    SpaceComplexity -> O(1) As no auxiallary space is needed for sorted array</pre>
- Number of Provinces (dfs)
    <pre markdown="2">
    TimeComplexity -> O(n2) As we need to traverse through the 2d array to find connections 
    SpaceComplexity -> O(n) Because of recursion stack consist on minimum n calls and we are using boolean visited array of size n</pre>
    
- My Calendar 1 (interval tree)
- Check Validity of BST (tree)
    <pre markdown="2">
    TimeComplexity -> O(n) As we need to traverse through each element of tree once to validate it 
    SpaceComplexity -> O(logn) Because of recursion stack mostly goes upto the depth which is equal to height of the tree which is log(n)
                      For skewed binary search tree, it can be O(n) which is not case most of the time</pre>
- Sudoku Solver. (recursive backtracking)
- Sliding Window Maximum (sliding window)
- level order traversal (tree)
   <pre markdown="2">
   TimeComplexity -> O(n) as we are travesing each node once
   SpaceComplexity ->O(n) as in worst case max no of elements at level can be n/2 which we are storing in Queue</pre>
- Bottom level order traversal (same as level order traversal but use LinkedList to add at start, which supports addFirst method)  
- reverse stack with recursion(Stack)
- merge k sorted array (using priority queue)
bulb right flip (greedy approach)
daily temperature (monotonic stack)
first non repeating number in stream (queue)
min stack (Stack) use Single Stack
implement queue using two stack
peak in mountain array (using binary search)
find in mountain array (double binary search)
wordsearch (dfs backtracking)
reverse words (String)
min window substring (sliding window)
longest-substring-without-repeating-characters(sliding window)
network delay time : (Dijkistra algortihm)
Design inmemory file system
serialize and deserialize n-ary tree
Snapshot Array :- (use binary search)
encode and decode list of strings
Visible people of queue :- (use monotonic stack)
searilize and deseralize tree :- use preorder traversal
Longest palindrome substring (dynamic programming and tabulation technique)

kth largest element in stream
meetings room (interval )
diameter of tree (tree dfs)
- Max Area of Island (Graph dfs)
  TimeComplexity -> O(m*n)
  SpaceComplexity ->O(m*n) in the worst case due to the recursion stack but auxiallary space can be O(1) wtihout using visibility matrix to track visited cell, just flip 1 to 0 after visiting 
Disappering elements in array (cyclic sort)
longest palindromic substring (tabulation technique using bottomsup approach)
