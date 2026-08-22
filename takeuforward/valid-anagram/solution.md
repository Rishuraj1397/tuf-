# Valid Anagram

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/valid-anagram
- **Date:** 2026-08-22

## Solution

```cpp
class Solution{	
	public:
		bool anagramStrings(string& s,string t){
			//your code goes here
            sort(s.begin(), s.end());
            sort(t.begin(), t.end());
            return s == t;
		}
};
```

---
*Generated automatically by LeetFeedback Extension*
