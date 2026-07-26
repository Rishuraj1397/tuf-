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

        // brute force approach using extra array temp


        // int* ans = new int[n];
        
        // for (int i = n-1; i >= 0; i--) {
        //     ans[n-i-1] = arr[i];
        // }
        
        // for(int i=0; i < n; i++) {
        //     arr[i] = ans[i];
        // }
        
        // delete[] ans; 
        
        // return;


        // Optimal approach by swapping them inline


        int p1 = 0, p2 = n - 1;
        while (p1 < p2) {
            int tmp = arr[p1];
            arr[p1] = arr[p2];
            arr[p2] = tmp;
            p1++;
            p2--;
        }
        return;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
