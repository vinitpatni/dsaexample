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
-  Encode and Decode String (contain special characters)
      <pre markdown="2"> 
        Use size of string followed by # as delimiter 
         TimeComplexity :- O(n)
         SpaceComplexity :- O(n) 
      </pre>
- Decode String  (s = "3[a]2[bc]" = "aaabcbc")     
