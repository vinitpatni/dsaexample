- Number of Islands (graph dfs)
     <pre markdown="2"> 
       TimeComplexity -> O(m*n)
       SpaceComplexity ->O(m*n) in the worst case due to the recursion stack but auxiallary space can be O(1) wtihout 
       using visibility matrix to track visited cell, just flip 1 to 0 after visiting</pre>
- Fair Distribution of Cookies (backtracking and pruning)
    <pre markdown="2"> 
       Apprach 1 :- We are doing backtracking doing enumeration for each cookie bag, can pruning branch if evaluated max is greater than
                    current answer
       TimeComplexity -> O(k pow n/factorial(n))
       SpaceComplexity ->O(n+k) Recursive backtracking call would be n equal to no of elements in array</pre>
- All Powersets (recursive backtracking)
     <pre markdown="2"> 
       TimeComplexity -> O(2 pow n)
       SpaceComplexity ->O(n) Recursive backtracking call would be n equal to no of elements in array</pre>
- daily temperature (monotonic stack)
    <pre markdown="2"> 
       Approach 1 :- An element can be maximum inserted 1 time and pop 1 times, size of Stack will never exceed n
         TimeComplexity -> O(n)
         SpaceComplexity -> O(m*n)
     </pre>
- Prefix Tree (Trie)
      <pre markdown="2"> 
          - Add, Search and Search Prefix
            TimeComplexity -> O(m) where m is size of each string
            SpaceComplexity -> O(m*n) where m is avg size of each string and n is total no of strings
           
     </pre>     
- All Permutations (recursive backtracking)
- Palindrome Partitioning (recursive backtracking)
    <pre markdown="2"> 
            TimeComplexity -> O(n * 2 pow n) finding all substring of string of size n is 2 pow n and checking for each string whether it is palindrome
            SpaceComplexity -> O(n) depth of recursion is equal to size of string
   </pre>     
- Burning Tree  (BFS to find shortest path)
    <pre markdown="2"> 
       Approach 1 :-  Using dfs to create adjancecyList of tree and bfs to find shortest path from one node to all the nodes of tree
          TimeComplexity :- O(n)
          SpaceComplexity :- O(n) + O(log(n)), auxillary map to store adjancencyLIst, recursive stack call for dfs 
     </pre>
- Rotting Oranges (Same as Burning Tree, only 2d array is present instead of Tree)     
- Compare leaves of binary tree
     <pre markdown="2"> 
       Approach 1 :-  Using dfs to collect all leaves of both the trees and compare leaves
          TimeComplexity :- O(l1+l2) where l1 and l2 no of leaf nodes
          SpaceComplexity :- O(h1+h2) + O(l1+l2) h1,h2 => heights and l1+l2 => no of leaf nodes
      Approach 2 (With less space) :- Use iterative approach and short circuit while comparing leaves
         TimeComplexity :- O(min(l1,l2)) where l1 and l2 no of leaf nodes
         SpaceComplexity :- O(h1+h2) h1,h2 => heights
     </pre>
- Two numbers  (array)
    <pre markdown="2">  
     TimeComplexity -> O(n) 
     SpaceComplexity -> O(n) Using Map to store number and index mapping</pre>
- Two numbers (sorted array)
    <pre markdown="2">
    TimeComplexity -> O(n) 
    SpaceComplexity -> O(1) As no auxiallary space is needed for sorted array</pre>
- Arrange -ve and +ve numbers in the array (maintain their order)
   <pre markdown="2"> 
     Approach 1 :-  Use Two for each loop and compare each pair of string using anagram algo 
        TimeComplexity :- Create separate list of negative and positive number which has complexity of O(n) and combine them to get final result
                           
        SpaceComplexity :- O(n)
         
     Approach 2 (Better) :- Use Modified Merge Sort. 
          How to combine  (-2,2,1) (-3,-4,1), 
            - swap (-2,(1,2)) and ((-4,-3),1)
            - reverse from 1 to 4 index which should be (-2, -3, -4, 1, 2,1) which is expectation
        TimeComplexity :- O(nlogn) 
        SpaceComplexity :- O(logn) as we are doing log(n) calls which is depth of merge tree </pre>
- Find All Duplicates in an Array Or (Find All Missing Numbers in an Array)
    <pre markdown="2">  
     Approach 1 :- Use Cyclic Sort to put elments in its expected place     
        TimeComplexity -> O(n) 
        SpaceComplexity -> O(1) </pre>          
- Group Anagrams
    <pre markdown="2"> 
     Approach 1 :-  Use Two for each loop and compare each pair of string using anagram algo 
        TimeComplexity :- O(n2m) for worst case where m is size of each string and n is the size of string array. 
                            O(m+m) is cost of comparing two string of size m and we are doing it n2 times
        SpaceComplexity :- we can use auxillary visited boolean array of size n to mark string which are already grouped
         
     Approach 2 (Better) :- Sort each string and store it in map with value as sorted string, Only single itr is needed 
        TimeComplexity :- O(nmlog(m)) mlogm is needed to sort string (Arrays.sort) of size m and it is done n times
        SpaceComplexity :- O(nm) which is used to store results </pre>
         
