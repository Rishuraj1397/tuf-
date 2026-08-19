# Pattern 5

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-5
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    void pattern5(int n) {
        for(int i = 0; i < n; i++){
            for(int j = 0; j < n-i; j++){
                cout << "*";
            }
            cout << endl;
        }
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
