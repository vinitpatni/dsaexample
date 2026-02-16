- Longest Palindrome Subsequence
      <pre markdown="2"> 
        We will fill the dp 2 d array of size n*n. Base case
            Fro size 1 it will be always 1 as any string of size 1 is always palindrome
            For dp [i,j] = if (s.charAt(i) == s.charAt(j) then dp[i,j] = 2 + dp[i+1][j-1]
                     else if (s.charAt(i) != s.charAt(j) then dp[i,j] = Max (dp[i-1][j]), dp[i][j-1])
     </pre>
- k-tolerant palindrome (Find size of longest palidnrome subsequence and subtract it from length of string)     
- Largest Rectangle in Histogram
     <pre markdown="2"> 
       For each element in the array, find next small element and prev small element 
       Approach 1 :-  Using two foreach loop
          TimeComplexity :- O(n2) 
          SpaceComplexity :- O(n) 
      Approach 2 () :- Use monotonic stack to find next small element and prev small element
         TimeComplexity :- O(n)  Monotonic stack has O(n) because size of stack never exceeds n 
          SpaceComplexity :- O(n) Auxillary space for storing results
     </pre>
 - Find Median of Data Stream
        
      <pre markdown="2"> 
        Approach 1 :- Maintain maxHeap and minHeap as elements are added to the stream. if difference in size of two pq is greater than 1. then rebalance
        needs to be done across two heaps
            TimeComplexity (add(int num)) ->  O(log(n)) is cost of removing and adding element to the priority que
                           (getMedian() -> O(1) as depending on que sizes we can calculate median
            SpaceComplexity (Of O(n)) as we are maintaining all the elements of stream
     </pre>      
- Maximal Rectangle
     <pre markdown="2"> 
           Use Monotonic stack to solve problem of pattern (find first next smaller element, first prev small element)
           Solve Largest Rectangle in Histogram problem, based on which solution of this problem is build up
     </pre>
- Binary Cameras
      <pre markdown="2"> 
           Do DFS and apply greedy approach
              - install camera if any of the children is not monitored
              - if any of the children have camera, current node is considered monitored 
              - if both of the children are monitored, then return 0 as current node is not monitored
     </pre>
- Binary Tree Maximum Path Sum
   <pre markdown="2"> 
           Do DFS and consider left child and right child computation
             - if number is negative then adding anything to it reduces the overall value and if number is negative then return zero to its parent
             hence if node.val + Math.max(left, right) is negative then return zero to its parent.
     </pre>
- Palindrome pairs
     <pre markdown="2"> 
          For given string, you can find all its possible palindrome using following approach :-
           Repeat below process for each possible partition of the string
            1. First split into parts , left and right
            2. Check if left is palindrome, if yes then generate palindrome of right part of string
            3. If you append palindrome generated in above step to the left side of above string, you will possible palindrome
           Repeat above process for right part also :-
            1. First split into parts , left and right
            2. Check if right is palindrome, if yes then generate palindrome of left part of string
            3. If you append palindrome generated in above step to the right side of above string, you will possible palindrome
          TimeComplexity :- O(n*k) where k is size of each word.   
          SpaceComplexity :- O(n) Auxillary space for storing words in to hashmap 
     </pre>
- Search AutoComplete System
  <pre markdown="2"> 
          For trie, we need to maintain list of result on the prefix node itself, In this way we can avoid computation every time
     </pre>

     
