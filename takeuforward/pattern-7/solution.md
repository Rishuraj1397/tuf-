# Pattern 7

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-7
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    void pattern7(int n) {
        for(int i = 1; i <= n; i++){
            
            for(int j = 1; j <= n-i; j++){
                cout << " ";
            }

            for(int j = 1; j <= 2*i-1; j++){
                cout << "*";
            }


            
            cout << endl;
        }
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
