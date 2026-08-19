# Print X N numbers of times

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/print-x-n-numbers-of-times
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    void printX(int X, int N) {
        for(int i = 0; i < N; i++){
            if (i > 0){
                cout << " ";
            }
            cout << X;
        }
        cout << endl;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
