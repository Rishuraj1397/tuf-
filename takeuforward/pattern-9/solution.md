# Pattern 9

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-9
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
   private:
    void pattern7(int n) {
        int num = 2 * n;
        for (int i = 1; i <= n; i++) {
            for (int j = 1; j <= n - i; j++) {
                cout << " ";
            }

            for (int j = 1; j <= 2 * i - 1; j++) {
                cout << "*";
            }

            cout << endl;
        }
    }
        void pattern8(int n) {
            for (int i = 1; i <= n; i++) {
                // For starting spaces
                for (int j = 0; j < i - 1; j++) {
                    cout << " ";
                }

                // For starting
                for (int j = 1; j <= (2 * n) - (2 * i) + 1; j++) {
                    cout << "*";
                }

                // //For ending spaces
                // for(int j = 0; j < i-1; j++){
                //     cout << " ";
                // }

                cout << endl;
            }
        }

   public:
    void pattern9(int n) {
        pattern7(n);
        pattern8(n);
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
