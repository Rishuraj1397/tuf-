# Check if the Array is Sorted I

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/check-if-the-array-is-sorted-i
- **Date:** 2026-07-26

## Solution

```cpp
class Solution {
public:
    bool arraySortedOrNot(int arr[], int n) {
        
        for(int i = 0; i < n-1; i++){
            if(arr[i] > arr[i+1]) return false;
        }
        return true;
    }
};

```

---
*Generated automatically by LeetFeedback Extension*
