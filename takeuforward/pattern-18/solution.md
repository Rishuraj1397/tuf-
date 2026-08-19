# Pattern 18

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-18
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    void pattern18(int n) {
        char chara = 'A' + n - 1;
        for(int i = 1; i <= n; i++){
            char ch = chara;
            for(int j = 1; j <= i; j++){
                cout << ch << " ";
                ch++;
            }
            chara--;
            cout << endl;
        }

    }
};
```

---
*Generated automatically by LeetFeedback Extension*
