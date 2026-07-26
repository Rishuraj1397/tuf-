# GCD of Two Numbers

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/gcd-of-two-numbers
- **Date:** 2026-07-26

## Solution

```cpp
class Solution {
public:
    int GCD(int n1,int n2) {
        int largest = 1;

        for(int i = 2; i <= min(n1, n2); i++){
            if(n1 % i == 0 && n2 % i == 0){
                largest = i;
            }
        }
        return largest;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
