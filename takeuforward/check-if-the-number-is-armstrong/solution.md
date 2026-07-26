# Check if the Number is Armstrong

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/check-if-the-number-if-armstrong
- **Date:** 2026-07-26

## Solution

```cpp
class Solution {
public:
    bool isArmstrong(int n) {
    int cnt = log10(n) + 1;
    int sum = 0;
    int dup = n;
    while(n > 0){
        int lastDigit = n % 10;
        sum = sum + pow(lastDigit, cnt);
        n /= 10;
    }
    if(dup == sum){
        return true;
    }
    return false;
    }
    
};
```

---
*Generated automatically by LeetFeedback Extension*
