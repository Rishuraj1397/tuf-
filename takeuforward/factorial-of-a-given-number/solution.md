# Factorial of a given number

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/factorial-of-a-given-number-i
- **Date:** 2026-07-25

## Solution

```cpp
class Solution {
public:
    int factorial(int n) {
        if (n == 0){
            return 1;
        }

        int ans = 1;

        for(int i = 1; i <= n; i++){
            ans = ans * i;
        }
        return ans;
    }
};

```

---
*Generated automatically by LeetFeedback Extension*
