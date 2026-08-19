# Pattern 12

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-12
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    void pattern12(int n) {
        for(int i = 1; i <= n; i++){
            // number
            for(int j = 1; j <= i; j++){
                cout << j;
            }

            for(int j = 1; j <= (2*n) - (2*i); j++){
                cout << " ";
            }


            for(int j = i; j >= 1; j--){
                cout << j;
            }
            cout << endl;
        }
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
