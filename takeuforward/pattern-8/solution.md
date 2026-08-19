# Pattern 8

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-8
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    void pattern8(int n) {
        for(int i = 1; i <= n; i++){

            //For starting spaces
            for(int j = 0; j < i-1; j++){
                cout << " ";
            }

            //For starting
            for(int j = 1; j <= (2*n)-(2*i)+1; j++){
                cout << "*";
            }

            // //For ending spaces
            // for(int j = 0; j < i-1; j++){
            //     cout << " ";
            // }

            cout << endl;
        }

    }
};
```

---
*Generated automatically by LeetFeedback Extension*
