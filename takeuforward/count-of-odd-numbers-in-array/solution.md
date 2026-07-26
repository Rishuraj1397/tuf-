# Count of odd numbers in array

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/count-of-odd-numbers-in-array
- **Date:** 2026-07-26

## Solution

```cpp
class Solution{
public:
    int countOdd(int arr[], int n){
          int cnt = 0;

          for(int i = 0; i < n; i++){
            if(arr[i] % 2 == 1){
                cnt++;
            }
          }
          return cnt;
    }
};

```

---
*Generated automatically by LeetFeedback Extension*
