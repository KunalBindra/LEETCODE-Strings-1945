# LEETCODE-Strings-1945
### Problem Summary
Given a string `s` consisting of lowercase English letters, we need to:
1. Convert each letter to its position in the alphabet: 'a' -> 1, 'b' -> 2, ..., 'z' -> 26.
2. Concatenate these numbers to form a new string.
3. Convert the new string into an integer.
4. Perform `k` iterations where, in each iteration, the integer is replaced by the sum of its digits.
5. Return the resulting integer after `k` iterations.

### Example
**Input:** `s = "leetcode", k = 2`  
**Output:** `6`

**Explanation:**
1. Convert each letter to its position:  
   'l' -> 12, 'e' -> 5, 'e' -> 5, 't' -> 20, 'c' -> 3, 'o' -> 15, 'd' -> 4, 'e' -> 5  
   Concatenate to form the string "12552031545".
   
2. First iteration: Sum the digits of "12552031545"  
   1 + 2 + 5 + 5 + 2 + 0 + 3 + 1 + 5 + 4 + 5 = 33

3. Second iteration: Sum the digits of "33"  
   3 + 3 = 6

Result after `k = 2` iterations is `6`.

### Dry Run of the Solution

#### Input
- `s = "leetcode"`
- `k = 2`

#### Step-by-Step Execution

1. **Convert letters to their positions in the alphabet:**
   - 'l' -> 12, 'e' -> 5, 'e' -> 5, 't' -> 20, 'c' -> 3, 'o' -> 15, 'd' -> 4, 'e' -> 5  
   Concatenated string = "12552031545".

2. **Convert concatenated string to an integer and sum the digits (1st iteration):**
   - Number: `12552031545`
   - Sum of digits: \(1 + 2 + 5 + 5 + 2 + 0 + 3 + 1 + 5 + 4 + 5 = 33\)

3. **Sum the digits again (2nd iteration):**
   - Number: `33`
   - Sum of digits: \(3 + 3 = 6\)

#### Output
- The result after `k = 2` iterations is `6`.

### Conclusion
The dry run shows how the string "leetcode" is transformed and iteratively reduced to a single integer after the given number of iterations. The answer for this example is `6`.
