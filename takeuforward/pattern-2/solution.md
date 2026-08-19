# Pattern 2

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-2
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    void pattern2(int n) {
        for(int i = 0; i < n; i++){
            for(int j = 0; j <= i; j++){
                cout << "*";
            }
            cout << endl;
        }
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
