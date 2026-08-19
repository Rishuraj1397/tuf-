# Pattern 6

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-6
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    void pattern6(int n) {
        for(int i = 0; i < n; i++){
            for(int j = 1; j <= n-i; j++){
                cout << j;
            }
            cout << endl;
        }
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
