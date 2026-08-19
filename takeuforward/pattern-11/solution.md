# Pattern 11

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-11
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    void pattern11(int n) {
        for(int i = 1; i <= n; i++){
            int start = (i % 2 == 0) ? 0 : 1;
            for(int j = 0; j < i; j++){
                cout << start << " ";
                start = 1 - start;
            }
            cout << endl;
        }
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
