# Largest Odd Number in a String

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/largest-odd-number-in-a-string
- **Date:** 2026-08-18

## Solution

```cpp
class Solution {
public:
    string largeOddNum(string s) {
        int i = s.size() - 1;

        while (i >= 0) {
            if ((s[i] - '0') % 2 == 1) {
                break;
            }
            i--;
        }

        if (i < 0) {
            return "";
        }

        int start = 0;

        while (start <= i && s[start] == '0') {
            start++;
        }

        return s.substr(start, i - start + 1);
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
