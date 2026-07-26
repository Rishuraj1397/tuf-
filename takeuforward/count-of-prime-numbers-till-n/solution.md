# Count of Prime Numbers till N

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/count-of-prime-numbers-till-n
- **Date:** 2026-07-26

## Solution

```cpp
class Solution {
public:
    int primeUptoN(int n) {
        int cnt = 0;

        for (int num = 2; num <= n; num++) {
            bool isPrime = true;

            for (int i = 2; i * i <= num; i++) {
                if (num % i == 0) {
                    isPrime = false;
                    break;
                }
            }

            if (isPrime) {
                cnt++;
            }
        }

        return cnt;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
