# Pattern 10

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-10
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
private:
    void pattern2(int n) {
        for(int i = 0; i < n; i++){
            for(int j = 0; j <= i; j++){
                cout << "*";
            }
            cout << endl;
        }
    }

    void pattern5(int n) {
        for(int i = 0; i < n; i++){
            for(int j = 0; j < n-i; j++){
                cout << "*";
            }
            cout << endl;
        }
    }
    
public:
    void pattern10(int n) {
        pattern2(n);
        pattern5(n-1);
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
