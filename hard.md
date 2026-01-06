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
