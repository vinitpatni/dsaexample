- Longest Plaindrome SubString :-
     <pre markdown="2"> 
      Use Tabulation Technique and Bottomsup Approach for solving it.
            String of length 1 is always palindrome
            String of length 2 is palidnrome if (s[0] == s[1])
            String of length n is palindrome if  S[0] == s[n-1] &&  substring(1,n-2) is palindrome
     </pre>        
- Find Median of Data Stream
        
      <pre markdown="2"> 
        Approach 1 :- Maintain maxHeap and minHeap as elements are added to the stream. if difference in size of two pq is greater than 1. then rebalance
        needs to be done across two heaps
            TimeComplexity (add(int num)) ->  O(log(n)) is cost of removing and adding element to the priority que
                           (getMedian() -> O(1) as depending on que sizes we can calculate median
            SpaceComplexity (Of O(n)) as we are maintaining all the elements of stream
     </pre>  
- Decode ways
      <pre markdown="2"> 
      Use Bottomsup approach for solving
            String of length 0 and length 1 has 1 way of decoding
            No of ways to decode char at index i = dp [i-1] + dp[i];
   
            if (s.charAt(i) is not '0') {
                //there would be number of ways equal to dp[i-1]
                dp[i] = dp[i] + dp[i-1]
            }
            if (s.charAt(i-1) is not '0' && substring(i-1,i+1) is in range 1 to 26 {
                //there would be number of ways equal to dp[i-1]
                dp[i] = dp[i] + dp[i-2]
            }
     </pre>
- Partition Equal Subset Sum :-
     Use 0/1 knapsack pattern for filling up the table and check whether it is possible to reach half of the target sum of given input array.
          <pre markdown="2"> 
       TimeComplexity -> O(m*n) where m is is size of input array and n is the target sum
       SpaceComplexity ->O(m)  Space Optimized and use boolean 2d array
         </pre>
- Edit Distance <br>
      - hor -> ro <br>
            <pre markdown="2"> 
              Replace -> Cost of transfroming (ho->r) + 1 (cost of replacing r with o) = 3<br>
             Insert ->  Cost of transfroming (hor->r) + 1 (cost of insert o) = 3 <br>
             Delete ->   Cost of transfroming (ho->ro) + 1 (cost of delete r) = 2 <br>
             </pre>
       - abc -> bcd <br>
              <pre markdown="2"> 
              Replace -> Cost of transfroming (ab->bc) + 1 (cost of replacing c with d) = 3 <br>
              Insert ->  Cost of transfroming (abc->bc) + 1 (cost of insert d) = 3 <br>
              Delete ->   Cost of transfroming (ab->bcd) + 1 (cost of delete c) = 2 <br>
             </pre>
