# Palindrome Check

## Problem Information
- **Platform:** Takeuforward
- **Difficulty:** Unknown
- **URL:** https://takeuforward.org/plus/dsa/problems/palindrome-check
- **Date:** 2026-08-18

## Solution

```cpp
class Solution{	
	public:		
		bool palindromeCheck(string& s){
			//your code goes here
            int i = 0;
            int j = s.length() - 1;

            while (i < j){
                if(s[i] != s[j]){
                    return false;
                }else{
                    i++;
                    j--;
                }

            }
            return true;
		}
};
```

---
*Generated automatically by LeetFeedback Extension*
