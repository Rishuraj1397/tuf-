# Pattern 4

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-4
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    void pattern4(int n) {
        for(int i = 1; i < n+1; i++){
            for(int j = 1; j <= i; j++){
                cout << i;
            }
            cout << endl;
        }
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
