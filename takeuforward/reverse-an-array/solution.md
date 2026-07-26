# Reverse an array

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/reverse-an-array
- **Date:** 2026-07-26

## Solution

```cpp
class Solution {
public:
    void reverse(int arr[], int n) {
        int* ans = new int[n];
        
        for (int i = n-1; i >= 0; i--) {
            ans[n-i-1] = arr[i];
        }
        
        for(int i=0; i < n; i++) {
            arr[i] = ans[i];
        }
        
        delete[] ans; 
        
        return;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
