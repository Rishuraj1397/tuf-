# Check for Perfect Number

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/check-for-perfect-number
- **Date:** 2026-07-26

## Solution

```cpp
class Solution {
public:
    bool isPerfect(int n) {
        if(n == 1){
            return false;
        }

        int sum = 0;
        
        for(int i = 1; i * i <= n; i++){
            if(n % i == 0){
                sum += i;

                if(n/i != n && i != n/i){
                    sum += (n/i);
                } 
            }
        }
        if(sum == n){
            return true;
        }
        return false;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
