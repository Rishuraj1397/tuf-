# Sum of first last element in array

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/sum-of-first-last-element-in-array
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    int sumOfFirstAndLast(vector<int>& nums) {
        int n = nums.size();
        return nums[0] + nums[n - 1];
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