- Number of Provinces (dfs)
    <pre markdown="2">
    TimeComplexity -> O(n2) As we need to traverse through the 2d array to find connections 
    SpaceComplexity -> O(n) Because of recursion stack consist on minimum n calls and we are using boolean visited array of size n</pre>
    
- My Calendar 1 (interval tree)
- Longest Substring Without Repeating Characters (two pointers)
   <pre markdown="2">
    TimeComplexity -> O(n) As we need to scan each character of string once 
    SpaceComplexity -> O(n) Because we are using hashset which can contain each character in worst case</pre>
- Check Validity of BST (tree)
    <pre markdown="2">
    TimeComplexity -> O(n) As we need to traverse through each element of tree once to validate it 
    SpaceComplexity -> O(logn) Because of recursion stack mostly goes upto the depth which is equal to height of the tree which is log(n)
                      For skewed binary search tree, it can be O(n) which is not case most of the time</pre>
- Kth Largest Element in an Array
    <pre markdown="2">
    TimeComplexity -> O(nlog(k)) Use priority queue and maintain height of k
    SpaceComplexity -> O(k) As height of queue never exceeds k</pre>                      
- Smallest kth element in BST (tree)
    <pre markdown="2"> 
       Approach 1 :-  Using inorder traversal to collect all nodes and fetch kth element as result
          TimeComplexity :- O(n) where n is not nodes
          SpaceComplexity :- O(n) recursive calls + O(n) auxillary list to collected n elemnts;
      Approach 2 (With less space) :- Use counter and short circuit while comparing leaves
          TimeComplexity :- O(n) where n is not nodes
          SpaceComplexity :- O(n) recursive calls + O(1) as we set result and exit from function once count reaches k;
     </pre>
- Sudoku Solver. (recursive backtracking)
- Sliding Window Maximum (sliding window)
- level order traversal (tree)
   <pre markdown="2">
   TimeComplexity -> O(n) as we are travesing each node once
   SpaceComplexity ->O(n) as in worst case max no of elements at level can be n/2 which we are storing in Queue</pre>
- Bottom level order traversal (same as level order traversal but use LinkedList to add at start, which supports addFirst method)
- Zigzag level order traversal (same as level order traversal but use LinkedList (addFirst method) at odd level to reverse the order of elements)
- reverse stack with recursion(Stack)
- merge m sorted array of size n same as merge m sorted linked list 
   <pre markdown="2"> 
       Approach 1 :- maintain index for each array and compare each element of all arrays at that index and then increment index which has lowest value
          TimeComplexity :- m * m * n where m comparisons is needed for mn elements
          SpaceComplexity :- O(mn) to store results
      Approach 2 :- Use Priority Queue of size m and just insert element in priority queue for index which got the lowest value
          TimeComplexity :- O(log(m) * m * n) where m no of arrays of size n each
          SpaceComplexity :-  O(mn) to store results and O(m) size for priority Queue
     </pre> 
- bulb right flip (greedy approach)
- minimize difference between min and max of high scores (greedy approach)
   <pre markdown="2"> 
       Approach 1 :- Sort it in increasing order as, Any skipping only increases the range
          TimeComplexity :- O(k*nlogn) as we are populating the dp table
          SpaceComplexity :- O(n) for storing the result of computation
  </pre>
- serialize and deserialize n-ary tree
- Longest palindrome substring (same as palidromic substrings)
  <pre markdown="2"> 
       Approach 1 :- Use dynamic programming and create dp table dp[i][j].Mark dp[i][j] as palidnrome if character at index i == character at index j && dp[i+1][j-1] is palindrome
          TimeComplexity :- O(n*n) as we are populating the dp table
          SpaceComplexity :- O(n*n) for storing the result of computation
  </pre>
- searilize and deseralize tree
      <pre markdown="2"> 
       Approach 1 :- Use Preorder traversal to store elements while serialize and Queue while deserialize 
          TimeComplexity :- O(n) as we are dfs 
          SpaceComplexity :- log(n) for recursion depth and queue which takes O(n) to store elements 
     </pre>
- Parallel courses (topological sorting with level order traversal technique)
      <pre markdown="2"> 
       Approach :- Do topological Sorting using adjacency list and indegree map 
          TimeComplexity :- O(V + E)
          SpaceComplexity :- O(V) not considering adjanceny list space and auxillary space for queue (which can be o(V) in worse case if many nodes are with incoming degree as zero)
     </pre>
- Max Area of Island (Graph dfs)
  TimeComplexity -> O(m*n)
  SpaceComplexity ->O(m*n) in the worst case due to the recursion stack but auxiallary space can be O(1) wtihout using visibility matrix to track visited cell, just flip 1 to 0 after visiting      
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


kth largest element in stream
meetings room (interval )
diameter of tree (tree dfs)

Disappering elements in array (cyclic sort)
longest palindromic substring (tabulation technique using bottomsup approach)
