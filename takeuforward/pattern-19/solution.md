# Pattern 19

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-19
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
   private:
    void uperhf(int n) {
        for (int i = 0; i < n; i++) {
            for (int j = 1; j <= n  - i; j++) {
                cout << "*";
            }

            for (int j = 1; j <= 2 * i; j++) {
                cout << " ";
            }

            for (int j = 1; j <= n - i; j++) {
                cout << "*";
            }
            cout << endl;
        }
    }

    void lowerhf(int n) {
        for (int i = 1; i <= n; i++) {
            for (int j = 1; j <= i; j++) {
                cout << "*";
            }

            for (int j = 1; j <= 2 * n - 2 * i; j++) {
                cout << " ";
            }

            for (int j = 1; j <= i; j++) {
                cout << "*";
            }

            cout << endl;
        }
    }

   public:
    void pattern19(int n) {
        uperhf(n);
        lowerhf(n);
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
