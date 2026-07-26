# Sum of Array Elements

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/sum-of-array-elements
- **Date:** 2026-07-26

## Solution

```cpp
class Solution{
public:
	int sum(int arr[], int n) {
	  int sUm = 0;

      for(int i = 0; i < n; i++){
        sUm += arr[i];
      }
      return sUm;
	}
};
```

---
*Generated automatically by LeetFeedback Extension*
