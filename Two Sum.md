### :shit:Approach 1  (Brute Force) 
```python
class Solution:
    def twoSum(self, nums, target):
        """
        :type nums: List[int]
        :type target: int
        :rtype: List[int]
        """
        try:
            for i in range(len(nums)-1):  # look up from index 0 to n-1
                for j in range(i+1, len(nums)): # look up from index i+1 to n
                    if nums[i] + nums[j] == target: 
                        return [i, j]
        except:
            "No two sum solution"
```

#### Complexity Analysis
- Time complexity: O(n^2)
  
  For each element, we try to find its complement by looping through the rest of array which takes O(n) time. So, the time complexity is O(n^2).
  
 - Space complexity: O(1)
 
### :shit:Approach 2 （hash table)
```python
class Solution:
    def twoSum(self, nums, target):
      """
      :type nums: List[int]
      :type target: int
      :rtype: List[int]
      """
      try: 
        dict = {}
        for i in range(len(nums)):
          if target-nums[i] in dict:
            return [i, dict[targ
           
```
