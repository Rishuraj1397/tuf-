# Pattern 17

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/pattern-17
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
public:
    void pattern17(int n) {
        for(int i = 1; i <= n; i++){
            for(int j = 1; j <= n-i; j++){
                cout << " ";
            }


            char ch = 'A';
            int numberOfCharacter = 2 * i - 1;
            for(int j = 1; j <= numberOfCharacter; j++){
                cout << ch;
                if(j < i){
                    ch++;
                }else{
                    ch--;
                }
            }

            for(int j = 1; j <= n-i; j++){
                cout << " ";
            }
            cout << endl;
        }

    }
};
```

---
*Generated automatically by LeetFeedback Extension*
