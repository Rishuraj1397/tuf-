# Isomorphic String

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/isomorphic-string
- **Date:** 2026-08-21

## Solution

```cpp
class Solution {
public:
    bool isomorphicString(string s, string t) {
    	//your code goes here
        int mapST[26] = {0};
        int mapTS[26] = {0};

        for(int i = 0; i < s.size(); i++){
            int a = s[i] - 'a';
            int b = t[i] - 'a';
            
            if (mapST[a] != 0 && mapST[a] != b + 1){
                return false;
            }
            if (mapTS[b] != 0 && mapTS[b] != a + 1){
                return false;
            }

            mapST[a] = b + 1;
            mapTS[b] = a + 1;
        }

        return true;
    }
};
```

---
*Generated automatically by LeetFeedback Extension*
