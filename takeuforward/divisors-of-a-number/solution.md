# Divisors of a Number

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/divisors-of-a-number
- **Date:** 2026-07-26

## Solution

```cpp
class Solution {
public:
    vector<int> divisors(int n) {
        vector<int> ans;

        for(int i = 1; i <= n; i++){
            if(n % i == 0){
                ans.push_back(i);
            }
        }
        return ans;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
