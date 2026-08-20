# Longest Common Prefix

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/longest-common-prefix
- **Date:** 2026-08-20

## Solution

```cpp
class Solution {
public:
    string longestCommonPrefix(vector<string>& str) {
        int n = str.size();

        sort(str.begin(), str.end());

        string first = str[0];
        string last = str[n - 1];

        string ans = "";

        for (int i = 0; i < min(first.length(), last.length()); i++) {
            if (first[i] != last[i]) {
                break;
            }
            else {
                ans = ans + first[i];
            }
        }

        return ans;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
