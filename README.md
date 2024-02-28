# DSA_two_pointers
Write a function that reverses a string. The input string is given as an array of characters s.

You must do this by modifying the input array in-place with O(1) extra memory.
Example 1:
```
Input: s = ["h","e","l","l","o"]
Output: ["o","l","l","e","h"]
```
Solution
```
class Solution:
    def reverseString(self, s: List[str]) -> None:
        """
        Do not return anything, modify s in-place instead.
        """
        self.s=s
        left=0
        right=len(s)-1
        while left < right:
            arr=self.s[left]
            self.s[left]=self.s[right]
            self.s[right]=arr
            left+=1
            right-=1
```
