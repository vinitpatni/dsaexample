
- Given a string s, return true if the s can be palindrome after deleting at most one character from it
     <pre markdown="2"> 
       Approach 1 :- Find Longest Palindrome Subsequence and subtract it from the length of string
                  if difference is less than 1 then true otherwise false
       Approach 2 (Better approach) :- if left and right are not matching, then either delete left character or delete right character and recursively keep on checking  
     </pre>
- Check if characters of a given string can be rearranged to form a palindrome
      <pre markdown="2"> 
       Approach 1 :-  Get frequency of each character and check if characters of odd frequency is greater than 1
          TimeComplexity :- O(n)
          SpaceComplexity :- O(n) Using hashmap to store frequency of each character of string
      Approach 2 (With Constant Space) :-
          Calculate BitVector for each character in the string.
          for (char ch : s.toCharArray()) {
               int leftShift = 1 << ch - 'a'
               bitVector = bitVector ^ leftShift; (//taking xor which toggles (set to 1 if frequency is odd and 0 if frequency is even)
          }
        // How to check if single bit is set in binary number, if (no & no - 1) == 0 //means single bit is set
          return bitVector & bitVector - 1;
     </pre>
- Longest Palindrome Subsequence
      <pre markdown="2"> 
        We will fill the dp 2 d array of size n*n. Base case
            Fro size 1 it will be always 1 as any string of size 1 is always palindrome
            For dp [i,j] = if (s.charAt(i) == s.charAt(j) then dp[i,j] = 2 + dp[i+1][j-1]
            else if (s.charAt(i) != s.charAt(j) then dp[i,j] = Max (dp[i-1][j]), dp[i][j-1])
     </pre>
- k-tolerant palindrome (Find size of longest palindrome subsequence and subtract it from length of string)     
