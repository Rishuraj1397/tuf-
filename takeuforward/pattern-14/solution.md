# Pattern 14

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-14
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    void pattern13(int n) {
        int cnt = 1;
        for(int i = 1; i <= n; i++){
            for(int j = 1; j <= i; j++){
                cout << cnt << " ";
                cnt++;
            }
            cout << endl;
        }
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
