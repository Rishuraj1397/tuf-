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
        // first menthod
        // ----------------------------------
        // int n = str.size();

        // sort(str.begin(), str.end());

        // string first = str[0];
        // string last = str[n - 1];

        // string ans = "";

        // for (int i = 0; i < min(first.length(), last.length()); i++) {
        //     if (first[i] != last[i]) {
        //         break;
        //     }
        //     else {
        //         ans = ans + first[i];
        //     }
        // }

        // return ans;

        // second method -----------------------

        string ans = "";
        int n = str.size();
        for (int i = 0; i < str[0].size(); i++) {
            char ch = str[0][i];

            bool match = true;

            for (int j = 1; j < n; j++) {
                if (str[j].size() < i || ch != str[j][i]) {
                    match = false;
                    break;
                }
            }
            if (match == false) {
                break;
            } else {
                ans.push_back(ch);
            }
        }
            return ans;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
