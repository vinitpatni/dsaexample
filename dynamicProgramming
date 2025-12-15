- Longest Plaindrome SubString :-
      Use Tabulation Technique and Bottomsup Approach for solving it.
            String of length 1 is always palindrome
            String of length 2 is palidnrome if (s[0] == s[1])
            String of length n is palindrome if  S[0] == s[n-1] &&  substring(1,n-2) is palindrome
- Partition Equal Subset Sum :-
     Use 0/1 knapsack pattern for filling up the table and check whether it is possible to reach half of the target sum of given input array.
          <pre markdown="2"> 
       TimeComplexity -> O(m*n) where m is is size of input array and n is the target sum
       SpaceComplexity ->O(m)  Space Optimized and use boolean 2d array
         </pre>
- Edit Distance
      Transfrom hor -> ro
            Cost of transforming 
              Replace -> Cost of transfroming (ho->r) + 1 (cost of replacing r with o) = 3
              Insert ->  Cost of transfroming (hor->r) + 1 (cost of insert o) = 3
              Delete ->   Cost of transfroming (ho->ro) + 1 (cost of delete r) = 2

     - abc -> bcd
             Cost of transforming 
              Replace -> Cost of transfroming (ab->bc) + 1 (cost of replacing c with d) = 3
              Insert ->  Cost of transfroming (abc->bc) + 1 (cost of insert d) = 3
              Delete ->   Cost of transfroming (ab->bcd) + 1 (cost of delete c) = 2
