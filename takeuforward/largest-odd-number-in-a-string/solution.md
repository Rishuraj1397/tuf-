# Largest Odd Number in a String

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/largest-odd-number-in-a-string
- **Date:** 2026-08-19

## Solution

```cpp
class Solution {
   public:
    string largeOddNum(string& s) {
        // your code goes here

        // This one is for finding the first odd digit from rightmost
        int i = s.size() - 1;

        while (i >= 0 && (s[i] - '0') % 2 == 0) {
            i--;
        }

        if (i < 0) return "";

        s.erase(i + 1);

        int start = 0;

        while (start < s.size() && s[start] == '0') {
            start++;
        }
        s.erase(0, start);
        return s;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
