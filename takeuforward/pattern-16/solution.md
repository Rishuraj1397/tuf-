# Pattern 16

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-16
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    void pattern16(int n) {
        char ch = 'A';
        for(int i = 1; i <= n; i++){
            for(int j = 1; j <= i; j++ ){
                cout << ch;
            }
            ch++;
            cout <<   endl;
        }

    }
};
```

---
*Generated automatically by LeetFeedback Extension*
