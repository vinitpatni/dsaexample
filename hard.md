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
 
