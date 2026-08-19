# Pattern 15

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-15
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    void pattern15(int n) {
        for(int i = 0; i < n; i++){
            char ch = 'A';
            for(int j = 0; j < n-i; j++){
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
