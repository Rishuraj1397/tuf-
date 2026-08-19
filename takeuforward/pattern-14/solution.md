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
    void pattern14(int n) {
        for(int i = 1; i <= n; i++){
            char ch = 'A';
            for(int j = 1; j <= i; j++){
                cout << ch;
                ch++;
            }
            cout << endl;
        }

    }
};
```

---
*Generated automatically by LeetFeedback Extension*
