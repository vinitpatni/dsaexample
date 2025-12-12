- Number of Islands (graph dfs)
     <pre markdown="2"> 
       TimeComplexity -> O(m*n)
       SpaceComplexity ->O(m*n) in the worst case due to the recursion stack but auxiallary space can be O(1) wtihout 
       using visibility matrix to track visited cell, just flip 1 to 0 after visiting</pre>
- All Powersets (recursive backtracking)
- All Permutations (recursive backtracking)
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
- serialize and deserialize n-ary tree
- searilize and deseralize tree
      <pre markdown="2"> 
       Approach 1 :- Use Preorder traversal to store elements while serialize and Queue while deserialize 
          TimeComplexity :- O(n) as we are dfs 
          SpaceComplexity :- log(n) for recursion depth and queue which takes O(n) to store elements 
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

Longest palindrome substring (dynamic programming and tabulation technique)

kth largest element in stream
meetings room (interval )
diameter of tree (tree dfs)

Disappering elements in array (cyclic sort)
longest palindromic substring (tabulation technique using bottomsup approach)
