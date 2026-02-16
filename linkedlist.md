
-  Middle of linkedList
      <pre markdown="2"> 
       Approach 1 :-  Using 2 scans. First Scan to get size of linked list and find middle node index.
                      Second scan to navigate to middle index of linkedlist
          TimeComplexity :- O(n)
          SpaceComplexity :- O(1)
      Approach 2 (With Single Pass Only) :- Use slow and fast pointer to reach middle of linked list in single pass
     </pre>
  - Reverse LinkedList
      <pre markdown="2"> 
       Approach 1 :-  Iterative approach using prev and curr pointer
          TimeComplexity :- O(n)
          SpaceComplexity :- O(1)
      Approach 2  :- Use recursion for reversing linked list
          TimeComplexity :- O(n)
          SpaceComplexity :- O(n) because space taken by recursion depth which is n
      </pre>
   - Add 1 to LinkedList
      <pre markdown="2"> 
       Approach 1 :-  Use recursion to access each element of LL
          TimeComplexity :- O(n)
          SpaceComplexity :- O(n) auxillary space used by recursion
      Approach 2  :- reverse ll iteratively and add 1 to first node of ll and propagate carry, In the end again reverse given ll to return head pointer
          TimeComplexity :- O(n)
          SpaceComplexity :- O(1) because of iterative approach
      </pre>    
  - Merge two sorted list (Use dummy node and two pointer approach)
  - Check Palindrome LinkedList
      <pre markdown="2"> 
       Approach 1 :-  collect all elements of linkedlist and check if it is palindrome or not
          TimeComplexity :- O(n)
          SpaceComplexity :- O(n)
      Approach 2  :- First find middle and and then reverse from middle of linkedlist to end. You have two points first and last. Compare them
          TimeComplexity :- O(n)
          SpaceComplexity :- O(1)
      </pre>  
