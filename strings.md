- CountBinary Strings in O(n) (Equal number of 0 and 1 and they should be consecutive)
     <pre markdown = "2"> 
     - Initialize prev=0 and curr=1. Start from index i=1 and increment current till char at i == i-1
     - if i != i-1 then capture the result reset prev and curr   
   </pre>
-Minimum number of flips to make binary string alternating 
   <pre markdown = "2"> 
     - Use sliding window technique and double the size of string
     - First calculate once for first window (0 to n-1) zeroMin and oneMin
     - We don't need to do recalculation for subseqeunt window like (1 to n), (2 to n+1)
       Just compare with the expected one using inclusion and exclusion character and expected value of indices for 
       both combination (010..) and (101..) and edit the zeroMin and oneMin variable at each step
     - Capture the smallest value
   </pre>
- Time need to rearrange binary string
   
   <pre markdown = "2"> 
    O(n) solution with constant space
         
          for (char ch : s.toCharArray()) {
            if (ch == '0') {
                zeros++;
            } else if (zeros > 0) {
                time = Math.max(time + 1, zeros);
            }
        }  
   </pre>
-  Longest Subarray With Equal Number of 0s and 1s
     <pre markdown = "2"> 
     - Replace all 0 with -1
     - If sum is same at two indices that means equal number of 1 and 0 exists between those two indices. Capture the result   
   </pre>   
-  Encode and Decode String (contain special characters)
      <pre markdown="2"> 
        Use size of string followed by # as delimiter 
         TimeComplexity :- O(n)
         SpaceComplexity :- O(n) 
      </pre>
- Decode String  (s = "3[a]2[bc]" = "aaabcbc")     
