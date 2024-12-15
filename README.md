# DNA-Sequencing
Problem definition
Substring matching is the process of determing whether a shorter string is contained within a longer string.
Python provides a find method that returns the lowest index where the substring is found in the index range,
start <= index <= end.
The start and end for this exercise will be mandatory. If the substring is not found, -1 is returned.

The exercise:
a. 
    Without using the find method, write a function that behaves exactly the same. The resulting format should e:
    find(some_string, substring, start, end).

b.
    Often it is required to find all the index locations that a substring is found, not just the first one. Write a 
    function called multi_find(some_string, substring, start, end) that returns a string that contains zero or more indices
    separated by commas. If the substring is not found, an empty string is returned.

c. 
    Write a program that exercise both the find and multi-find functions, including their use in boolean functions.  Create strings using only the base letters ATCG and search for substrings within them.

************************************************************************************************************************************************************************************

Planning and analysis
find function:
- find(some_string, substring, start, end)
- Take some_string, starting from index 0, slice from 0 to 0+len(substring) and check if    equal to substring
- If equal to substring return index, else -1 returned.

1. Set a length variable as the length of the substring.
2. For i in range(len(some_string))
3. If some_string[i:i+1]==substring, index = i. elif end - i+len()substring >= len(substring), i++ and continue. Else index = -1, break
4. Return index.

multi-find function:
- multi_find(some_string, substring, start, end)
- Take a string, start from index 0 and use the find function to find every index that contains the substring.


